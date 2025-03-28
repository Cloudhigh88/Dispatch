# Block Basics in Warp

## Overview
Blocks in Warp group commands and their outputs into a single atomic unit, enhancing usability and organization within the terminal.

## The Basics of Blocks
- **Grouping**: Blocks group your command and command output.
- **Input Editor Positioning**: The Input Editor can pin to the bottom, pin to the top, or start at the top.
- **Growth Direction**: Blocks grow from the bottom to the top.
- **Color Coding**: Blocks that quit with a non-zero exit code have a red background and red sidebar.

### Try It Yourself!
- Type a command that doesn’t exist (e.g., `xyz`) and hit ENTER to see how Blocks behave.

## Creating a Block
1. Execute a command (e.g., type `ls` and hit ENTER) in the Input Editor at the bottom of the screen.
2. Your command and output will be grouped into a Block.
3. Try executing a different command (e.g., `echo hello` and hit ENTER) to create another Block.

## Selecting a Single Block
- **Using Your Mouse**: Click on a Block.
- **Using Your Keyboard**: 
  - Hit CMD-UP (or CMD-DOWN if input is pinned at the top) to select the most recently executed Block.
  - Use the UP ↑ and DOWN ↓ arrow keys to navigate to the desired Block.

### For Long Blocks:
- Click "Jump to the bottom of this block."
- Press SHIFT-CMD-UP/SHIFT-CMD-DOWN to scroll to the top/bottom of the selected Block.
- Use the Command Palette to "Scroll to the top/bottom of selected block."

## Selecting Multiple Blocks
- Click another Block while holding CMD to toggle the selection of that Block.
- Click another Block while holding SHIFT to select a range of Blocks.
- Use SHIFT-UP ↑ or SHIFT-DOWN ↓ to expand the active selection (the Block with the thicker border) up or down.

## Navigating Blocks
- Scroll using your mouse or the scrollbar, or select a Block and use the UP ↑ and DOWN ↓ arrow keys.
- Use "Scroll Terminal output up/down one line" to navigate block output, which can be configured with a keyboard shortcut or accessed from the Command Palette.
- When the output of a command is cut off, Warp keeps the Sticky Command Header pinned at the top, displaying the command the Block corresponds to. Clicking the header will scroll the screen to the start of the Block.

This guide will assist users in understanding and utilizing Blocks effectively within the Warp terminal.
