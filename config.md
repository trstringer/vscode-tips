# Configuration and Settings

#### In this section
- [Settings](#settings)

## Settings

Settings have two different scopes: **user** and **workspace**.  User settings apply to the user, and workspace applies to the currently open workspace/folder.

Settings are applied in the following scope (latter overriding former)

**Default Settings** > **User Settings** > **Workspace Settings**  

> :bulb: Workspace settings override user settings

### Change User Settings

Open up settings by doing one or the other:

- Command Palette - `>Preferences: Open User Settings`
- Menu - *File -> Preferences -> User Settings*

This will open up two editor windows:

- Default Settings (do **not** modify anything in here)
- settings.json

In `settings.json` you specify the configuration item (lookup from *Default Settings* the option you want to change for reference and copy it over to `settings.json`).

#### Example

*You want to change change the tab size from 4 to 2*

1. Locate the setting in *Default Settings*
```json
	// Controls the rendering size of tabs in characters. Accepted values: "auto", 2, 4, 6, etc. If set to "auto", the value will be guessed when a file is opened.
	"editor.tabSize": 4
```
2. Copy (or type) this to `settings.json` and modify the value in `settings.json`
```json
	"editor.tabSize": 2
```

### Change Workspace Settings

Open the workspace settings by doing one of the following:

- Command Pallete - `>Preferences: Open Workspace Settings`
- Menu - *File -> Preferences -> Workspace Settings*