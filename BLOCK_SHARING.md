# Block Sharing in Warp

## Overview
Block Sharing allows users to share command information with their team or community through permalinks or HTML embeds. This feature enhances collaboration and makes it easy to share technical content.

## How to Share Blocks
To share your blocks, follow these steps:
1. On a finished Block, click the context menu and select **Share...** or set up a key binding for **Share Block** in **Settings > Keyboard Shortcuts**.
2. A modal will pop up that lets you title your Block and customize it by selecting which parts of the Block you want to share (e.g., command, output, prompt, etc.).
3. Click either **"Create link"** or **"Get embed"** depending on how you want to share your Block.
4. The link or embed snippet will be copied to your clipboard.

## Sharing Options
- **Permalink**: Create and share a permalink to your Blocks to collaborate with teammates. Shared permalinks will display a preview of your code for quick context on each link.
- **Embedded Blocks**: Create and embed your Blocks on web pages to help your readers follow along with technical writing. Readers can interact with an embedded Block as they would with a Block in Warp, complete with a context menu and styling. When you click **"Get embed,"** Warp will copy an iframe to your clipboard.

### Example Embed Code
```html
<iframe src="https://app.warp.dev/block/embed/qn0g1CqQnkYjEafPH5HCVT"
title="server script error" style="width: 712px; height: 397px; border:0;
overflow:hidden;" allow="clipboard-read; clipboard-write"></iframe>
```

## Managing Shared Blocks
You can unshare a Block by navigating to **Settings > Shared blocks**. Currently, shared Blocks are accessible to anyone with the link.

## Link Previews
Shared permalinks will also display a preview of your code, compatible with any platform that supports Open Graph or Twitter meta tags, such as Slack, Twitter, Facebook, Telegram, Notion, and more.

This guide will assist users in understanding and utilizing Block Sharing effectively within the Warp terminal.
