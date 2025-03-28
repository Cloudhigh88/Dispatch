# Wayland Support in Warp

## Overview
Warp's Wayland support can be enabled to improve the user experience, particularly for users with fractional scaling enabled in their window manager. This feature may help resolve issues with blurry text.

## Enabling Wayland Support
- To enable Wayland support, navigate to **Settings > Features > System**.
- Note that enabling Wayland support will disable Global Hotkey support, as the Wayland protocol does not expose the necessary configuration to support this feature.

## Wayland Crash Recovery
- When Wayland support is enabled, Warp uses a custom crash recovery process to detect any crashes that may occur while using Wayland.
- If a crash occurs, Warp will fall back to using X11, allowing you to continue using the application without interruption.

This guide will assist users in understanding and utilizing Wayland support features effectively within the Warp terminal.
