# FlutterStep
Simple python script for auto-incrementing the build number in pubspec.yaml each time you build your project

This is a pretty simple script, but one that I couldn't find a good example to copy anywhere on the internet.  It's based on this comment https://github.com/flutter/flutter/issues/41955#issuecomment-571321918, but I'm no good at perl.  When I couldn't get it to work, I decided to reuse the reges and create a python script that is easily readable and modifiable.

## How to use
To use this, first make sure you have Python 3 installed.  Next, simply place the python script in the root folder of your project (i.e. the folder that holds your pubspec.yaml file) and configure it as a pre-build task.  If you're using VS Code, you can use the two included json files as an example to modify your launch.json and tasks.json files found in the .vscode folder.  If you don't already have a tasks.json file, you can drop mine straight into your project's .vscode folder, but depending on your Python setup, you may need to change `"python increment_build.py"` to something like `"python3 increment_build.py"`.
