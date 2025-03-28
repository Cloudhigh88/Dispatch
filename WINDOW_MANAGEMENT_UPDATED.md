# Window Management in Warp

## Overview
Warp's Window Management features enhance the user experience by providing tools for Window Management.

## Features of Window Management in Warp

### 1. Global Hotkey
- Warp's Global Hotkey is a configurable shortcut that can show/hide a dedicated Warp window or all Warp windows on your chosen desktop, regardless of whether the app is focused.
- On macOS, system keyboard shortcuts like CMD-ESC, CMD-BACKTICK, CMD-TAB, CMD-PERIOD, and CMD-TILDE need to be unbound before you can use them in Warp.
- On Linux, the Global Hotkey may not work for some X11 window managers that do not implement Extended Window Manager Hints. Some examples include: sowm, catwm, Fvwm, dwm, 2bWM, monsterwm, TinyWM, x11fs, XMonad.
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

### 2. Tabs
- The Tabs feature allows you to organize a window into multiple terminal sessions. Tabs can be customized with a title and/or an ANSI color to help identify them.
- New Tabs will default to the active Tab’s current Working Directory, and the actual color values will be automatically derived from your Warp Theme.

#### How to use Tabs
- Right-click on the new Tab button + to make a new tab, restore closed tab, or run a saved Launch Configuration.
- Open a new Tab with **CTRL-SHIFT-T** or by clicking on the + in the top bar.
- Close the current Tab with **CTRL-SHIFT-W** or by clicking on the x on hover over a Tab.
- Reopen closed tabs with **CTRL-ALT-T**.
- Move a Tab to the Left / Right with **CTRL-SHIFT-LEFT / CTRL-SHIFT-RIGHT** or by clicking and dragging a Tab.
- Activate the Previous / Next Tab with **CTRL-PGUP / CTRL-PGDN** or by clicking a Tab.
- Activate the first through eighth Tabs with **CTRL-1 thru CTRL-8**.
- Switch to the last Tab with **CTRL-9**.
- Double-click a Tab to rename it.
- Right-clicking on a Tab reveals more options you can explore within the Command Palette or Keyboard Shortcuts.

#### How to use Tabs
- Right-click on the new Tab button + to make a new tab, restore closed tab, or run a saved Launch Configuration.
- Open a new Tab with **CTRL-SHIFT-T** or by clicking on the + in the top bar.
- Close the current Tab with **CTRL-SHIFT-W** or by clicking on the x on hover over a Tab.
- Reopen closed tabs with **CTRL-ALT-T**.
- Move a Tab to the Left / Right with **CTRL-SHIFT-LEFT / CTRL-SHIFT-RIGHT** or by clicking and dragging a Tab.
- Activate the Previous / Next Tab with **CTRL-PGUP / CTRL-PGDN** or by clicking a Tab.
- Activate the first through eighth Tabs with **CTRL-1 thru CTRL-8**.
- Switch to the last Tab with **CTRL-9**.
- Double-click a Tab to rename it.
- Right-clicking on a Tab reveals more options you can explore within the Command Palette or Keyboard Shortcuts.

### Terminal Tip
Using your .zshrc or .bashrc files on macOS or Linux, you can set a new Tab name:

```bash
# Set name, where MyTabName would be whatever you want to see in the Tab (either a fixed string, $PWD, or something else)
function set_name () {
  echo -ne "\033]0;MyTabName\007"
}
# Add the function to the environment variable in either Zsh or Bash
if [ -n "$ZSH_VERSION" ]; then
  precmd_functions+=(set_name)
elif [ -n "$BASH_VERSION" ]; then
  PROMPT_COMMAND='set_name'
fi
```

Learn more about Tab names here.

### 3. Tab Restoration
- Tab Restoration enables you to reopen recently closed tabs for up to 60 seconds. Configure this feature in **Settings > Features > Session > Enable reopening of closed sessions**.

### 4. Split Panes
- The Split Panes feature allows you to divide a tab into multiple rectangular panes, each of which is a unique terminal session.

### CTRL-TAB Behavior
- The **CTRL-TAB** shortcut defaults to activate the previous / next Tab. You can configure the shortcut to cycle the most recent session, including any Split Panes, in **Settings > Features > Keys > Ctrl-Tab behavior**.

### Tabs Behavior
- Please see our **Appearance > Tabs Behavior** docs for more Tab related settings.

This guide will assist users in understanding and utilizing Window Management features effectively within the Warp terminal.
