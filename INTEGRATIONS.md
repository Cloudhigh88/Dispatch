# Integrations in Warp

## Overview
Warp extends and integrates with popular development tools, enhancing the user experience and streamlining workflows. This document outlines the available integrations and how to utilize them effectively.

## 1. Docker Integration
- **Availability**: Currently only available on macOS.
- **Functionality**: The Docker extension allows users to open Docker containers in Warp easily. You can click to open any Docker container in a Warpified subshell without manually running `docker exec` or typing lengthy container IDs.
- **How to Use**:
  - Select a container from the list.
  - Specify a shell type (only `bash`, `zsh`, or `fish` are supported).
  - Optionally select a user.
  - Click “Open in Warp” to run commands within the Docker container.

## 2. Raycast Integration
- **Availability**: Currently only available on macOS.
- **Functionality**: The Warp + Raycast extension helps you open new windows, tabs, or Launch Configurations with ease.
- **How to Use**:
  - In Raycast, go to **Settings > Extensions > Apps**.
  - Search for Warp and assign the alias "terminal" so that it will show up in searches.

## 3. VSCode Integration
- **Functionality**: Press **CTRL-SHIFT-C** while in VSCode to open a new session in Warp.
- **How to Configure**:
  - Navigate to **Settings** in VSCode and search for **Terminal › External: Linux Exec**.
  - Change this to `warp-terminal` if you've installed Warp with your distribution's package manager. Otherwise, provide the full path to the executable (e.g., if it is an AppImage).

## 4. JetBrains IDEs Integration
- **Availability**: Currently only available on macOS.
- **Functionality**: Press a keyboard shortcut of your choice while in a JetBrains IDE to open a new session in Warp.
- **How to Configure**:
  - Use the Apple Menu to click on **Preferences**.
  - Go to **External Tools** and click **Add**.
  - Fill in the following information:
    - **Name**: Open Warp
    - **Program**: `/Applications/Warp.app`
    - **Arguments**: `$ProjectFileDir$`
    - **Working Directory**: `/Applications`
  - Press **Ok**. You will now be able to open Warp from the Apple Menu under **Tools > External Tools**.

### Attaching a Keyboard Shortcut
- To attach this configuration to a keyboard shortcut:
  - Go to the Apple Menu -> **Preferences**.
  - Navigate to **Keymap > External Tools**.
  - Find **Open Warp**, right-click on it, and select **Add Keyboard Shortcut**. Type your desired shortcut and click save.

This guide will assist users in understanding and utilizing the integrations available in Warp effectively.
