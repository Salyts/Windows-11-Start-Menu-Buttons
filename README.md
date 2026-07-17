# Windows 11 Start Menu Buttons 2.2

Replace the Windows 11 Start menu's bottom bar with fully customizable buttons!

❗ **There may be conflicts with these mods:** [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler), [Windows 11 Start Menu Power Buttons](https://windhawk.net/mods/win11-power-buttons).

![img](https://i.imgur.com/J5CC8XP.png)

![img](https://i.imgur.com/dm7SVQj.png)

---

## Visual Configurator

Configure your buttons visually using the **[Start Menu Buttons Configurator](https://salyts.github.io/Windows-11-Start-Menu-Buttons/)** — a web-based tool that lets you:

- Add, remove and reorder buttons with drag & drop
- Set icons, names and actions visually
- Build nested submenus (left-click and right-click, up to 3 levels)
- Preview your layout in real time
- Export / import configuration as YAML text
- Migrate settings from v2.1 to v2.2

👉 **[Open Configurator](https://salyts.github.io/Windows-11-Start-Menu-Buttons/)**

---

## Installation

1. Install [Windhawk](https://windhawk.net/).
2. Open **Windhawk** → **Explore** → **Search**.
3. Search for **Windows 11 Start Menu Buttons**.
4. Click **Install**.

---

## Quick Start

1. Open Windhawk settings for this mod.
2. Add buttons using the **Buttons** list.
3. Pick a **Preset** (ready-made template) or set **Preset = Custom** for your own button.
4. Configure Name, Icon, and Action.
5. Save — the Start menu updates immediately.

---

## Upgrading from v2.1 to v2.2

Your buttons will continue to work after upgrading. However, the **Action** field may appear empty in the Windhawk UI because v2.2 changed it from a plain string to an array to support multiple commands.

**Your actions still work** — the mod reads old settings automatically. But if you want to edit actions or add multiple commands, re-enter them manually:

1. Open mod settings in Windhawk.
2. For each button with an empty Action field, re-enter the command.
3. Save.

Alternatively, use the **[Configurator's Migrate tool](https://salyts.github.io/Windows-11-Start-Menu-Buttons/)** to convert your v2.1 config automatically.

---

## Button Fields

| Field | Description |
|---|---|
| **Preset** | Ready-made button template. Set to `Custom` to define your own. |
| **Name** | Tooltip shown on hover. Leave empty on presets to use their default name. |
| **Icon** | [Segoe Fluent Icons](https://learn.microsoft.com/en-us/windows/apps/design/iconography/segoe-fluent-icons-font) glyph, image file path, or `.exe`/`.dll` path to extract icon. |
| **Action** | Action for Custom preset only. Supports multiple commands. See formats below. |
| **Left-click submenu** | Flyout menu opened on left-click (up to 3 levels deep). |
| **Right-click submenu** | Separate flyout menu opened on right-click (up to 3 levels deep). |

---

## Action Formats (Custom preset only)

| Prefix | Example | Description |
|---|---|---|
| path | `C:\Program Files\app.exe` | Opens a file or folder by absolute path. |
| `~` | `~Downloads` | Opens a folder or file by name. |
| `cmd:` | `cmd:control` | Runs a command via `cmd.exe`. |
| `shell:` | `shell:shutdown /r /f /t 0` | Runs via `powershell.exe`. |
| `press:` | `press:Win+E` or `press:0x5B;0x45` | Keyboard key press using [Win32 VK codes](https://learn.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes). |
| `web:` | `web:https://windhawk.net/` | Opens a URL in the default browser. |
| `ms-settings:` | `ms-settings:bluetooth` | Opens a Windows Settings page. |

### Modifier Signs

Prepend to any action:

| Sign | Example | Description |
|---|---|---|
| `-` | `-cmd:regedit` | Run as administrator. |
| `*` | `*cmd:tasklist` | Show terminal window (`cmd:`/`shell:` only). |

Signs can be combined: `-*cmd:tasklist` runs in a visible terminal as admin.

### Multiple Commands

Add multiple Action entries in the Windhawk UI (click **Add new item**). Commands execute sequentially with a 50ms delay.

---

## Icon Field

| Type | Example | Description |
|---|---|---|
| **Glyph** | `E774` or `\uE774` | Hex code of a [Segoe Fluent Icons](https://learn.microsoft.com/en-us/windows/apps/design/iconography/segoe-fluent-icons-font) glyph. `\u` prefix is optional. |
| **Image file** | `C:\Icons\name.png` | Full path to an image. Supported: `.png` `.ico` `.jpg` `.bmp` `.webp`. Recommended: 32×32 px, transparent background. |
| **App icon** | `C:\Program Files\app.exe` | Full path to `.exe` or `.dll`. The icon is extracted automatically. |

---

## Presets

| # | Name | Icon | Description |
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
| 12 | `Sign out` | \uF3B1 | Logs out of the current account. |
| 13 | `Sleep` | \uE708 | Puts the PC to sleep. |
| 14 | `Hibernate` | \uE823 | Hibernates the PC. |
| 15 | `Lock` | \uE72E | Locks the PC session. |
| 16 | `Power Menu` | \uE7E8 | Opens the power options menu. |

---

### Credits
* **[Salyts](https://github.com/Salyts) —** Author of Windows 11 Start Menu Buttons.
* **[SharkIT-sys](https://github.com/SharkIT-sys) —** Improved code and support for button images.

### Report a Bug
If you encounter any issues or have a feature suggestion, please open a report on the project's GitHub page:
👉 **[Report an Issue on GitHub](https://github.com/Salyts/Windows-11-Start-Menu-Buttons/issues)**

---

## 📄 License

This project is licensed under the MIT License.
