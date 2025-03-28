# Agent Mode in Warp

## Overview
Agent Mode is a powerful feature in Warp that allows users to perform terminal tasks using natural language. It interprets user input and executes highly accurate commands tailored to the user's environment.

## Features of Agent Mode

### 1. Natural Language Understanding
- Agent Mode can understand plain English, allowing users to type tasks or questions directly into the terminal.

### 2. Command Execution
- Executes commands and uses the output to guide users, correcting itself when it encounters mistakes.

### 3. Integration with Services
- Learns and integrates with any service that has public documentation or `--help`.

### 4. Workflow Utilization
- Utilizes saved workflows to answer queries.

### 5. Entering Agent Mode
Users can enter Agent Mode in several ways:
- Type any natural language task or question in the terminal input.
- Use keyboard shortcuts: CMD-I (Mac) or type ASTERISK-SPACE.
- Click the “AI” sparkles icon in the menu bar to open a new terminal pane in Agent Mode.
- From a block, click the sparkles icon in the toolbelt or the block context menu item “Attach block(s) to AI query.”

### 6. Exiting Agent Mode
- Exit Agent Mode at any point using ESC or CTRL-C, or toggle out with CMD-I.

### 7. Command Suggestions
- If Agent Mode finds a suitable command, it will describe it in an AI block and fill the terminal input with the suggested command for execution.

### 8. Context Management
- Users can attach context from previous blocks to their queries, enhancing the accuracy of responses.

### 9. Auto-detection
- The feature for detecting natural language is local, and no input is sent to AI until ENTER is pressed in Agent Mode. Users can manage auto-detection settings in **Settings > AI**.

### 10. Input Hints
- Input hints are shown in light grey text to help users learn about features. This can be toggled in **Settings > AI**.

### 11. Coding Capabilities
- Agent Mode includes advanced coding capabilities, allowing for seamless code generation and editing tasks directly within the terminal.

### 12. Dispatch
- A form of Agent Mode that automates complex tasks by gathering context and executing commands based on user input.

## Managing Permissions and Settings
- Users can manage permissions for commands and configure settings for Agent Mode in **Settings > AI**.

## Known Issues and Limitations
- Agent Mode blocks are not shareable during session sharing.
- Long conversations may lead to context loss due to token limits.

This guide will assist users in understanding and utilizing Agent Mode effectively within the Warp terminal.
