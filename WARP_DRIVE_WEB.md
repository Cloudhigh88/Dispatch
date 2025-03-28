# Warp Drive on the Web

## Overview
Warp Drive on the Web allows developers to view their drives and shared sessions through a web browser, enhancing accessibility and flexibility.

## Accessing Warp Drive on the Web
You can access Warp's web-based viewing experience via:
- The homepage: **app.warp.dev/app**
- Drive Object Links
- Session Sharing Links

Users can edit and view web-based objects and sessions as normal. However, executing a command from a workflow or notebook is not possible since there is no shell session running on the web.

## Managing Your View Preferences - Web or Desktop
If the Warp app is installed, links will open on the desktop by default. You can manage whether Warp links open in the desktop app or the browser in several ways:
- The desktop option is presented only if Warp's web service detects the Warp app installed locally. This detection is done through localhost port 9277 in a separate process that does not access your terminal contents.
- The first time you follow a link, if Warp is not installed, you will be prompted to download it. You can dismiss the popup to stay on the web.
- This preference can be changed at any point in **Settings > Features > General > Open links in desktop app**. Note that this setting is only available while on the web-based version of Warp.

### Switching Between Web and Desktop Views
You can switch between web and desktop views on a case-by-case basis:
- To switch from a web view to Desktop for a given object, open the overflow menu and select **Open link on Desktop**.
- To stay on the web for a given object despite a global Desktop preference, follow the **View on the web** option that is part of the redirect screen to Desktop.

## Supported Browsers
Modern browser support currently includes:
- Chrome
- Firefox

This guide will assist users in understanding and utilizing Warp Drive on the Web effectively.
