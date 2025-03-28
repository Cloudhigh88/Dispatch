# Keyboard Shortcuts in Warp

## Overview
Warp provides a variety of keyboard shortcuts to enhance user productivity and streamline workflows. Users can quickly access commonly used commands and customize their keyboard shortcuts to fit their preferences.

## Accessing Keyboard Shortcuts
- Warp opens with a shortcut screen displaying some of the most commonly used keyboard shortcuts. You can hide the shortcut screen by clicking the "x" button.
- Quickly view keyboard shortcuts via the Command Palette or the Resource Center keyboard shortcut sidebar.

## Custom Keyboard Shortcuts
- Set custom, clear, or default keyboard shortcuts by navigating to **Settings > Keyboard Shortcuts**.
- Use the search bar to find re-mappable actions or existing shortcuts.
- Remap keyboard shortcuts using a file. Refer to the keysets repository for instructions.
- On macOS, system keyboard shortcuts like CMD-ESC, CMD-BACKTICK, CMD-TAB, CMD-PERIOD, and CMD-TILDE need to be unbound before you can use them in Warp.
- Keybinds that conflict with others are highlighted with an orange border.

## Commonly Used Shortcuts

### Warp Essentials
| Shortcut         | Command                                   | Action                                      |
|------------------|-------------------------------------------|---------------------------------------------|
| CTRL-SHIFT-D     | Split Pane Right                          | pane_group:add_right                        |
|                  | Launch Configuration Palette              | workspace:toggle_launch_config_palette      |
|                  | Open Theme Picker                         | workspace:show_theme_chooser                |
| CTRL-R           | Command Search                            | workspace:show_command_search                |
| CTRL-SHIFT-R     | Workflows                                 | input:toggle_workflows                      |
| CTRL-`           | Generate                                  | input:toggle_natural_language_command_search |
| CTRL-SHIFT-L     | Focus Terminal Input                      | terminal:focus_input                        |
| CTRL-I           | Warpify Subshell                         | terminal:trigger_subshell_bootstrap         |
| CTRL-SHIFT-\     | Warp Drive                                | terminal:toggle_warp_drive                  |

### Blocks
| Shortcut         | Command                                   | Action                                      |
|------------------|-------------------------------------------|---------------------------------------------|
| ALT-DOWN         | Select the Closest Bookmark Down          | terminal:select_bookmark_down               |
| CTRL-SHIFT-ALT-C | Copy Command Output                        | terminal:copy_outputs                       |
| ALT-UP           | Select the Closest Bookmark Up            | terminal:select_bookmark_up                 |
| CTRL-SHIFT-A     | Select All Blocks                         | terminal:select_all_blocks                  |
| CTRL-SHIFT-K     | Clear Blocks                              | terminal:clear_blocks                       |
| CTRL-SHIFT-B     | Bookmark Selected Block                   | terminal:bookmark_selected_block            |
| CTRL-DOWN        | Select Next Block                         | terminal:select_next_block                  |
| CTRL-SHIFT-I     | Reinput Selected Commands                 | terminal:reinput_commands                   |
| CTRL-UP          | Select Previous Block                     | terminal:select_previous_block              |
|                  | Open Block Context Menu                   | terminal:open_block_list_context_menu_via_keybinding |
| CTRL-SHIFT-C     | Copy Command                              | terminal:copy_commands                       |
|                  | Reinput Selected Commands as Root         | terminal:reinput_commands_with_sudo         |
| CTRL-SHIFT-S     | Share Selected Block                      | terminal:open_share_modal                   |
| SHIFT-DOWN       | Expand Selected Blocks Below              | terminal:expand_block_selection_below       |
| SHIFT-UP         | Expand Selected Blocks Above              | terminal:expand_block_selection_above        |

### Input Editor
| Shortcut         | Command                                   | Action                                      |
|------------------|-------------------------------------------|---------------------------------------------|
| CTRL-BACKSPACE    | Delete Word Left                         | editor:delete_word_left                     |
| CTRL-ALT-F       | Fold Selected Ranges                      | editor_view:fold_selected_ranges            |
| CTRL-ALT-[       | Fold                                      | editor_view:fold                            |
| CTRL-ALT-]       | Unfold                                    | editor_view:unfold                          |
| CTRL-DELETE       | Delete Word Right                        | editor:delete_word_right                    |
| CTRL-A           | Select All                                | editor_view:select_all                      |
| CTRL-Y           | Delete All Left                          | editor_view:delete_all_left                 |
|                  | Delete All Right                         | editor_view:delete_all_right                |
| CTRL-END         | Move Cursor to the Bottom                | editor_view:cmd_down                        |
| CTRL-I           | Inspect Command                           | editor_view:cmd_i                           |
| HOME             | Home                                      | editor_view:home                            |
| END              | End                                       | editor_view:end                             |
| CTRL-A           | Move to Start of Line                    | editor_view:move_to_line_start              |
| CTRL-B           | Move Cursor Left                         | editor_view:left                            |
| CTRL-C           | Clear Command Editor                      | editor_view:clear_buffer                    |
| CTRL-D           | Delete                                    | editor:view:delete                          |
| CTRL-E           | Move to End of Line                      | editor_view:move_to_line_end                |
| CTRL-F           | Move Cursor Right / Accept Autosuggestion | editor_view:right                           |
| CTRL-G           | Add Selection for Next Occurrence        | editor_view:add_next_occurrence             |
| CTRL-H           | Remove the Previous Character             | editor_view:backspace                       |
| CTRL-J           | Insert Newline                            | editor_view:insert_newline                  |
| CTRL-K           | Cut All Right                            | editor_view:cut_all_right                   |
| CTRL-L           | Clear Screen                              | input:clear_screen                          |
| CTRL-N           | Move Cursor Down                          | editor_view:down                            |
| CTRL-P           | Move Cursor Up                            | editor_view:up                              |
|                  | Select to Start of Line                   | editor_view:select_to_line_start            |
| CTRL-SHIFT-B     | Select One Character to the Left          | editor_view:select_left                     |
| CTRL-SHIFT-DOWN  | Add Cursor Below                          | editor_view:add_cursor_below                |
|                  | Select to End of Line                     | editor:select_to_line_end                   |
| CTRL-Z           | Undo                                      | editor:undo                                 |
| CTRL-SHIFT-Z     | Redo                                      | editor:redo                                 |
| CTRL-SHIFT-F     | Select One Character to the Right         | editor:select_right                         |
|                  | Select Down                                | editor_view:select_down                     |
| CTRL-SHIFT-P     | Select Up                                  | editor_view:select_up                       |
| CTRL-SHIFT-UP    | Add Cursor Above                          | editor_view:add_cursor_above                |
| CTRL-U           | Copy and Clear Selected Lines             | editor_view:clear_and_copy_lines            |
| CTRL-W           | Cut Word Left                             | editor_view:cut_word_left                   |
| META-.           | Insert Last Word of Previous Command      | editor:insert_last_word_previous_command     |
| META-A           | Move to the Start of the Paragraph        | editor_view:move_to_paragraph_start         |
| CTRL-LEFT        | Move Backward One Word                    | editor_view:move_backward_one_word          |
| ALT-D            | Cut Word Right                            | editor_view:cut_word_right                  |
| META-E           | Move to the End of the Paragraph          | editor_view:move_to_paragraph_end           |
| CTRL-RIGHT       | Move Forward One Word                     | editor_view:move_forward_one_word           |
| CTRL-ALT-LEFT    | Move Backward One Subword                 | editor_view:move_backward_one_subword       |
| CTRL-ALT-RIGHT   | Move Forward One Subword                  | editor_view:move_forward_one_subword        |
| SHIFT-META-<     | Move to the Start of the Buffer           | editor_view:move_to_buffer_start            |
| SHIFT-META->     | Move to the End of the Buffer             | editor_view:move_to_buffer_end              |
| CTRL-SHIFT-LEFT   | Select One Word to the Left               | editor_view:select_left_by_word             |
| CTRL-SHIFT-RIGHT  | Select One Word to the Right              | editor_view:select_right_by_word            |

### Terminal
| Shortcut         | Command                                   | Action                                      |
|------------------|-------------------------------------------|---------------------------------------------|
| CTRL-ALT-DOWN    | Switch Panes Down                         | pane_group:navigate_down                    |
| CTRL-ALT-LEFT    | Switch Panes Left                         | pane_group:navigate_left                    |
| CTRL-ALT-RIGHT   | Switch Panes Right                        | pane_group:navigate_right                   |
| CTRL-ALT-UP      | Switch Panes Up                           | pane_group:navigate_up                      |
| CTRL-ALT-V       | [a11y] Set Concise Accessibility Announcements | workspace:set_a11y_concise_verbosity_level |
| CTRL-ALT-V       | [a11y] Set Verbose Accessibility Announcements | workspace:set_a11y_verbose_verbosity_level  |
| CTRL-,           | Open Settings                             | workspace:show_settings_modal               |
| CTRL-,           | Open Settings: Account                    | workspace:show_settings_account_page        |
| F3               | Find the Next Occurrence of Your Search Query | find:find_next_occurrence                  |
| CTRL-SHIFT-P     | Toggle Command Palette                    | workspace:toggle_command_palette            |
|                  | Toggle Mouse Reporting                    | workspace:toggle_mouse_reporting            |
| CTRL-SHIFT-[     | Activate Previous Pane                    | pane_group:navigate_prev                    |
| CTRL-SHIFT-]     | Activate Next Pane                        | pane_group:navigate_next                    |
|                  | Resize Pane > Move Divider Down           | pane_group:resize_down                      |
| CTRL-CMD-K       | Open Keybindings Editor                   | workspace:show_keybinding_settings          |
|                  | Resize Pane > Move Divider Left           | pane_group:resize_left                      |
|                  | Resize Pane > Move Divider Right          | pane_group:resize_right                     |
|                  | Resize Pane > Move Divider Up             | pane_group:resize_up                        |
| CTRL-SHIFT-/     | Open Resource Center                      | workspace:toggle_resource_center            |
| CTRL-SHIFT-E     | Split Pane Down                           | pane_group:add_down                         |
| CTRL-SHIFT-ENTER | Toggle Maximize Active Pane               | pane_group:toggle_maximize_pane            |
| SHIFT-F3         | Find the Previous Occurrence of Your Search Query | find:find_prev_occurrence                  |
|                  | Toggle Navigation Palette                 | workspace:toggle_navigation_palette         |

This guide will assist users in understanding and utilizing keyboard shortcuts effectively within the Warp terminal.
