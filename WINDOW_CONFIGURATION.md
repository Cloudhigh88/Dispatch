# Window Configuration for Warp Terminal

## Overview
Warp supports settings for window size, opacity (transparency), and blurring effects, allowing users to customize their terminal layout and visual preferences.

## Window Size
To access size settings:
1. Navigate to **Settings > Appearance > Window**.
2. Enable **Open new windows with custom size**.
3. Configure your preferred number of columns and rows.

### Session Restoration
- If Session Restoration is enabled, Warp will restore the size of the last window closed when you quit the app. 
- Ensure that the custom-sized window is the last one closed, or disable Session Restoration to launch Warp with the custom-sized window.

## Window Opacity
To adjust window opacity:
1. Go to **Settings > Appearance > Themes**.
2. Use the slider to set the opacity value between 1 and 100, where 100 is completely opaque.

## Window Blurring
To enable window blurring:
- After decreasing Opacity (moving the slider to a value less than 100), you can blur the background.
  - **On macOS**: Use the blur slider to increase the blur radius applied to the background image.
  - **On Windows**: Toggle the Acrylic background texture on or off.

### Performance Considerations
- On macOS, large blur radiuses may affect performance, especially on Retina displays.
- On Linux, window blurring is not supported.
- On Windows, some graphics drivers may not support rendering transparent or translucent windows. Refer to troubleshooting tips if issues arise.

This guide will assist users in personalizing their terminal window settings effectively.
