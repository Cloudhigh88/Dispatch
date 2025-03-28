# Command Completions in Warp

## Overview
Warp's Command Completions feature enhances the user experience by providing suggestions for commands, option names, and path parameters. This functionality helps users quickly find and execute commands without needing to remember exact syntax.

## Features of Command Completions

### 1. Command Suggestions
- Completions will suggest commands based on the context of what the user is typing.
- This feature helps users discover available commands and their options without needing to consult documentation.

### 2. Option Name Suggestions
- As users type, Warp will suggest option names for commands, making it easier to understand the available flags and parameters.

### 3. Path Parameter Suggestions
- When applicable, Warp will suggest path parameters, helping users navigate file systems and directories more efficiently.

### 4. Autosuggestions
- Autosuggestions automatically suggest commands as users type, based on shell history and possible completions.
- This feature allows users to quickly access previously used commands, reducing the need for repetitive typing.

### 5. Fuzzy Search Capability
- The Completions feature includes fuzzy search capability, providing approximate matches for user queries.
- If users are unsure about the exact syntax or spelling, suggestions will be provided based on their input, even if it's not an exact match.

## How to Access Command Completions
- Type out the beginning of your command, then press **TAB**.
- To search for options and flags, type and press **TAB**.
- Alternatively, enable "Open completions menu as you type" in **Settings > Features**.

## How to Use Command Completions
- For example, type `git checkout` (note the space) and then press **TAB**. A menu will show all of your local branches, which can be selected using the mouse or the UP ↑/DOWN ↓ arrow keys.

### Completions on Aliases
- **Shell Aliases**: If you have an alias (e.g., `gc=git checkout`), typing `gc` and hitting **TAB** will provide the same completion options as for `git checkout`.
- **Command Aliases**: For subcommands (e.g., setting `git status` to `git st`), completions will suggest options for `git status` even if you typed `git st`.

## Terminal Tip
- The "Tab key behavior" setting under **Features > Editor** can change the action that **TAB** is bound to. If **TAB** is not bound to open the completions menu, **CTRL-SPACE** will be assigned as the default keybinding. You can also enable the "Open completions menu as you type" in **Settings > Features** to have the completions menu open automatically.

This guide will assist users in understanding and utilizing Command Completions effectively within the Warp terminal.
