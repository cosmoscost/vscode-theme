# CosmosCost VSCode Theme

A beautiful color theme for Visual Studio Code that matches the CosmosCost application design system. Features both dark and light variants with a carefully crafted blue-based color palette.

## Features

- **Dark Theme**: Deep dark backgrounds (#0a0a0a) with vibrant blue accents (#3b82f6, #60a5fa)
- **Light Theme**: Clean light backgrounds (#fafaf9) with professional blue tones (#2563eb)
- **Consistent Branding**: Matches the CosmosCost application color system
- **Tailwind-Inspired**: Uses colors from the Tailwind CSS palette for familiarity
- **Semantic Highlighting**: Enhanced code understanding with semantic token support
- **Complete Coverage**: Supports all popular languages and file types
- **Git Integration**: Distinct colors for modified, added, deleted, and untracked files

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

**UI Colors:**
- Editor Background: `#0a0a0a` (Near black)
- Sidebar Background: `#0f172a` (Slate 950)
- Activity Bar: `#0f172a` with `#60a5fa` accents (Blue 400)
- Primary Accent: `#3b82f6` (Blue 500)
- Secondary Accent: `#60a5fa` (Blue 400)

**Syntax Colors:**
- Keywords: `#a78bfa` / `#8b5cf6` (Purple 400/500)
- Strings: `#22c55e` (Green 500)
- Functions: `#60a5fa` (Blue 400)
- Classes/Types: `#06b6d4` (Cyan 500)
- Constants: `#fb923c` (Orange 400)
- Attributes: `#ec4899` (Pink 500)
- Comments: `#64748b` (Slate 500)
- Errors: `#ef4444` (Red 500)
- Warnings: `#f97316` (Orange 500)

**Git Decorations:**
- Modified: `#f97316` (Orange)
- Added: `#22c55e` (Green)
- Deleted: `#ef4444` (Red)
- Untracked: `#22c55e` (Green)

### Light Theme

**UI Colors:**
- Editor Background: `#fafaf9` (Stone 50)
- Sidebar Background: `#f8fafc` (Slate 50)
- Activity Bar: `#f8fafc` with `#2563eb` accents (Blue 600)
- Primary Accent: `#2563eb` (Blue 600)
- Secondary Accent: `#1e40af` (Blue 700)

**Syntax Colors:**
- Keywords: `#7c3aed` / `#6d28d9` (Purple 600/700)
- Strings: `#15803d` (Green 700)
- Functions: `#1e40af` (Blue 700)
- Classes/Types: `#0e7490` (Cyan 700)
- Constants: `#ea580c` (Orange 600)
- Attributes: `#be185d` (Pink 700)
- Comments: `#64748b` (Slate 500)
- Errors: `#dc2626` (Red 600)
- Warnings: `#ea580c` (Orange 600)

**Git Decorations:**
- Modified: `#ea580c` (Orange)
- Added: `#16a34a` (Green)
- Deleted: `#dc2626` (Red)
- Untracked: `#16a34a` (Green)

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
