# justin-vim-cheatsheet
Personalised list of vim commands that help speed up coding efficiency

- Do not enter insert mode
- Stop using hjkl (remove fine-grainedness)
- Use f and t 
- Type less and be fast. Not type more and sound fast.
- Feel bumps of `j` to mean down. 

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

# Always search 

```
/<search-word>
```

# Move to matching bracket

```
%
```

# Move to line (absolute)

```
:<line-number>
```

```
<line-number>G
```

# Move within Line

Move cursor to beginning
```
0
```
Move cursor to end
```
$
```
Move cursor to beginning (insert mode)
```
I
```
Move cursor to end (insert mode)
```
A
```
Move cursor to next <character>
```
f<character>
```

Move cursor just before next <character>
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

Yank entre line
```
yy
```

Delete entire line
```
dd
```

Paste
```
P
p
```


# Replace Inside

```
ciw
```

```
ci"
```

```
ci(
```

```
ci[
```

# Insert on new line

Insert next 
```
o
```

Insert before
```
O
```

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

Copy lines and paste to current line
```
:<1st-line-number>,<2nd-line-number>co.
```

# Delete Lines using Reference

Delete lines
```
:<1st-line-number>,<2nd-line-number>d
```

# High, Middle, Low

```
H
M
L
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

```
<no-of-lines>O
```



