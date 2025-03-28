# Input Position Configuration for Warp Terminal

## Overview
Warp allows you to configure the position of your input, which includes both the prompt and the command line. You can select from three different input positions, each with distinct behaviors for the flow of input/output blocks.

## Input Position Options

### 1. Start at the Top (Classic Mode)
- **Behavior**: The prompt with input initiates at the top of the view and moves down as you enter commands. 
- **Input/Output Flow**: Blocks of input/output stack above the prompt and command input.
- **Navigation**: You can scroll up or navigate up to visit past commands. Use `CTRL-L` or the `clear` command to return the input to the top of the screen while maintaining your scroll history.

### 2. Pin to the Top (Reverse Mode)
- **Behavior**: The prompt with input is pinned to the top of your terminal view.
- **Input/Output Flow**: Blocks of grouped input/output flow down the view in reverse order, with the latest results at the top.
- **Navigation**: You can scroll down or navigate down to visit past commands. For long-running commands, click "Lock scrolling at bottom of block" to continue following the stdout.

### 3. Pin to the Bottom (Warp Mode)
- **Behavior**: Input is pinned to the bottom of your terminal view.
- **Input/Output Flow**: Blocks of grouped input/output flow up and out of view.
- **Navigation**: You can scroll up or navigate up to visit past commands.

## Accessing Input Position Configuration
To configure your input position:
1. Navigate to **Settings > Appearance > Input**.
2. You can also choose and set modes from the Command Palette.

Changes to the input position take effect immediately and apply to all open panes, allowing for a seamless user experience.
