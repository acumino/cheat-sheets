## Vim Commands Cheat Sheet

**Table of Contents:**
- [Vim Commands Cheat Sheet](#vim-commands-cheat-sheet)
  - [Modes](#modes)
  - [Navigation](#navigation)
  - [Editing](#editing)
  - [Visual Selection](#visual-selection)
  - [Saving and Quitting](#saving-and-quitting)
  - [Search and Replace](#search-and-replace)
  - [Windows and Tabs](#windows-and-tabs)
  - [Miscellaneous](#miscellaneous)

### Modes

- **Normal mode**: Default mode for navigation and executing commands.
- **Insert mode**: Mode for inserting text.
- **Visual mode**: Mode for selecting and manipulating text.
- **Command-line mode**: Mode for entering Vim commands.

### Navigation

- **h**: Move left.
- **j**: Move down.
- **k**: Move up.
- **l**: Move right.
- **w**: Move to the beginning of the next word.
- **b**: Move to the beginning of the previous word.
- **e**: Move to the end of the current word.
- **0**: Move to the beginning of the line.
- **$**: Move to the end of the line.
- **gg**: Move to the beginning of the file.
- **G**: Move to the end of the file.
- **Ctrl+f**: Move forward one page.
- **Ctrl+b**: Move backward one page.
- **Ctrl+d**: Move down half a page.
- **Ctrl+u**: Move up half a page.
- **Ctrl+e**: Scroll the window down one line.
- **Ctrl+y**: Scroll the window up one line.
- **:{line_number}**: Move to a specific line number.

### Editing

- **i**: Enter insert mode at the current cursor position.
- **I**: Enter insert mode at the beginning of the line.
- **a**: Enter insert mode after the current cursor position.
- **A**: Enter insert mode at the end of the line.
- **o**: Insert a new line below the current line and enter insert mode.
- **O**: Insert a new line above the current line and enter insert mode.
- **r**: Replace the character under the cursor.
- **R**: Enter replace mode, which overwrites existing text.
- **x**: Delete the character at the cursor position.
- **X**: Delete the character before the cursor position.
- **dd**: Delete the current line.
- **D**: Delete from the cursor position to the end of the line.
- **yy**: Copy the current line.
- **Y**: Copy from the cursor position to the end of the line.
- **p**: Paste the copied or deleted content after the cursor position.
- **P**: Paste the copied or deleted content before the cursor position.
- **u**: Undo the last change.
- **Ctrl+r**: Redo the last undone change.
- **J**: Join the current line with the line below.
- **.**: Repeat the last change.

### Visual Selection

- **v**: Enter visual mode to select characters.
- **V**: Enter visual mode to select whole lines.
- **Ctrl+v**: Enter visual block mode to select rectangular blocks.
- **o**: Move the cursor to the other end of the selection.
- **y**: Copy the selected text.
- **d**: Delete the selected text.
- **~**: Switch case of the selected text.
- **>`**: Indent the selected lines.
- **<`**: Unindent the selected lines.

### Saving and Quitting

- **:w**: Save the current file.
- **:wq**: Save the file and quit Vim.
- **:x**: Same as :wq (save and quit).
- **:q**: Quit Vim (if no changes were made).
- **:q!**: Quit Vim without saving changes.
- **:w {filename}**: Save the current buffer to a new file.

### Search and Replace

- **/{pattern}**: Search for a pattern forward.
- **?{pattern}**: Search for a pattern backward.
- **n**: Move to the next search result.
- **N**: Move to the previous search result.
- **:%s/{pattern}/{replacement}/g**: Search and replace globally in the file.
- **:%s/{pattern}/{replacement}/gc**: Search and replace globally in the file with confirmation.

### Windows and Tabs

- **:sp {filename}**: Split the window horizontally and open a file.
- **:vsp {filename}**: Split the window vertically and open a file.
- **Ctrl+w+w**: Cycle through open windows.
- **Ctrl+w+h**: Move to the window on the left.
- **Ctrl+w+j**: Move to the window below.
- **Ctrl+w+k**: Move to the window above.
- **Ctrl+w+l**: Move to the window on the right.
- **Ctrl+w+=**: Make all windows equal size.
- **:tabnew**: Open a new tab.
- **gt**: Move to the next tab.
- **gT**: Move to the previous tab.
- **:tabclose**: Close the current tab.

### Miscellaneous

- **:set number**: Show line numbers.
- **:set nonumber**: Hide line numbers.
- **:set list**: Show invisible characters.
- **:set nolist**: Hide invisible characters.
- **:set hlsearch**: Highlight search results.
- **:set nohlsearch**: Disable search result highlighting.
- **:set syntax=java**: Set syntax highlighting for Java (replace "java" with the appropriate language).
- **:set expandtab**: Use spaces instead of tabs for indentation.
- **:set tabstop=4**: Set the tab width to 4 spaces.
