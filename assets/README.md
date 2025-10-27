# Assets

This folder contains theme assets.

## Icon Requirements

⚠️ **IMPORTANT**: VS Code extensions only support PNG format for icons. SVG is NOT supported.

The theme icon (`icon.png`) must be:
- **PNG format** (required by VS Code)
- **128x128 pixels** (minimum)
- Square aspect ratio
- Represents the CosmosCost brand

### Current Files

- `cosmoscost-128.svg` - Source SVG (needs conversion)
- `icon.png` - **Required PNG** (convert from SVG)

### Convert SVG to PNG

You need to convert `cosmoscost-128.svg` to `icon.png`:

**Option 1: macOS Preview**
```bash
open assets/images/cosmoscost-128.svg
# File → Export → Format: PNG → Size: 128x128
```

**Option 2: Online Converter**
- https://cloudconvert.com/svg-to-png
- https://svgtopng.com/

**Option 3: Install librsvg (CLI)**
```bash
brew install librsvg
rsvg-convert -w 128 -h 128 assets/images/cosmoscost-128.svg -o assets/images/icon.png
```

### Theme Colors

Use these CosmosCost colors in your icon:
- Purple: `#a277ff`
- Cyan: `#61ffca`
- Orange: `#ffca85`
- Pink: `#f694ff`
- Background: `#15141b`

### Icon Path

The `package.json` references: `./assets/images/icon.png`
