# Warpify in Warp

## Overview
Warpify enables Warp's features in local and remote sessions, enhancing the terminal experience by allowing users to utilize advanced functionalities in various shell environments.

## Features of Warpify

### 1. Subshells
- Warp supports enabling features in subshells for bash, zsh, and fish.
- **What is a Subshell?**: A subshell is defined as any nested interactive shell session running within the context of an existing shell. This includes local nested sessions, Docker container shells, or remote servers accessed through SSH.

#### How to Warpify the Subshell
- Warp automatically recognizes the following commands as subshell-compatible:
  - `bash`, `fish`, `zsh`
  - `docker exec`
  - `gcloud compute ssh`
  - `eb ssh`
  - `poetry shell`
- When running a subshell-compatible command, Warp will prompt you to "Warpify" the subshell, making all modern IDE features available.

### 2. SSH Support
- Warp provides a wrapper that enables Warp features in remote (SSH) sessions.
- This implementation allows users to access all Warp features without additional configuration.

#### Limitations of SSH
- The SSH Wrapper only supports bash or zsh shells in remote sessions.
- If using a different shell, you should use the command `ssh` directly.
- For zsh, `xxd` is required to bootstrap Warp.
- On Windows, Cygwin is required to bootstrap the SSH Wrapper.
- RemoteCommand may cause the SSH wrapper to fail, and Tmux is not currently supported.

### 3. Accessing Warpify
- Warp takes over the prompt, enabling a modern input editor.
- Warp configures histcontrol to ignore commands with leading spaces to prevent clutter in history.

## Troubleshooting SSH
- If you encounter issues with the SSH wrapper, ensure that your server configuration allows Warp's ControlMaster connection to work. Check the `MaxSessions` setting in `/etc/ssh/sshd_config` and ensure it is set to at least 2.

## Conclusion
This guide will assist users in understanding and utilizing Warpify features effectively within the Warp terminal, enhancing their workflow in both local and remote environments.
