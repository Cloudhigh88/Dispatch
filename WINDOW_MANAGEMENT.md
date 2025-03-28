# Window Management in Warp

## Overview
Warp's Window Management features enhance the user experience by providing tools for Window Management.

## Features of Window Management

### 1. Global Hotkey
- Warp's Global Hotkey is a configurable shortcut that can show/hide a dedicated Warp window or all Warp windows on your chosen desktop regardless of whether the app is focused.
- On macOS, system keyboard shortcuts like CMD-ESC, CMD-BACKTICK, CMD-TAB, CMD-PERIOD, and CMD-TILDE need to be unbound before you can use them in Warp.
- On Linux, the Global Hotkey may not work for some X11 window managers that do not implement Extended Window Manager Hints. Some examples include: sowm, catwm, Fvwm, dwm, 2bWM, monsterwm, TinyWM, x11fs, XMonad.

#### How to access it
**Dedicated Window**
- Dedicated Window allows you to customize the windows' pinned position and its width and height ratio relative to your active screen size (also known as Quake Mode).
- Open **Settings > Features > Keys** and select "Dedicated hotkey window" from the Global Hotkey dropdown to enable the feature.
- Configure the keybinding, the windows position, screen, and relative size or uncheck "Autohides on the loss of keyboard focus" which will cause the dedicated Hotkey Window to stay on top when triggered regardless of mouse or keyboard focus.
- On Linux and Windows, Warp does not support the "Autohides on the loss of keyboard focus" feature.

**Show/Hide All Windows**
- Show/Hide All Windows allows you to configure a shortcut to show/hide all Warp windows.
- Open **Settings > Features > Keys** and select "Show/hide all windows" from the Global Hotkey dropdown to enable the feature.
- Configure your preferred keybinding.
- On Linux, hidden windows may not appear in your ALT-TAB window switcher menu. Furthermore, the ordering of windows beyond the top window may change after toggling.

This guide will assist users in understanding and utilizing Window Management features effectively within the Warp terminal.
