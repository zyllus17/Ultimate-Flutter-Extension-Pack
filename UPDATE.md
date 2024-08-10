# Update Extension

Follow these instructions if you want to update the extension pack.

1. Make sure you have npm installed. Run ` npm -v` to check the version installed.
2. Run this command and download vsce `npm install -g @vscode/vsce`
3. Make sure your directory is in the project folder. Eg it should be something like `F:\Flutter projects\Ultimate-Flutter-Extension-Pack>`
4. Make the change in [package.json](package.json) regarding the changes in the extensions you want in the extension pack and make sure to update the `version`
5. Update the changes in [README.md](README.md) & [CHANGELOG.md](CHANGELOG.md)
6. Run `vsce package` in the terminal.
7. If you get the error `File C:\Users\..\.. cannot be loaded because running scripts is disabled on this system.` then run this command in the terminal to give permission - `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`
8. Run `vsce package` in the terminal again.
9. Your file will be generated in root directory named `flutter-0.0.{Version no. in your package.json}`. Move this file to `version` folder.
10. Drop the newly created .vsix file in [VSCode MarketPlace](https://marketplace.visualstudio.com/manage/publishers/marufhassan) by clicking the three dots on the extension and selecting Update option.
11. Push the changes in Github.
