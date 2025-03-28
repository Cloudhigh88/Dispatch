# Notifications & Audible Bell in Warp

## Overview
Warp can send customizable desktop notifications when you are away from the app, allowing you to quickly refocus when something meaningful happens in your terminal sessions. Additionally, Warp supports an audible terminal bell that can be triggered by various CLI tools.

## Features of Notifications

### What is it?
- Notifications can be sent when a command completes after a configurable number of seconds or when a running command requires you to enter a password to proceed.
- Warp will only send a desktop notification if you are using a different app at the time the trigger occurs.

### How to Access Notifications
- Notifications are enabled by default and require system permissions to appear.
- If you've previously turned Notifications off, toggle it back on by going to **Settings > Features > Session**, or quickly toggle Notifications with the Command Palette.
- On macOS, you will need to allow or accept the request for Warp to send you desktop notifications. If you accidentally denied it, refer to the troubleshooting guide below.

### Customizing Notification Triggers
- Customize Notification triggers for long-running commands or password prompts by going to **Settings > Features**.

## Features of Audible Bell

### What is it?
- Warp allows you to enable an audible terminal bell (disabled by default) that can be triggered by various CLI tools (e.g., `ping -a`).

### How to Access Audible Bell
- In **Settings**, enable an Audible terminal bell by navigating to **Settings > Features > Terminal**.
- You can also enable or disable the Audible Terminal Bell from the Command Palette by searching for **"Enable/Disable Audible Terminal Bell."**

## Troubleshooting Notifications
- Warp requires two distinct notification settings to work: 
  1. Linux system settings found in **Settings > Notifications > Warp**.
  2. Warp app settings found in **Settings > Features > Session**.
  
- If you have Notifications enabled in both the system and Warp but still aren't receiving desktop notifications, try the following:
  - Ensure you are navigated away from Warp when you expect to receive the notification.
  - Make sure the Do Not Disturb mode (if your distribution supports it) is turned off.
  - Go to **Settings > Notifications** and select Warp in the list. Ensure notifications are turned on, then quit and restart Warp.

This guide will assist users in understanding and utilizing the Notifications and Audible Bell features effectively within the Warp terminal.
