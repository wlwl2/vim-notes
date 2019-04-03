# vim-shortcuts

## Copy/cut and paste selection (command mode).
1. Press `v` to select from where your cursor is.
2. Move the cursor to select, using `h`,`j`,`k`, or `l`, or the arrow keys.
3. Press `y` to copy it, or `d` to cut it.
4. Move your cursor to the line ABOVE where you want to paste.
5. Press `p` to paste it on the line AFTER the cursor.

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
