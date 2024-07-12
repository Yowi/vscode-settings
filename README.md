# vscode-settings

> Last updated on 2024-07-09 (VSCode v1.91.0).

## Extensions

The following extensions are recommended for an enhanced development experience in VSCode:

- vscode-ant-design-vue-helper
- vscode-language-pack-zh-hans
- vscode-eslint
- git-graph
- git-commit-plugin
- gitlens
- material-icon-theme
- noctis
- prettier-vscode
- svg
- vue.volar

## Settings (`settings.json`)

Below is the recommended `settings.json` configuration to ensure a consistent and efficient coding environment:

```json
{
  "workbench.colorTheme": "Noctis Uva",
  "workbench.iconTheme": "material-icon-theme",
  "terminal.integrated.tabs.enabled": false,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "window.zoomLevel": 1,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  // Enable format on save for CSS/LESS files.
  "editor.formatOnSave": true,
  // Disable default JS/TS formatter to avoid conflicts with ESLint.
  "javascript.format.enable": false,
  "typescript.format.enable": false,
  // Disable Vetur is formatter for HTML, JS, and TS to prevent conflicts with ESLint and Prettier.
  "vetur.format.defaultFormatter.html": "none",
  "vetur.format.defaultFormatter.js": "none",
  "vetur.format.defaultFormatter.ts": "none",
  // Enable ESLint auto-fix on save for JS, TS, JSX, and TSX files.
  "eslint.format.enable": true,
  "[vue]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
  },
  "[javascript]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
  },
  "[typescript]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
  },
  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "eslint.codeActionsOnSave.mode": "problems",
  "eslint.validate": [
    "vue",
    "typescript",
    "javascript",
    "javascriptreact",
    "typescriptreact"
  ],
  // Associate .json files with JSON with comments (jsonc) for better readability.
  "files.associations": {
    "*.json": "jsonc"
  },
  "editor.tabSize": 2
}
```

### Configuration Overview

Adhering to the specified **extensions** and **settings**, you will achieve automatic code formatting upon saving (⌘ + S). The formatting behavior for different file types is as follows:

- By default, all files are formatted using Prettier.
- In Vue projects, JavaScript, TypeScript, JSX, TSX, and Vue files are formatted using ESLint's save actions.

This configuration ensures code consistency and adherence to best practices, facilitating a streamlined development workflow across the team.

## LICENSE

MIT