# Generate Feature in Warp

## Overview
The Generate feature in Warp allows users to turn natural language queries into precise commands, enhancing productivity and streamlining command execution. It is accessible directly from the command line input or within interactive command-line programs.

## Features of Generate

### 1. Generating Commands as Terminal Input
- **How to Use**: Type `#` on the command line input to open the suggestions interface.
- **Steps**:
  1. Press CTRL-` or type `#` in the text input editor to initiate a search using natural language.
  2. Enter your desired action, such as "replace a string in a file."
  3. Results are generated in real-time, allowing you to modify the prompt as needed.
  4. Once you find the command you want, you can execute it or save it as a Workflow in Warp Drive for future use.

### 2. Generating Text and Contextual Suggestions in Interactive CLIs
- **How to Use**: In interactive CLI applications, press CMD-I when you see the hint text appear.
- **Steps**:
  1. Type your desired command, such as "show me all tables in my Postgres database."
  2. Results are generated in real-time using the selected LLM.
  3. To refine or follow up on your query, press CMD-Y. You can edit your last message or add a follow-up.
  4. Press Enter or click the Accept button to execute the generated command.

### 3. Supported Interactive CLI Applications
- **Examples**:
  - **Database REPL**: Generate SQL queries like "create a table to store user data."
  - **Text Editors**: Quickly generate text such as markdown headers or boilerplate code.
  - **Python REPL**: Generate Python snippets like "create a simple plot of x."
  - **Debugger Tools**: Get commands for setting breakpoints or inspecting memory.
  - **Version Control**: Speed up complex git commands by describing your goal.
  - **Cloud Provider Shells**: Manage resources with commands like "create a new Kubernetes cluster."

## Requirements
- Currently, you need to be online to use the Generate feature. If it doesn't work, check if your ISP or firewall is blocking calls to app.warp.dev.

## Supported LLMs
The following LLMs are currently supported in Warp for the Generate feature:
- **OpenAI**: GPT-4o, o3-mini
- **Claude**: 3.7 Sonnet, 3.5 Sonnet, 3.5 Haiku
- **Google**: Gemini 2.0 Flash
- **DeepSeek**: R1, V3 (hosted by Fireworks AI in the US)

This guide will assist users in understanding and utilizing the Generate feature effectively within the Warp terminal.
