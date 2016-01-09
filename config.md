# Configuration and Settings

#### In this section
- [Settings](#settings)
- [Themes](#themes)
- [Keyboard Shortcuts](#keyboard-shortcuts)

## Settings

Settings have two different scopes: **user** and **workspace**.  User settings apply to the user, and workspace applies to the currently open workspace/folder.

Settings are applied in the following scope (granular overriding broader)

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

## Themes

### Change the Theme

To change the color theme of the IDE, use the following command palette command to open up available themes:

`>Preferences: Color Theme`

### Get/Download/Install New Themes

Either search through themes from the command palette by starting typing and viewing available extensions with "theme" in them:

`ext install theme`

The easier way to browse themes to install is through the [Themes section in the Visual Studio Marketplace](https://marketplace.visualstudio.com/vscode/Themes)

## Keyboard Shortcuts

#### Open up the shortcuts configuration

`>Preferences: Open Keyboard Shortcuts`

> :bulb: To overwrite *Default Keyboard Shortcuts* or to add keyboard shortcuts, add the configuration in the `keybindings.json` file opened up in the editor

> :bulb: Scroll to the bottom of the *Default Keyboard Shortcuts* to get a listing of "other actions" that can be bound to keyboard actions
