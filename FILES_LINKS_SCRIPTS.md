# Files, Links, & Scripts in Warp

## Overview
Warp allows users to quickly open files, folders, and URL links, as well as run scripts directly from the terminal. This feature enhances productivity by enabling seamless interaction with various resources.

## Features of Files & Links

### Opening Files and Links
- Warp supports opening files, folders, and URL links contained within Blocks.
- Multiple URL protocols are supported, including:
  - `https`
  - `ftp`
  - `file`
- Warp can open files and folders in various editors and opens web links directly in your default browser.
- Markdown files can be opened directly with a Markdown Viewer.

### Supported File Path Formats
Warp parses both relative and absolute file paths and captures line and column numbers in the following formats:
- `file_name:line_num`
- `file_name:line_num:column_num`
- `file_name[line_num, column_num]`
- `file_name(line_num, column_num)`
- `file_name, line: line_num, column: column_num`
- `file_name, line: line_num, in`

### Interacting with Links
- Hold down **CTRL** while clicking a link to open it directly.
- Clicking a link normally will show a tooltip that says “Open File/Folder/Link”.
- Right-clicking a link opens a context menu for copying the absolute file path or URL to the clipboard.
- Drag and drop a folder or file onto the Warp dock icon to open a new tab in that directory.
- Right-click on a folder or file in Finder, select Services, and choose "Open new Warp Tab | Window here".

### Configuring Default Editors
- Configure the default editor for opening files by navigating to **Settings > Features > Choose an editor to open file links**.
- Selecting "Default App" uses your system's default application for the file type.

### Supported Editors
Warp supports a variety of GUI-based editors, including:
- Visual Studio Code
- JetBrains IDEs (e.g., WebStorm, PhpStorm, GoLand, PyCharm, DataGrip, DataSpell, Rider, RubyMine)
- Zed
- Cursor
- Windsurf
- Sublime Text
- Android Studio

*Note: Warp currently does not support terminal-based editors like vim, nano, or helix. To use a terminal-based editor, type `$EDITOR <path/to/file>`.*

## Scripts
- Warp can open `.command` and Unix Executable files directly from Finder.
- To open a script, find the `.command` or shell script in Finder, right-click, and select "Open with Warp".

This guide will assist users in understanding and utilizing the Files, Links, and Scripts features effectively within the Warp terminal.
