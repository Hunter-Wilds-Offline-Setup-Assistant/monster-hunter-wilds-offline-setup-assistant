# Assets Directory

This directory contains all visual assets and media files for the Monster Hunter Wilds Offline Setup Assistant.

## 📁 Directory Structure

### `icons/`
Application icons and UI elements:
- `app-icon.png` - Main application icon (512x512)
- `app-icon.ico` - Windows icon format
- `app-icon.icns` - macOS icon format  
- `tray-icon.png` - System tray icon (32x32)
- `logo.png` - Project logo (256x256)

### `screenshots/`
Interface and gameplay screenshots:
- `setup-interface.png` - Main configuration screen
- `training-mode.png` - Training mode interface
- `config-manager.png` - Graphics configuration panel
- `biome-exploration.png` - Biome preview screens
- `controller-setup.png` - Input configuration interface

### `banners/`
Marketing and social media assets:
- `mh-wilds-banner.gif` - Animated banner for README
- `mh-wilds-social-preview.png` - Social media preview (1200x630)
- `github-header.png` - Repository header image
- `download-banner.png` - Download section graphics

### `ui/`
User interface elements:
- `buttons/` - Button assets and states
- `backgrounds/` - Interface backgrounds
- `cursors/` - Custom cursor assets
- `themes/` - UI theme resources

## 🎨 Asset Guidelines

### Image Requirements
- **Format**: PNG preferred for UI elements, JPG for photos
- **Resolution**: High-DPI ready (2x versions when applicable)
- **Compression**: Optimized for web delivery
- **Color Space**: sRGB color profile

### Icon Specifications
- **App Icon**: 512x512 base resolution with lower resolutions generated
- **Favicon**: 32x32, 16x16 versions included
- **Platform Icons**: Native formats for Windows (.ico), macOS (.icns)

### Screenshot Standards
- **Resolution**: Minimum 1920x1080 for desktop screenshots
- **Format**: PNG for UI screenshots, JPG for gameplay
- **Annotations**: Use consistent highlight colors and fonts
- **Privacy**: No personal information visible

### Social Media Assets
- **Twitter Cards**: 1200x675 aspect ratio
- **OpenGraph**: 1200x630 aspect ratio  
- **GitHub Social Preview**: 1280x640 aspect ratio
- **Discord Embeds**: 16:9 aspect ratio recommended

## 🔗 Usage in Documentation

### README.md References
```markdown
![Monster Hunter Wilds Setup](assets/screenshots/setup-interface.png)
*Main configuration interface*
```

### GitHub Pages Integration
```yaml
og:image: /assets/mh-wilds-social-preview.png
twitter:image: /assets/mh-wilds-social-preview.png
```

### Application Resources
```python
ICON_PATH = "assets/icons/app-icon.png"
LOGO_PATH = "assets/icons/logo.png"
```

## 📝 Attribution

### Monster Hunter Wilds Content
- **Game Images**: Fair use for educational/informational purposes
- **Capcom Trademarks**: Properly attributed and not claiming ownership
- **Screenshot Guidelines**: No copyrighted music or inappropriate content

### Original Content
- **UI Screenshots**: Created by the development team
- **Application Icons**: Original designs or properly licensed
- **Logos**: Community-created assets with clear licensing

## 🚫 Excluded Content

Do not include in this repository:
- Copyrighted game files or assets
- Extracted game textures or models
- Licensed music or sound effects
- Personal screenshots with identifying information
- Proprietary Capcom intellectual property

## 🔄 Asset Management

### Adding New Assets
1. Follow naming conventions (lowercase, hyphenated)
2. Optimize file sizes for web delivery
3. Include multiple resolutions where appropriate
4. Update this README with new asset descriptions

### Version Control
- Use Git LFS for large binary files (>1MB)
- Compress images appropriately before committing
- Include alt-text descriptions in documentation
- Tag releases with asset version information

---

**Note**: All assets should comply with fair use guidelines and respect Capcom's intellectual property rights. 