# TODO

- figure out tabs and nerdtree/sidebar methodology
- code folding
- https://vim.fandom.com/wiki/Using_tab_pages
- replace NERDTree with vim's default file explorer
- :help user-manual

# Sort this:

ciw — deletes the word you’re hovering and automatically puts you in INSERT mode
(change inside word) C — deletes from cursor to end of line and puts you in
INSERT mode dt<char> — deletes from your cursor to the next instance of the
character you specify (delete to <character>) ~ — toggles the case [upper/lower]
on the character hovered or selected (tilde; key below Esc for standard
keyboards) ggvG= — auto-indent the entire file (goto beginning, enter VISUAL
mode, go/select to end of file, and indent lines [==] selected)

# Main

:open file - open file in current tab :vs file - open file in vertical split
:bn - switch to nth buffer x/X - delete current/previous char A - $a a - li c -
if in visual > remove selected and enter insert mode ce - de+i cc - dd+i
Ctrl+G - show status message Ctrl+O/I - go to prev/next cursor position v:!ls /
:r !ls - prints the output of `ls` in the current line gv - reselect previous
selection :set ic/noic - make search case insensitive/sensitive Ctrl+D - show
suggestions when typing `:` commands or passing arguments Ctrl+C - return to the
normal mode

# Search & Replace

\*/# - find next/prev occurrence of this word /word - search for word. n/N -
show next/previous occurrence % - go to matching ([{ :%s/old/new/gc -
search&replace with a prompt

# Tabs

- :tabfind file - open file in new tab
- gt/T - go to the right/left tab ngt - go to the nth tab :tabs - list all tabs

# Windows

Ctrl+w v/s - open new vim window on the left/bottom Ctrl+w c - close window

- Ctrl+w l/h/j/k - switch to the window to the right/left/below/above Ctrl+w
  Ctrl+w - toggle between windows Ctrl+w </>/-/+ - decrease/increase current
  window horizontally/vertically Ctrl+w |- maximize current window
  horizontally/vertically Ctrl+w = - make all windows have equal size

# NERDTree

Ctrl+n - toggle NERDTree window Ctrl+s - open current file in NERDTree

# Misc

`sed -n l` - show key codes

# Markers

mk - make marker `k` y'k - copy from marker `k` till current position :marks -
list all marks

# Folding

zf'k - fold from marker 5:16fo - fold lines 5-16 zo - unfold

# Reformatting

=i{ - reformat current scope

# Vim's file explorer:

:Ex or :Vexplore

# Macros

qa - start recording a macro `a` q - finish recording @a - replay a macros
