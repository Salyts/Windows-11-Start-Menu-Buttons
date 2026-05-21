# Windows 11 Start Menu Buttons 2.1

Replaces the default bottom row of the Windows 11 Start menu with fully customizable buttons.

❗**There may be issues with mods:** [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler), [Windows 11 Start Menu Power Buttons](https://windhawk.net/mods/win11-power-buttons).

![img](https://i.imgur.com/J5CC8XP.png)

![img](https://i.imgur.com/dm7SVQj.png)

---
## Installation

1. Install [Windhawk](https://windhawk.net/).
2. Open **Windhawk** and go to **Explore** → **Search**.
3. Enter **Windows 11 Start Menu Buttons** in the search field.
4. In the results, select [Windows 11 Start Menu Buttons](https://windhawk.net/mods/windows-11-start-menu-buttons).
5. Click the "Install" button.

---

## Quick Start

1. Open Windhawk settings for this mod.
2. Add buttons using the **Buttons** list.
3. For each button, pick a **Preset** or set **Preset = Custom** and fill in Name, Icon, Action.
4. Save — the Start menu updates immediately.

---

## Button fields

| Field    | Description |
|----------|-------------|
| **Preset** | Ready-made button. Set to `Custom` to define your own. |
| **Name** | Tooltip shown on hover. Leave empty on presets to use their default name. |
| **Icon** | [Segoe Fluent Icons](https://learn.microsoft.com/en-us/windows/apps/design/iconography/segoe-ui-symbol-font) glyph (e.g. `\uE7E8`) **or** full path to an image file (PNG, ICO, JPG, BMP). |
| **Action** | Used only when Preset = `Custom`. See action formats below. |
| **Submenu** | Optional list of child items shown in a flyout. If any submenu items are defined, the button opens the flyout instead of running a direct action. |

---

## Action formats (Custom preset only)

| Prefix | Example | Description |
|--------|---------|-------------|
| `" "` | `"C:\Program Files\Windhawk\windhawk.exe"` | Opens a file or folder by absolute path. |
| `~` | `~Downloads` and `~windhawk.exe` | Opens a folder or file by name. |
| `cmd:` | `cmd:control` | Runs a command through `cmd.exe`. |
| `shell:` | `shell:shutdown /r /f /t 0` | Runs through `powershell.exe`. |
| `press:` | `press:Win+E` or `press:0x5B;0x45` | Keyboard key press using a [Win32 key code](https://learn.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes). |
| `web:` | `web:https://windhawk.net/` | Opens a URL in the default browser. |
| `ms-settings:` | `ms-settings:bluetooth` | Opens a Windows Settings page. |

### Modifier signs (prepend to any action)

| Sign | Example | Description |
|--------|---------|-------------|
| `-` | `-"C:\Program Files\app.exe"` or `-shell:shutdown /r /f /t 0` | Runs as administrator. |
| `*` | `*cmd:tasklist` or `*shell:Get-Process` | Execution with a terminal window. (only for `cmd:` and `shell:` prefixes). |

Signs can be combined: `-*cmd:tasklist` runs cmd in a visible window as admin.

---

## Icon field

| Type | Example | Description |
|---|---|---|
| **Glyph** | `E774` or `\uE774` | Hex code of a [Segoe Fluent Icons](https://learn.microsoft.com/en-us/windows/apps/design/iconography/segoe-ui-symbol-font) glyph. 4-digit hex, `\u` prefix is optional. |
| **Image file** | `C:\Icons\name.png` | Full path to an image. Supported: `.png` `.ico` `.jpg` `.bmp` `.webp`. Recommended: 32x32 px, transparent background. |
| **App path** | `C:\Program Files\Windhawk\windhawk.exe` | Full path to an executable file (`.exe`, `.dll`). The icon will be extracted from the application. |

---

## Presets

| ID | Name | Icon | Description |
|---|---|---|---|
| 1 | `Settings` | \uE713 | Opens Windows Settings. |
| 2 | `Explorer` | \uEC50 | Opens File Explorer. |
| 3 | `Documents` | \uE8A5 | Opens the Documents folder. |
| 4 | `Music` | \uEC4F | Opens the Music folder. |
| 5 | `Downloads` | \uE896 | Opens the Downloads folder. |
| 6 | `Pictures` | \uE91B | Opens the Pictures folder. |
| 7 | `Videos` | \uE714 | Opens the Videos folder. |
| 8 | `Network` | \uEC27 | Opens Network places. |
| 9 | `Personal Folder` | \uEC25 | Opens the user's profile folder. |
| 10 | `Shut down` | \uE7E8 | Shuts down the PC. |
| 11 | `Restart` | \uE777 | Restarts the PC. |
| 12 | `Sign out`| \uF3B1 | Logs out of the current account. |
| 13 | `Sleep` | \uE708 | Puts the PC to sleep. |
| 14 | `Hibernate` | \uE823 | Hibernates the PC. |
| 15 | `Lock` | \uE72E | Locks the PC session. |
| 16 | `Power Menu` | \uE7E8 | Opens the power options menu. |

## Submenus

Fill in the **Submenu** entries for a button. Each submenu item has its own Name, Icon, and Action.
When at least one submenu item exists, the button opens a flyout menu instead of executing a direct action.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Thank you so much, [@SharkIT-sys](https://github.com/SharkIT-sys), for helping to improve the mod!
