# Session Management in Warp

## Overview
Warp's Session Management features enhance the user experience by providing tools to manage sessions effectively. This includes saving configurations, navigating between sessions, and restoring previous sessions.

## Features of Session Management

### 1. Launch Configurations
- Launch Configurations enables you to save your configuration of windows, tabs, and panes, so that you can reopen the same set of sessions per project quickly.

#### What is it?
- With Launch Configurations, you can save in the app or by adding a YAML file.
- Launch Configurations files are generated when you create them with the UI and can also be created or modified manually.

#### Creating a Launch Configuration
- **From the UI:**

**From the UI:**
1. Set up the configuration of windows, tabs, and panes you would like to save.
2. Open the Command Palette and type in **Save New Launch Configuration**.
3. Name the configuration file (the name field cannot be empty).
4. Click the **Save configuration** button.

- **With a YAML File:**

#### Using a Launch Configuration
- From the Command Palette, enter **Launch Configuration** to open and select a Launch Configuration.
- Right-click the new Tab + button to open a menu and select saved Launch Configuration.
- Single-window launch configs can be launched into the active window from the launch configuration palette using **CTRL-ENTER** on Linux.

### 2. Session Navigation
- The Session Navigation Palette helps you speed up your workflow by allowing you to quickly navigate using the keyboard or mouse to the terminal sessions you are looking for across Warp.
- Enables users to easily navigate to any session in Warp.

### 3. Session Restoration
- The Session Restoration feature enables Warp to restore your session history, specifically windows, tabs, and panes, along with the last few Blocks in each pane.
- This feature allows you to quickly pick up where you left off in your previous terminal session.

#### How to access Session Restoration
- Session Restoration comes enabled by default in Warp.
- On Linux, opening windows at a specific position is not supported in Wayland.
- You can disable Session Restoration by going to **Settings > Features**, then toggling off **Restore windows, tabs, and panes on startup**.
- Toggling off Session Restoration will not clear the SQLite database; however, Warp will stop recording new output.

#### How to access Session Navigation
- Open the Session Navigation palette with the Command Palette, click on session >_ or type in "sessions:".
- Jump to a session by using your mouse or the UP ↑/DOWN ↓ arrow keys and ENTER.
- Refine the session results by searching for sessions by prompt, the currently running command, last run command, and command status (ex: “Running…”, “Completed 10 minutes ago”, “Empty Session”).
- Sessions are ordered by recency, so the most recently focused sessions show up first. The Session Navigation palette does not have PS1 support and can only show Warp's native prompt.

## Terminal Tip
- You can open saved Launch Configurations via Alfred Workflow or Raycast Extension. Learn more here. Credit to @joetannenbaum.

This guide will assist users in understanding and utilizing Session Management features effectively within the Warp terminal.
