# Vim Keybindings in Warp

## Overview
Vim Keybindings (also known as Vim mode) allow users to edit commands in Warp's input editor using keyboard-driven text editing, similar to the Vi family of programs (including Vim and Neovim).

## Enabling Vim Keybindings
- Warp attempts to detect the shell's keybinding settings. If a shell vi mode is detected, Warp may suggest enabling Vim keybindings.
- To manually toggle Vim keybindings:
  - Through the Command Palette, search for **"Vim Keybindings."**
  - Through **Settings > Features > Editor**, toggle **"Edit commands with Vim keybindings."**

## Supported Keybindings
### Movement
- **h, j, k, l**: Single-char movement
- **<space>, <backspace>**: Single-char movement with line wrap
- **w, W, b, B, e, E**: Word movement
- **ge, gE**: End of previous word
- **$**: End of line
- **0**: Beginning of line
- **^**: First non-whitespace character of line
- **%**: Jump to matching bracket
- **[, ]**: Prev/next unmatched bracket
- **_**: Beginning of the current line
- **+**: First non-whitespace character of the next line
- **-**: First non-whitespace character of the previous line
- **gg, G**: Jump to first/last line

### Editing
- **r**: Replace character under cursor
- **d, D**: Delete a range or object
- **c, C**: Change a range or object (delete, then go to insert mode)
- **s, S**: Substitute (like change, but can only delete at the cursor)
- **x, X**: Delete under cursor
- **y, Y**: Yank (copy) into the clipboard
- **p, P**: Paste from the clipboard
- **u, ⌃r**: Undo, redo
- **~,**: Toggle upper/lowercase under cursor
- **gu**: Lowercase under cursor (u in visual mode)
- **gU**: Uppercase under cursor (U in visual mode)
- **J**: Join current and following lines
- **.**: Repeat last edit

### Text Objects
- **i**: Inner (exclude delimiters in text object)
- **a**: Around (include delimiters in text object)
- **w, W**: Whitespace-delimited string (word)
- **", ', ```**: Quote-delimited string
- **(, {, [**: Parenthesized/bracketed string

### Search
- **t, T, f, F**: Find next/prev matching character on line
- **;**: Repeat last character search in the same direction
- **,**: Repeat last character search in the opposite direction
- **/, ?, *, #**: Open Warp command search

### Mode Switching
- **i**: Insert text before the cursor
- **I**: Insert text before the first non-whitespace character in the line
- **a**: Append text after the cursor
- **A**: Append text at the end of the line
- **o**: Begin new line below the cursor and insert text
- **O**: Begin new line above the cursor and insert text
- **v**: Visual character mode
- **V**: Visual line mode

### Registers
- **"**: Register prefix
- **a–z, A–Z**: Named registers
- **+, ***: System clipboard
- **"**: Unnamed register, containing the text of the last delete or yank

This guide will assist users in understanding and utilizing Vim Keybindings effectively within the Warp terminal.
