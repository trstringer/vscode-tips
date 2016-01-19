# Productivity

#### In this section
- [IntelliSense (JavaScript)](#intelliSense-for-javascript)

## IntelliSense for JavaScript

> :bulb: JavaScript is a dynamically-typed language, but in order to be able to utilize IntelliSense (a *huge* tool when writing code) you can download the TypeScript definition file from DefinitelyTyped, as VS Code will recognize the type definition file and utilize it for IntelliSense.  Don't be thrown off by the "TypeScript" part of this.  If you are just writing plain JavaScript (and not TypeScript) you will still utilize these TypeScript definition files for IntelliSense

### Enable IntelliSense for a JavaScript package from npm 

1. *(first time only)* Install the TypeScript definition manager: `npm install --global tsd`
2. Navigate to the workspace's root directory
3. *(optional)* Search for the tsd file you want: (i.e.) `tsd query node`
4. Install the tsd file: (i.e.) `tsd install node`

> :bulb: This will create (if not already existing) a folder in the workspace root named `typings` and each *.d.ts file will be placed in its owning folder (i.e. `.\typings\node\node.d.ts`)

> :bulb: You can also search for type definition files on [DefinitelyTyped's website](http://definitelytyped.org/tsd/)