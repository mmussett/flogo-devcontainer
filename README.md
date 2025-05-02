# flogo-devcontainer

## Instructions for using DevContainer for Flogo.


1. Place your downloaded flogo-vscode-linux-x64.vsix file in the .devcontainer/extensions folder.

2. Modify line 18 .devcontainer/devcontainer.json so that the filename of the extension matches your downloaded version

```
 "${containerWorkspaceFolder}/.devcontainer/extensions/flogo-vscode-linux-x64-1.2.0-836.vsix"
```

3. Run the command (CTRL+SHIFT+P) Dev Containers: Rebuild and Reopen in Container command

4. Enjoy Flogo from within your devcontainer!


