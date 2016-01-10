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