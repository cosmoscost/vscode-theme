# CosmosCost VSCode Theme

A beautiful color theme for Visual Studio Code with both dark and light variants.

## Features

- **Dark Theme**: Easy on the eyes with carefully selected colors for long coding sessions
- **Light Theme**: Clean and bright for daytime coding
- **Semantic Highlighting**: Enhanced code understanding with semantic token support
- **Complete Coverage**: Supports all popular languages and file types

## Installation

### From VS Code Marketplace

1. Open VS Code
2. Go to Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for "CosmosCost"
4. Click Install

### From VSIX File (Local Installation)

1. Download the `.vsix` file
2. Open VS Code
3. Go to Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
4. Click on the `...` menu at the top
5. Select "Install from VSIX..."
6. Choose the downloaded `.vsix` file

## Activation

1. Open VS Code
2. Press `Ctrl+K Ctrl+T` (or `Cmd+K Cmd+T` on Mac) to open theme selector
3. Choose either:
   - **CosmosCost Dark**
   - **CosmosCost Light**

Or use Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`):

- Type "Preferences: Color Theme"
- Select your preferred theme

## Customization

You can customize specific colors by adding to your `settings.json`:

```json
{
  "workbench.colorCustomizations": {
    "[CosmosCost Dark]": {
      "editor.background": "#1a1a1a"
    }
  },
  "editor.tokenColorCustomizations": {
    "[CosmosCost Dark]": {
      "comments": "#6a9955"
    }
  }
}
```

## Color Palette

### Dark Theme

- Background: `#1e1e1e`
- Foreground: `#d4d4d4`
- Keywords: `#569cd6`
- Strings: `#ce9178`
- Functions: `#dcdcaa`
- Types: `#4ec9b0`

### Light Theme

- Background: `#ffffff`
- Foreground: `#000000`
- Keywords: `#0000ff`
- Strings: `#a31515`
- Functions: `#795e26`
- Types: `#267f99`

## Development

### Prerequisites

- Node.js and npm
- Visual Studio Code
- `@vscode/vsce` CLI tool

### Setup

```bash
# Clone the repository
git clone <your-repo-url>
cd vscode-theme

# Install vsce globally
npm install -g @vscode/vsce
```

### Testing Locally

1. Press `F5` in VS Code to open a new Extension Development Host window
2. In the new window, select your theme from the theme picker

### Modifying Colors

Edit the theme files in the `themes/` directory:

- `themes/cosmoscost-dark-theme.json` - Dark theme colors
- `themes/cosmoscost-light-theme.json` - Light theme colors

Key sections to modify:

- **`colors`**: Workbench UI colors (editor, sidebar, terminal, etc.)
- **`tokenColors`**: Syntax highlighting colors for code

### Building and Publishing

```bash
# Package the extension
vsce package

# This creates a .vsix file you can install locally or share

# Publish to marketplace (requires publisher account)
vsce publish
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - feel free to use and modify as needed.

## Acknowledgments

Inspired by the VS Code default themes and community feedback.

## Changelog

### 0.0.1

- Initial release
- Dark theme variant
- Light theme variant
- Semantic highlighting support

## Support

If you encounter any issues or have suggestions, please file an issue on the GitHub repository.

## Screenshots

_Add screenshots of your theme in action here_

## Tips for Customization

### Common Modifications

1. **Change Editor Background**:

   ```json
   "editor.background": "#yourcolor"
   ```

2. **Adjust Syntax Colors**:
   Edit the `tokenColors` array and modify the `foreground` values for different scopes.

3. **Modify UI Elements**:
   Common UI color keys:
   - `sideBar.background`
   - `activityBar.background`
   - `statusBar.background`
   - `terminal.background`

### Useful Resources

- [VS Code Theme Color Reference](https://code.visualstudio.com/api/references/theme-color)
- [TextMate Scopes](https://macromates.com/manual/en/language_grammars)
- [Color Theme Guide](https://code.visualstudio.com/api/extension-guides/color-theme)

---

**Enjoy coding with CosmosCost!**
