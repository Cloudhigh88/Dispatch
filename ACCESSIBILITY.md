# Accessibility in Warp

## Overview
Warp's mission is to make the terminal accessible for all developers, including those who are visually impaired. This document summarizes the current accessibility features, how Warp works with VoiceOver, and outlines the main changes from the typical workflow.

## Features of Accessibility

### 1. VoiceOver Support
- Warp is designed to work seamlessly with VoiceOver on macOS, announcing actions and events happening on the screen.
- To install Warp using Homebrew, run:
  ```bash
  brew install warp
  ```
- After installation, Warp will prompt you to log in and send telemetry to improve user experience.

### 2. Using Warp with VoiceOver
- Warp announces actions and possible commands, providing a different experience compared to other applications.
- The main terminal window includes a Command Input area and a list of previously executed commands and their outputs, grouped into Blocks.

### 3. Differences from Regular VoiceOver Workflow
- Typical VoiceOver navigation keys do not currently work in Warp due to the UI framework's implementation.
- Warp announces actions and events, allowing users to understand what is happening without traditional navigation.

### 4. A11y Specific Actions
- Accessibility settings are available through the Command Palette. Type "a11y" to discover related options and their keybindings.
- Users can adjust the verbosity level of messages for better accessibility.

### 5. Voice Input
- Warp supports voice input as an alternative way to interact with the terminal, allowing users to:
  - Issue terminal commands
  - Ask questions about command usage
  - Perform complex multi-step operations
- Voice input can be enabled in **Settings > AI > Voice**.

## Future Work
- Warp is committed to improving accessibility and plans to add support for keyboard navigation of UI elements.
- Feedback from users is encouraged to enhance the accessibility experience.

This guide will assist users in understanding and utilizing accessibility features effectively within the Warp terminal.
