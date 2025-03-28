# Text, Fonts, and Cursor Configuration for Warp Terminal

## Overview
Warp supports customizing the font and how text is displayed, which can enhance readability and usability. Additionally, users can customize the cursor behavior.

## Text and Fonts
To access text and font settings:
1. Navigate to **Settings > Appearance > Text**.

### Customization Options
- **Font Type**: Select from available system fonts.
- **Font Weight**: Adjust the weight of the font.
- **Font Size**: Set the desired font size.
- **Line Height**: Customize the line height for better readability.
- **Use Thin Strokes**: This option prevents text from appearing blurry on low-DPI displays. (Note: Not supported on Linux.)
- **Enforce Minimum Contrast**: This setting tweaks named colors to meet accessibility standards.
- **Show Ligatures in Terminal**: Enabling ligatures can reduce performance. It is recommended to use fonts that support ligatures (e.g., Fira Code) as Warp's default font, Hack, does not yet support ligatures.

### Important Note
Once a new font is installed on your system, restart Warp for it to appear in the list of options. You may also need to check "View all available system fonts" to see the new font.

## Cursor Configuration
To access cursor settings:
1. Navigate to **Settings > Appearance > Cursor**.

### Customization Options
- **Cursor Type**: Choose between Bar, Block, or Underline.
- **Blinking Cursor**: Toggle the blinking cursor option. You can also toggle this setting from the Command Palette by typing "Cursor blink".

### Cursor Type Preference
Note that cursor type preference is disabled while Vim keybindings (vim mode) are active.

This guide will assist users in personalizing their terminal's text display and cursor behavior effectively.
