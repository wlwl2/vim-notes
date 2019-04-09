# vim-shortcuts

## Copy selection to clipboard (command mode).
1. Press `v` to select from where your cursor is. DO NOT hold `v`.
2. Move the cursor to select, using `h`,`j`,`k`, or `l`, or the arrow keys.
3. Type in `"+y` (Remember to add the double quotes at the start of this command).

## Copy/cut and paste selection (command mode).
1. Press `v` to select from where your cursor is. DO NOT hold `v`.
2. Move the cursor to select, using `h`,`j`,`k`, or `l`, or the arrow keys.
3. Press `y` to copy it, or `d` to cut it.
4. Move your cursor onto the character where you want to paste 
(selection is pasted AFTER this character).
5. Press `p` to paste selection AFTER this character.

## Copy/cut and paste multiple lines (command mode).
1. Press `shift+v` or `V` to select the line on your cursor. DO NOT hold `shift-v` or `V`.
2. Move the cursor to select lines, using `h`,`j`,`k`, or `l`, or the arrow keys.
3. Press `y` to copy it, or `d` to cut it.
4. Move your cursor to the line where you want to paste
(selection is pasted on the line AFTER this line).
5. Press `p` to paste it on the line AFTER the cursor/on the next line.

### This does not work by default using gvim on Windows.
See: Vim visual selection method differs between Windows & Linux?
https://unix.stackexchange.com/questions/170754/vim-visual-selection-method-differs-between-windows-linux

#### In short:

1. In `_vimrc` change:
```
set nocompatible
source $VIMRUNTIME/vimrc_example.vim
source $VIMRUNTIME/mswin.vim
behave mswin
```
2. To:
```
set nocompatible
source $VIMRUNTIME/vimrc_example.vim
