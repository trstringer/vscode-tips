# Other Languages

#### In this section
- [PowerShell](#powershell)
- [Go](#go)
- [Markdown](#markdown)

## PowerShell

#### Installing

*(Command palette)* `ext install powershell`

#### Usage

1. Create a new workspace directory
2. Add one or more `*.ps1` files
3. Run (`F5`) and select the `PowerShell` environment

> :bulb: Ensure that the `.\vscode\launch.json` configuration is set correctly

## Markdown

> :bulb: Markdown is a first-class citizen in VS Code.  It requires no extra downloads or extensions.

1. Create or open a markdown file `*.md`
2. Open the markdown preview with the command palette: `>Markdown: Open Preview to the Side`
3. *(Recommended)* Default keyboard shortcut: `CTRL+K V`

## Go

1. [Download and install Go](http://golang.org)
2. Set your `GOPATH` environment variable appropriately (i.e. *powershell* `[Environment]::SetEnvironmentVariable("GOPATH", "C:\Go\pkg", "User")`)
3. Install the Go extension with the command palette: `ext install Go`
4. Create a new workspace (or open an existing Go workspace)
5. *(command prompt)* Run your Go source: `go run your-file.go` 