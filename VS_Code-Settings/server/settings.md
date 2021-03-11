# Here is my `server`/`.vscode`/`settings.json`!

### settings.json

**USAGE**: Make a folder in the _root_ of the folder you desire to have these settings in called `.vscode`, inside of the folder you will be making a `settings.json` to place these settings in.

```js
{
  "workbench.colorCustomizations": {
    "titleBar.activeForeground": "#fff",
    "titleBar.inactiveForeground": "#ffffffcc",
    "titleBar.activeBackground": "#FF2C70",
    "titleBar.inactiveBackground": "#FF2C70CC"
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
