# Vim cheat sheet

This list of Vim command is only the most useful command I use.
If you want to see all commands available for Vim you should check [vim documentation](https://vimhelp.org/).  
I highly recommend you to use the [vimtutor](https://vimhelp.org/usr_01.txt.html#vimtutor) to learn the basics of Vim.

- **Move**
  > `h` (left), `j` (down), `k` (up), `l` (right)  
  > `0` to start of the line  
  > `w` to first character of next word  
  > `$` last character of the line  
  > `G` bottom of the file  
  > `gg` top of the file  
  > line number + `G` go to the line
  > `j$` end of next line
- **Create new file**
  > `vim FILENAME` to edit or create a file  
  > `:w` to set a name for your current document, useful if you open and edit a document just by typing `vim <ENTER>` > `:edit FILENAME` to open a new file
- **Exit vim**
  > `:q!` to quit without saving the file.  
  > `:wq` to save and quit  
  > `:w` to save current file
- **Edit, Insert or Append**
  > `i` before the cursor  
  > `a` after the cursor  
  > `A` end of line  
  > `o` below current line  
  > `O` above current line  
  > `R` replace mode from cursor location  
  > `r` to replace current character  
  > `ce` to delete until end of word  
  > `c$` to delete until end of word
- **Delete**
  > `x` a charactere  
  > `dw` a word  
  > `d$` from cursor to end of line  
  > `dd` whole line
- **Undo**
  > `u` previous action  
  >  `U` all changes of a line  
  >  `CTRL-R` undo the undo's
- **Copy/Cut/Paste**
  > `dd` cut the whole line  
  > `p` paste  
  > `v` and move the cursor to select text  
  > `y` to copy highlighted text
  > `:w FILENAME` to save your selection in a new file  
  > `:r FILENAME` to paste the content of a file in your current cursor location, you can also paste the content of a command like `:r !ls`
- **Search**
  > `/` and text you want to look for  
  > `:set ic` to ignore case, `set noic` to disable ignore case
  > `:set hls` to highlight matching text, `:set nohls` do disable highlight  
  > `n` to search second occurence of previous search  
  > `N` to search previous occurence of previous search  
  > `?` to search in backward direction  
  > `CTRL-O` go back to your previous position  
  > `CTRL-I` goes forward  
  > Place cursor on any of these **(**, **[**, or **{** and type `%` to move to its matching closer or opener
- **Substitute**
  > `:s/old/new` one occurence in current line  
  > `:s/old/new/g` all occurence in current line  
  > `:%s/old/new/g` all occurrence in whole file  
  > add `c` at the end to prompt for each occurence  
  > example:
  > `:%s/old/new/gc`
- **External command**
  > `:!` and your command, examples: `:!dir` or `:!ls`
- **Help**
  > `:help` > `:help e` to jump to e command description  
  > `:q` to quit the help  
  > `:` + CTRL-D to see available commands
