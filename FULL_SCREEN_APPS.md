# Full-screen Apps in Warp

## Overview
Warp supports running alt-grid applications like Vim and Emacs in full-screen mode. This feature enhances the user experience by allowing seamless interaction with these applications while providing options for mouse and scroll event handling.

## Features of Full-screen Apps

### 1. Mouse and Scroll Reporting
- Warp allows configuring how to handle mouse and scroll events. These events can be sent to the currently running app (e.g., Vim) or handled by Warp.
- Mouse reporting must be enabled to toggle scroll reporting.
- Once mouse reporting is enabled, Warp uses ANSI escape sequences to communicate mouse events to the running app.
- To send a mouse event to Warp (for example, for text selection) without disabling mouse reporting, hold the **SHIFT** key.

#### How to Access Mouse Reporting
- From the Settings panel: **Settings > Features > Enable Mouse Reporting**.
- From the Command Palette, search for **"Toggle Mouse Reporting."**
- From the macOS Menu: **View > Toggle Mouse Reporting.**
- Use the keyboard shortcut: **CMD-R**.

### 2. Padding Configuration
- Warp supports configuring the amount of padding surrounding full-screen apps. The default is 0 pixel padding, but this can be changed to a custom padding amount or to match the padding in the Blocklist.
- Warp allows scaling the terminal by fractions of a cell width/height. When the terminal size is not perfectly aligned to a cell width/height, the extra space appears as padding on the right/bottom.

#### How to Access Padding Configuration
- Go to **Settings > Appearance > Full Screen Apps** or search for **"Appearance"** in the Command Palette.
- Use custom padding in alt-screen, which is enabled by default. You can disable it to match the Blocklist padding.
- Set the desired uniform padding (px), which is set to 0px by default.

### 3. Troubleshooting
- Some full-screen applications may not behave well when resizing. If you experience rendering issues with full-screen apps, try turning off the custom padding setting to ensure that full-screen apps don't need to resize when starting up.

This guide will assist users in understanding and utilizing Full-screen Apps features effectively within the Warp terminal.
