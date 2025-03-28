# Settings Sync in Warp

## Overview
Settings Sync is a cloud feature in Warp that allows users to conveniently use Warp on multiple devices or on a single device using both the Desktop and Web versions of Warp. This feature is currently in experimental (Beta) status.

## What is Settings Sync?
- Settings Sync sends your settings information to Warp’s servers, enabling a consistent experience across devices.
- Starting January 9, 2025, Settings Sync will be gradually enabled for a percentage of Warp users. New users included in this rollout will have Settings Sync on by default, while existing users will need to opt-in.

## How to Toggle Settings Sync
- You can toggle Settings Sync within the **Settings > Account** pane.
- Alternatively, you can use the Command Palette by searching for **“Settings Sync.”**

### Settings Sync in Account Pane
- Access the Settings Sync option directly from the Account settings.

### Settings Sync in Command Palette
- Quickly toggle Settings Sync using the Command Palette.

## How Settings Sync Works
- Settings Sync syncs the state of most Warp settings to the cloud.
- When you log in to Warp on another device or through the browser with Settings Sync enabled, most of your settings will be the same as they were previously.
- This includes themes, most features, privacy settings, and AI settings, saving you time from having to set them up again.

### Default Settings
- When you first enable Settings Sync, the settings from the computer you enabled it on become the default settings for all devices.
- If you toggle Settings Sync off and on, the synced settings will always reflect the last device you enabled it on.

## Non-synced Settings
Not all settings are synced. Notably, Warp does not sync:
- Custom keybindings (this may change in the future).
- Custom themes (this may change in the future).
- Device-specific settings (e.g., preferred editor, startup shell).
- Platform-specific settings are synced across devices on the same platform (e.g., Linux clipboard settings are synced across all Linux devices but not on Mac, Windows, or Web).

### Identifying Non-synced Settings
- You can identify non-synced settings by the special cloud strikethrough icon in the settings panel.

This guide will assist users in understanding and utilizing the Settings Sync feature effectively within the Warp terminal.
