# Voice Feature in Warp

## Overview
The Voice feature in Warp transforms how users interact with the terminal by allowing them to speak commands and queries directly. This feature is especially powerful when combined with Agent Mode for complex operations or longer scenarios.

## Getting Started with Voice

### Initial Setup
First-time users need to grant microphone permissions:
- **macOS**: Accept the system permission prompt or allow Warp microphone access in **System Settings > Privacy & Security > Microphone**.
- **Windows**: Allow Warp microphone access in **Settings > Privacy & Security > Microphone**.
- **Linux**: Configure through system sound settings.

### Activating Voice
There are two ways to activate the Voice feature:
1. **Microphone Button in Agent Mode**:
   - Click the microphone icon in Agent Mode.
   - Start speaking when the indicator shows it's listening.
   - Click again to stop recording.
   
2. **Hotkey Method**:
   - Press and hold the Fn key (configurable) to start recording.
   - Speak your command or query while holding the key.
   - Release the Fn key to stop recording and transcribe.

## Using Voice
Voice input allows for natural and efficient interactions with Agent Mode. Users can ask complex questions or describe multi-step tasks, such as:
- "Create a new Node.js project, install Express and MongoDB, then set up a basic server with a health check endpoint."
- "Find all log files in my project that contain errors from the last 24 hours, create a summary of the errors, and email it to me."

Voice input works across all of Warp's input interfaces, including the Find dialog and other input editors.

## Privacy & Security
- The transcription is powered by Wispr Flow. Voice data is processed in real-time and is not retained as a recording after transcription.

## Usage Limits
Voice features have anti-abuse limits to ensure fair usage. These limits may change as the service improves.

## Troubleshooting Common Issues
- **Microphone Not Detected**: Check system permissions and ensure the microphone is properly connected. Restart Warp if issues persist.
- **Poor Transcription Quality**: Minimize background noise, position yourself closer to the microphone, and speak clearly.
- **Feature Not Activating**: Confirm hotkey settings and check for conflicting keyboard shortcuts. Ensure you are running the latest version of Warp.

This guide will assist users in understanding and utilizing the Voice feature effectively within the Warp terminal.
