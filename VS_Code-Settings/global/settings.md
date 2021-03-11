# Here is my global `settings.json` & extensions!

## Extensions:

- Apollo GrapghQL
- Auto Rename Tag
- Better Comments
- Better TOML
- Bracket Pair Colorizer
- Cobalt2 Theme Offical
- Code Spell Checker
- Color Highlight
- Docker
- DotENV
- ES7 React/Redux/GraphQL/React-Native snippets
- ESLint
- GraphQL
- Handlebars
- Javascript (ES6) code snippets
- Jest
- Kite AutoComplete AI Code
- Material Icon Theme
- open in browser
- Prettier
- open in browser
- Prettier - Code Formatter
- Prisma
- Remote - WSL
- SQL Server (mssql)
- TODO Highlight
- Toggle Format on Save
- vscode-styled-components

## settings.json

**USAGE**: To access your global VS Code settings you can open the command pallette (`Ctrl+Shift+P` or Look in the "View" option in the Toolbar & search for "Preferences: Open Settings (JSON)")

```js
{
  "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
  "workbench.iconTheme": "material-icon-theme",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "emmet.excludeLanguages": ["markdown"],
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "workbench.colorTheme": "Cobalt2",
  "editor.fontFamily": "Operator Mono, Menlo, Monaco, 'Courier New', monospace",
  "editor.fontSize": 17,
  "editor.lineHeight": 25,
  "editor.letterSpacing": 0.5,
  "files.trimTrailingWhitespace": true,
  "editor.linkedEditing": true,
  "editor.fontWeight": "400",
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.cursorStyle": "line",
  "editor.cursorWidth": 5,
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
  "prettier.disableLanguages": ["javascript", "javascriptreact"],
  "mssql.connections": [
    {
      "server": "localhost:3306",
      "database": "VS-DB",
      "user": "root",
      "password": "password"
    }
  ],
  "kite.showWelcomeNotificationOnStartup": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "window.zoomLevel": -1
}
```
