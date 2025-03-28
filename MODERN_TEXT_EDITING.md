# Modern Text Editing in Warp

## Overview
Warp’s input editor operates like a modern IDE, providing a user-friendly text editing experience that enhances productivity. This includes features such as soft wrapping, copy on select, autocomplete for quotes and brackets, alias expansion, syntax highlighting, and error highlighting.

## Features of Modern Text Editing

### 1. Soft Wrapping
- Warp supports soft wrapping in the input editor. If an autosuggestion goes off-screen, the input editor will be horizontally scrollable to make it visible.
- Some operations treat soft-wrapped lines as logical lines (e.g., TRIPLE-CLICK), while others treat them as separate visible lines (e.g., UP/DOWN, SHIFT-UP/SHIFT-DOWN).

### 2. Copy on Select
- Warp supports copy on select for selectable text within Blocks.
- Toggle this feature in **Settings > Features > General** or search for "Copy on select" in the Command Palette.

### 3. Autocomplete Quotes, Parentheses, and Brackets
- Warp can automatically complete quotes, brackets, and parentheses.
- Toggle this feature in **Settings > Features > Editor** or search for "Autocomplete quotes" in the Command Palette.

### 4. Keyboard Shortcuts
Here are some useful keyboard shortcuts for text editing:
- **ESCAPE**: Closes the input suggestions or history menu.
- **CTRL-L**: Clears the terminal.
- **CTRL-H**: Backspace.
- **CTRL-C**: Clear the entire editor buffer.
- **CTRL-U**: Copy and clear the current line.
- **CTRL-SHIFT-K**: Clear selected lines.
- **CTRL-C, CTRL-X, CTRL-V**: Copy, cut, paste.
- **CTRL-W / ALT-D**: Cut the word to the left/right of the cursor.
- **ALT-BACKSPACE / ALT-D**: Delete the word to the left/right of the cursor.
- **CTRL-K**: Delete everything to the right of the cursor.
- **ALT-LEFT / ALT-RIGHT**: Move to the beginning of the previous/next word.
- **CTRL-LEFT / CTRL-RIGHT**: Move backward/forward by one subword.
- **CTRL-A / CTRL-E**: Move the cursor to the start/end of the line.
- **SHIFT-UP / SHIFT-DOWN**: Select everything above/below the cursor.
- **CTRL-A**: Select the entire editor buffer.
- **SHIFT-ENTER / CTRL-ENTER / ALT-ENTER**: Insert newline.
- **CTRL-R**: Command Search.
- **CTRL-SHIFT-D**: Split pane.

### 5. Alias Expansion
- Warp automatically expands your aliases as you type in the input editor.
- To enable or disable alias expansion, navigate to **Settings > Features > Editor** and toggle **“Expand aliases as you type.”**

### 6. Syntax Highlighting
- Warp supports syntax highlighting in the input editor, coloring each part of a command to help differentiate between sub-commands, options/flags, arguments, and variables.
- Syntax highlighting is enabled by default. To toggle it, search for the "Syntax Highlighting" option in the Command Palette or navigate to **Settings > Features > Editor**.

### 7. Error Highlighting
- Warp highlights errors in commands typed within the input editor, underlining invalid commands with a dashed red underline.

This guide will assist users in understanding and utilizing Modern Text Editing features effectively within the Warp terminal.
