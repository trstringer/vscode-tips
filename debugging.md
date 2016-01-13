# Debugging

## launch.json

The `launch.json` is the configuration that Visual Studio Code uses to determine how to run and debug your application.  This configuration is typically defined as the following...

```json
{
  "version": "0.2.0",
  "configurations": [
    { ... },
    { ... }
  ]
}
```

`version` is the version of the configuration file.  `configurations` is what contains the array of different launch configurations.

> :bulb: You can have multiple configurations for different running and debugging scenarios within a single workspace

### Common configuration settings

- **name**: the name of the launch configuration (referenced when selecting which to use when running/debugging)
- **type**: *node*, *mono*, *extensionHost*, *go* (specifies the config environment)
- **request**: *launch*, *attach*
- **program**: the starting point source file (i.e. *app.js*) for launching
- **stopOnEntry**: if set to *true*, break on entry of the application. If set to *false* then run until explicit breakpoint or end of application
- **args**: command line arguments passed in
- **cwd**: location of the workspace that will be launched/debugged (defaults to `.`)
- **runtimeExecutable**: if specified, this will be the runtime executable (if not, it'll use the `PATH` env var)
- **env**: array of environment variables
- **externalConsole**: *true* to launch in separate console window, otherwise *false* to run in VS Code
- **sourceMaps**: if *true* use source maps if they exist, if *false* then do not
- **outDir**: specify where the generated source map code exists if not in the same directory as the original source
- **preLaunchTask**: *(must have tasks setup)* the task to run prior to launch the application
- **port**: *(when working with `request: attach`)* the port to attach to

## Debug experience

*Visual Studio Code provides a well-known and accepted debugging experience with breakpoints, variables, call stack, and console*

#### Switch to debug workbench

The keyboard shortcut to switch the IDE to the debug workbench is `CTRL+SHIFT+D` (configurable in `keybindings.json`)

#### Breakpoints

- **Toggle Breakpoint** - `F9` (configurable in `keybindings.json`)
- **Disable Breakpoint** - in the debug workbench, uncheck the desired breakpoint to disable
- **Enable Breakpoint** - in the debug workbench, check the desired breakpoint to enable
- **Remove Breakpoint** - in the debug workbench, hit the `X` next to the breakpoint to remove it

#### Debug console

The debug console is a common way to interact with the current state of the application during typical debugging scenarios.

Open the console: `>Debug: Open Console`