# Markdown Viewer in Warp

## Overview
Warp allows users to open Markdown files directly in the terminal, providing a built-in viewer in addition to the option to open files in external editors. This feature enhances the user experience by enabling seamless interaction with Markdown content.

## Features of Markdown Viewer

### Opening Markdown Files
- Warp treats any local file with the `.md` or `.markdown` extension as a Markdown file. Remote files are currently not supported.
- You can configure Warp to open Markdown files with either the default external editor or Warp's built-in Markdown viewer in **Settings > Features > General > Open Markdown files in Warp's Markdown viewer by default**.

### Accessing Markdown Files
- To open a Markdown file link within a block, hold **CTRL** and click the link, or use the link tooltip or right-click context menu.
- You can also open a Markdown file from Finder by right-clicking the file and selecting "Open With" to choose Warp.

### Markdown-Viewing Commands
- Running a Markdown-viewing command like `cat myfile.md` will prompt Warp to show a banner with a button to open the Markdown file.
- The following commands are considered Markdown viewers:
  - `cat`
  - `glow`
  - `less`

### Running Shell Commands from Markdown
- Warp can execute shell commands from Markdown code blocks in your active terminal session.
- To run a command, the shell command must be enclosed in a code block with three backticks (```), not inline code.
- Click the run icon >_ to insert a command into the terminal input.

### Navigating Shell Blocks
- You can enter keyboard navigation mode by clicking on a shell block or pressing **CTRL-UP** or **CTRL-DOWN**.
- Once a shell block is selected, press **CTRL-ENTER** to insert it into the terminal input.
- You can navigate between shell blocks using UP, DOWN, **CTRL-UP**, and **CTRL-DOWN**.
- While focused on the Markdown file, press **CTRL-SHIFT-L** to switch focus back to the terminal without inserting a command.

### Copying Code Blocks
- All shell and code blocks have a copy button to quickly copy the block’s text to the clipboard.

### Supported Code Block Languages
- Code blocks without a set language, or with the following languages, are treated as shell commands:
  - `sh`, `shell`, `bash`, `fish`, `zsh`, `warp-runnable-command`

This guide will assist users in understanding and utilizing the Markdown Viewer features effectively within the Warp terminal.
