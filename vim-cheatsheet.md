# justin-vim-cheatsheet
Personalised list of vim commands that help speed up coding efficiency

- Do not enter insert mode
- Stop using hjkl (remove fine-grainedness)
- Use f and t 

# Disable Keys

`~/.vimrc`

```
inoremap <Up> <Nop> 
inoremap <Down> <Nop>
inoremap <Left> <Nop>
inoremap <Right> <Nop>
nnoremap <Up> <Nop>
nnoremap <Down> <Nop>
nnoremap <Left> <Nop>
nnoremap <Right> <Nop>
inoremap <backspace> <Nop>
nnoremap <backspace> <Nop>
```

# Always Search 

```
/<search-word>
```

# Move to Next 

```
*
#
```

# (Absolute) Line numbers

```
:<line-number>
```

```
<line-number>G
```

# Move within Line

```
0
^
```

```
$
```

```
I
```

```
A
```


```
f<character>
```

```
t<character>
```
# Copying a Bunch Of Lines

Highlight Line
```
V
```

Highlight Block
```
Ctrl+V
```

Yank
```
yy
```

```
d
```

Paste
```
P
```

# Replace Inside

# Insert a Line 

insert line between
```
o
```

insert line before
```
O
```

# Copy Pasting

# Record and apply a Macro


Recording macro
```
q<macro-name>
...
...
...
q
```

Apply macro to single line
```
@q
```

```
:normal @n
```

# Redo and Undo

```
u
```

```
Ctrl+r
```

# Removes line containing String

```
:g/<string>/d
```

# Delete using relative number

```
set relativenumber
``

```
<number-of-lines>dd
d<number-of-lines>j
```


```
set norelativenumber
```

# Copy Lines 

```
:<1st-line-number>,<2nd-line-number>co.
```

# Delete Lines using Reference

```
:<1st-line-number>,<2nd-line-number>d
```

# High, Middle, Low

```
H
M
L
```

# Adding and removing parantheses 

```
ciw '' Esc P

```

# Adding many hyphens (for separator)

```
<no-hyphhes>a<Esc>
```
Remember to escape. Many times vs code will screw you over

# Adding multiple lines with the same text 

```
<no-of-lines>o 
```

Be patient to wait

# Add line to top

```
<no-of-lines>O
```

# Positioning Hands

Feel bumps of `j` to mean down. 
