# Here is my `client`/`.vscode`/`settings.json`!

### settings.json

**USAGE**: Make a folder in the _root_ of the folder you desire to have these settings in called `.vscode`, inside of the folder you will be making a `settings.json` to place these settings in.

```js
{
  "workbench.colorCustomizations": {
    "titleBar.activeForeground": "#000",
    "titleBar.inactiveForeground": "#000000CC",
    "titleBar.activeBackground": "#FFC600",
    "titleBar.inactiveBackground": "#FFC600CC"
  },
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false
  },
  "eslint.alwaysShowStatus": true,
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "prettier.disableLanguages": ["javascript", "javascriptreact"]
}
```
