# BISICLES Config Syntax Highlighting

A VS Code extension that adds syntax highlighting for [BISICLES](https://davis.lbl.gov/Manuals/BISICLES-DOCS/) input/config files.

The extension activates automatically for files matching `inputs.*` or `*.inputs`. It highlights `#` comments, `@placeholders`, `key = value` assignments, and boolean literals.

## Installation

Building the extension requires [`vsce`](https://github.com/microsoft/vscode-vsce):

```sh
npm install -g @vscode/vsce
# or, on macOS with Homebrew:
brew install vsce
```

### 1. Build the `.vsix`

From the repo root:

```sh
vsce package
```

This produces `bisicles-syntax-<version>.vsix`.

### 2. Install it

**From the command line:**

```sh
code --install-extension bisicles-syntax-<version>.vsix
```

**From the VS Code UI:**

1. Open the Extensions view (`Cmd+Shift+X` / `Ctrl+Shift+X`).
2. Click the `...` menu in the top-right of the Extensions panel.
3. Choose **Install from VSIX...** and select the `.vsix` file you built.

Reload the window and open any `inputs.*` file to see the highlighting.

## License

[MIT](./LICENSE)
