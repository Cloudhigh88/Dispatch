# Background Blocks in Warp

## Overview
Background Blocks in Warp handle output from background processes that continue running even after the initial command exits. This feature allows users to manage and interact with background output using the same functionalities as regular blocks.

## What are Background Blocks?
- Commands can start background processes that continue running after they exit, often initiated by appending `&` to the command.
- If Warp receives output that is likely from a background process, it goes into a Background Block. These blocks act like regular blocks but do not have an associated command.

## How to Use Background Blocks
- Background Blocks are automatically created as needed, interleaved with regular blocks running commands.
- If you run commands while a background process is still producing output, that output gets split into multiple blocks.

## Troubleshooting Background Blocks
There are some limitations to be aware of:
- If a background process writes output while a foreground command is running in a regular block, the output goes into that block.
- If multiple background processes are running simultaneously, their output may be mixed together.
- If you start entering a command while another one is running (typeahead), Warp may mistake the partial command for background output. This is more common with older versions of bash (older than 4.0) when editing typeahead.

This guide will assist users in understanding and utilizing Background Blocks effectively within the Warp terminal.
