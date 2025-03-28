# Known Issues in Warp

## Overview
This document outlines known issues in Warp along with workarounds and solutions to help users navigate potential challenges while using the terminal.

## General Issues
- **SSH Wrapper**: When you SSH, Warp starts a bash shell on the remote host. This wrapper is necessary to enable Warp features.
- **Default Shell Aliases**: If your default shell is zsh, your aliases typically do not transfer over. Other shells are unsupported for now.
- **Non-shell-based Subshells**: When opening a non-shell-based subshell (REPL), it operates like a normal terminal session without Warp features.
- **Unresponsive Warp**: Warp may become unresponsive if it doesn't have permission to access certain folders.
- **No Touch Input Support**: Touch input is currently not supported.

## SSH Issues
- **Blocks over SSH**: To enable Blocks over SSH, Warp uses an SSH Wrapper function. Navigate to **Settings > Features** if you need to disable it. Refer to the Troubleshooting Legacy SSH for more info on workarounds.

## Online Features
- **Stale Login Token**: Online features (Warp AI, Generate, Block Sharing, Refer a Friend) may break due to a stale login token, typically caused by a password change. To resolve this:
  1. Remove Warp user login with your keychain manager (gnome-keyring, kwallet, etc.) by searching for `dev.warp.Warp` and deleting the User password/secret.
  2. Remove any user files with the command:
     ```
     rm -f ${XDG_STATE_HOME:-$HOME/.local/state}/warp-terminal/*-User
     ```
  3. Log in to Warp again.

## Language Support
- **English-only UI**: As of November 2021, character support for Chinese, Korean, and Japanese has been added, but the UI currently only supports English.
- **Abnormal Rendering of Chinese Characters**: If you notice issues with rendering Chinese characters, try adding the following lines to your rc file:
  ```
  export LC_ALL=zh_CN.UTF-8
  export LANG=zh_CN.UTF-8
  ```

## Shell Issues
- **Fish Shell Read Command**: There is an issue in fish shell version 3.6 and below that causes the `read` built-in command to break Warp's integration. Upgrade fish to the latest version to resolve this issue.

## Configuring and Debugging RC Files
- To support Blocks and a native Input Editor experience, custom support for a subset of shell functionality is required. You can disable conflicting settings for Warp using the following flag:
  ```
  $TERM_PROGRAM != "WarpTerminal"
  ```

### Example for Bash and Zsh
```bash
if [[ $TERM_PROGRAM != "WarpTerminal" ]]; then
    # Unsupported plugin/prompt code here
    test -e "${HOME}/.iterm2_shell_integration.zsh" && source "${HOME}/.iterm2_shell_integration.zsh" || true
fi
```

### Example for Fish
```fish
if test "$TERM_PROGRAM" != "WarpTerminal"
    # Unsupported plugin/prompt code here
    test -e {$HOME}/.iterm2_shell_integration.fish; and source {$HOME}/.iterm2_shell_integration.fish
end
```

## List of Incompatible Tools
Due to the Input Editor wrapping around the shell, the following tools may cause conflicts:
- oh-my-fish, oh-my-bash, or other unsupported shell prompts.
- iterm shell integration.
- Various plugins and completion tools (e.g., zsh-autosuggestions, FZF, etc.).

## macOS Issues
- **SSH Denied on Local Network**: On macOS, you may be denied permission to SSH from Warp into other devices. To resolve this, go to **System Settings > Privacy & Security > Local Network** and add Warp.
- **Unexpected Loss of Permission**: If you encounter an "Operation not permitted" error, apply any pending updates to ensure the new Warp binary has the correct permissions.
- **Auto-Update Error**: If Warp fails to open after an auto-update on macOS Ventura, follow the provided steps to resolve the issue.

## Windows Issues
- **Unsupported Features**: Certain features are not supported in Warp on Windows. Please track the relevant GitHub issues for updates.
- **Crash on Opening Launch Configuration**: Known limitations with graphics drivers may cause crashes. Workarounds are provided for users experiencing this issue.

## Linux Issues
- **Warp Won't Run or Render**: Known issues may prevent Warp from running or rendering on Linux. Workarounds are provided for users experiencing this issue.

This guide will assist users in understanding known issues in Warp and how to address them effectively.
