# Network Log in Warp

## Overview
The Network Log feature in Warp logs all network traffic (both requests and responses) originating from the current terminal session. This feature is useful for debugging issues and understanding when information is sent or received over the network throughout a Warp terminal session.

## What is the Network Log?
- Each log item is a timestamped debug format string for either a request or response object handled by Warp.
- Messages are logged via pre-request and post-response hooks in Warp’s internal HTTP client.

## How to Use the Network Log
1. To access the network panel, open the Command Palette and type in **“Show Warp Network Log.”**
2. This will insert a workflow into your input editor, which should look something like this:
   ```
   tail -f "some/path/to/warp_network.log"
   ```
3. Press **Enter** to run this workflow.
4. Then, search for a generated command or share a Block to see the network log activity.
5. Once you run one of these examples, you’ll see the corresponding requests and responses logged in the network log.

## Known Issues with Network Log
- Currently, network traffic originating from crash reports and error messages is not captured in the network log due to the use of the Sentry SDK, which encapsulates all network logic and doesn’t expose a hook for handling requests and responses directly.
- The team is actively investigating a solution to include such traffic in the log in a future release.
- You may disable Crash Reporting entirely in Warp’s **Settings > Privacy** tab.

This guide will assist users in understanding and utilizing the Network Log feature effectively within the Warp terminal.
