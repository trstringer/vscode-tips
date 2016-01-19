# Productivity

#### In this section
- [IntelliSense (JavaScript)](#intellisense-for-javascript)
- [Tasks](#tasks)

## IntelliSense for JavaScript

> :bulb: JavaScript is a dynamically-typed language and in order to be able to utilize IntelliSense (a *huge* tool when writing code) you can download the TypeScript definition file from DefinitelyTyped, as VS Code will recognize the type definition file and utilize it for IntelliSense.  Don't be thrown off by the "TypeScript" part of this.  If you are just writing plain JavaScript (and not TypeScript) you will still utilize these TypeScript definition files for IntelliSense

### Enable IntelliSense for a JavaScript package from npm 

1. *(first time only)* Install the TypeScript definition manager: `npm install --global tsd`
2. Navigate to the workspace's root directory
3. *(optional)* Search for the tsd file you want: (i.e.) `tsd query node`
4. Install the tsd file: (i.e.) `tsd install node`

> :bulb: This will create (if not already existing) a folder in the workspace root named `typings` and each `*.d.ts` file will be placed in its owning folder (i.e. `.\typings\node\node.d.ts`)

> :bulb: You can also search for type definition files on [DefinitelyTyped's website](http://definitelytyped.org/tsd/)

## Tasks

### Enable tasks

1. *(command palette)* `>Tasks: Configure Task Runner`
2. In the `tasks.json` configuration file, uncomment out your task runner to define it (gulp, tsc, jake, msbuild)
3. *See below instructions for different task runners*

#### Gulp tasks

1. Enable tasks and uncomment out the `gulp` section
2. Install gulp locally (as well as any gulp modules specific to your needs): `npm install --save-dev gulp`
3. Create `gulpfile.js` in your workspace's root directory
4. Create your gulp tasks in the `gulpfile.js`

### Run tasks

From the command palette, type `task` and there will be a dropdown of all defined tasks.  To run a particular task either arrow-key-down to it, or type in `task <your-task-name>` and hit `ENTER`

### PreLaunch task

> :bulb: Define a prelaunch task if you would like to automatically run a particular task prior to launching your application from VS Code

1. Open up (or generate if not yet created) the `launch.json` configuration file
2. Navigate to the particular debug configuration you want to add the prelaunch task to
3. Add the following to the configuration: `"preLaunchTask": "your-prelaunch-task-name"`

Now when you `F5/debug` your application, this prelaunch task will automatically start prior to launching the software

### Special tasks

> :bulb: VS Code defines a few special tasks (**build** and **test**) that you can leverage in a quicker and more efficient way

#### Build task

Do one of the following to **define your build task**...
- create a task named `build`
- or define your task in `tasks.json` and specify `true` for the `isBuildCommand` property

**Run the build task** by doing either...
- (recommended) the keyboard shortcut: `CTRL+SHIFT+B`
- command palette: `>Tasks:Run Build Task`
- command palette: `task <your-build-task-name>`

#### Test task

Do one of the following to **define your test task**...
- create a task named `test`
- or define your task in `tasks.json` and specify `true` for the `isTestCommand` property

**Run the test task** by doing either...
- (recommended) the keyboard shortcut: `CTRL+SHIFT+T`
- command palette: `>Tasks:Run Test Task`
- command palette: `task <your-test-task-name>`

#### Watch task (gulp)

> :bulb: Create a watch task if you want code to run when files are saved (i.e. auto-minification)

1. Create a `watch` task in your `gulpfile.js`
2. Have the watch task run `gulp.watch()` and specify an array of tasks that should be run on save
3. *(optional)* Turn on auto-save in VS Code: `>Files:Enable Auto Save` (only do this if you want VS Code to auto save)