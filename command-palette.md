# Command Palette

## What is it??

The Command Palette is the keyboard way to accomplish just about any task that you would desire in Visual Studio Code.  The benefits of knowing and using the Command Palette extensively are:

1. Ease of use (one place for almost every action)
2. Speed (keystrokes are faster than mouse clicks)

> :exclamation: Force yourself to rely heavily on the command palette and keyboard shortcuts.  It'll feel "awkward" at first, but in no time you will be exponentially more productive when you become well-versed with the command palette and keyboard shortcuts

## Open the Command Palette

#### (recommended) Keyboard Shortcut

`CTRL+SHIFT+P`

#### (not recommended) Menu

*View -> Command Palette...*

## Command Palette Operations

> :bulb: The best way to think about the command palette is that it uses a convention where the first "indicator" directs it to a subset of commands that are related

### Subsets

#### Help

`?` - shows the available subset entrance commands

#### Run commands

`>` - once you type this greater-than symbol you'll see all of the commands.  Type partial command strings in to search through the available commands

#### Open files

`<partial-file-name>` - start typing in the partial file name (including just an extension to get all files with the desired extension)

> :bulb: Hold down `CTRL` while hitting `ENTER` to open the selected file in a new editor instead of replacing your currently-focused editor with the desired file 

#### Symbols

`@[partial-symbol-name]` - with no partial symbol name, it'll display all of the symbols in the currently-focused file

`@:[partial-symbol-name]` - (recommended) this sorts the symbols by the different categories (i.e. functions, variables, etc.)

> :exclamation: This is a *super* quick and easy way to go to a symbol in the current file instead of having to scroll and search with your eyes.  Highly recommended!

#### Go to line

`:<line-number>` - moves cursor to the specified line number in the currently-focused editor

#### Errors and warnings

`!`

> :bulb: Use the up and down arrow keys to select different errors or warnings to select and navigate to

#### Git

`git <command>` - allows you to currently `checkout` or `branch`

`>Git:` - brings up other git commands available

#### Tasks

`task [partial-task-name]` - without specifying a partial, it'll pull up all current tasks in the workspace

> :bulb: Use the up and down arrow keys to select desired task and `ENTER` to run it

#### Extensions

`ext [partial-ext-name]` - list locally installed extensions (optionally with a search term)

`ext install [partial-ext-name]` - search and install an extension

`ext update` - update locally installed extensions