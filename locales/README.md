# Localization Directory

Multi-language support files for the Monster Hunter Wilds Offline Setup Assistant.

## 🌍 Supported Languages

### Currently Available
- **English (en)** - Default language
- **Japanese (ja)** - 日本語 
- **Chinese Simplified (zh-CN)** - 简体中文
- **Spanish (es)** - Español

### Planned Languages
- **Korean (ko)** - 한국어
- **French (fr)** - Français  
- **German (de)** - Deutsch
- **Portuguese (pt-BR)** - Português (Brasil)

## 📁 File Structure

```
locales/
├── en/
│   ├── common.json          # Common UI elements
│   ├── setup.json           # Setup wizard text
│   ├── training.json        # Training mode strings
│   ├── settings.json        # Settings/configuration
│   └── errors.json          # Error messages
├── ja/
│   ├── common.json
│   ├── setup.json
│   ├── training.json
│   ├── settings.json
│   └── errors.json
├── zh-CN/
│   └── [same structure]
├── es/
│   └── [same structure]
└── template.json            # Template for new languages
```

## 🔧 Translation Format

### JSON Structure
```json
{
  "app": {
    "title": "Monster Hunter Wilds Offline Setup Assistant",
    "version": "Version {version}",
    "description": "Experience Monster Hunter Wilds offline"
  },
  "setup": {
    "welcome": "Welcome to the setup assistant",
    "gameDetection": "Detecting Monster Hunter Wilds installation...",
    "selectPath": "Select Game Installation Path"
  },
  "training": {
    "weapons": {
      "greatSword": "Great Sword",
      "longSword": "Long Sword", 
      "swordShield": "Sword & Shield"
    }
  }
}
```

### Variable Interpolation
```json
{
  "welcome": "Welcome, {playerName}!",
  "progress": "Progress: {current}/{total}",
  "fileSize": "File size: {size} MB"
}
```

### Pluralization Support
```json
{
  "items": {
    "zero": "No items",
    "one": "{count} item", 
    "other": "{count} items"
  }
}
```

## 🎮 Gaming-Specific Terms

### Monster Hunter Terminology
Maintain consistency with official Monster Hunter translations:

**Weapons (English → Japanese → Chinese)**
- Great Sword → 大剣 → 大剑
- Long Sword → 太刀 → 太刀  
- Hammer → ハンマー → 大锤
- Bow → 弓 → 弓

**Monsters**
- Rathalos → リオレウス → 火龙
- Diablos → ディアブロス → 角龙

**Game Mechanics**
- Hunt → 狩猟 → 狩猎
- Carve → 剥ぎ取り → 剥取
- Forge → 生産 → 锻造

## 🔄 Translation Workflow

### For New Translators
1. **Start with template.json** - Copy and rename for your language
2. **Translate common.json first** - Most frequently used strings
3. **Use gaming terminology** - Research official Monster Hunter translations
4. **Test in application** - Verify text fits in UI elements
5. **Submit pull request** - Include sample screenshots

### Translation Guidelines
- **Maintain tone** - Friendly but informative
- **Gaming context** - Use established Monster Hunter terminology
- **UI constraints** - Consider text length in interface elements
- **Cultural adaptation** - Adapt for local gaming culture
- **Technical accuracy** - Ensure technical terms are correct

### Quality Assurance
- **Native speaker review** - Must be reviewed by native speaker
- **Gaming community input** - Feedback from local Monster Hunter players
- **UI testing** - Verify all text displays correctly
- **Functional testing** - Ensure features work in translated version

## 📝 Translation Keys

### Common Categories
- **Navigation**: menu, buttons, tabs
- **Actions**: save, load, cancel, apply
- **Status**: loading, success, error, warning
- **Time**: seconds, minutes, hours, days

### Monster Hunter Specific
- **Weapons**: All 14 weapon type names and descriptions
- **Biomes**: Environment names and descriptions  
- **Settings**: Graphics, audio, control options
- **Training**: Combat moves and techniques

### Technical Terms
- **Graphics**: resolution, framerate, vsync, antialiasing
- **Audio**: volume, effects, music, voice
- **Controls**: keyboard, mouse, gamepad, bindings
- **System**: Windows, macOS, Linux, requirements

## 🌐 Locale-Specific Considerations

### Japanese (ja)
- **Honorifics**: Use appropriate keigo levels
- **Monster Hunter**: Follow official Capcom Japan translations
- **Text Direction**: Left-to-right (standard for games)
- **Character Encoding**: UTF-8 with proper font support

### Chinese Simplified (zh-CN)
- **Regional Terms**: Mainland China gaming terminology
- **Monster Hunter**: Follow official Chinese translations
- **Technical Terms**: Use established PC gaming translations
- **Input Methods**: Consider keyboard layout differences

### Spanish (es)
- **Regional Variant**: Neutral Spanish for broad appeal
- **Gaming Terms**: Use Latin American gaming conventions
- **Formality**: Tu/Usted - use "tú" for gaming context
- **Monster Hunter**: Reference official Spanish translations

## 🔧 Implementation

### Loading Translations
```javascript
const locale = getUserLocale() || 'en';
const translations = await import(`./locales/${locale}/common.json`);
```

### Fallback System
```javascript
function translate(key, locale = 'en') {
  return translations[locale][key] || 
         translations['en'][key] || 
         key;
}
```

### Runtime Language Switching
```javascript
function changeLanguage(newLocale) {
  loadTranslations(newLocale);
  updateUI();
  saveUserPreference(newLocale);
}
```

## 🤝 Contributing Translations

### Getting Started
1. Check [open translation issues](../issues?q=is%3Aissue+is%3Aopen+label%3Atranslation)
2. Join our [Discord translation channel](https://discord.gg/mhwilds-offline)
3. Read the [Contributing Guide](../CONTRIBUTING.md)
4. Review existing translations for consistency

### Translation Tools
- **JSON Editor**: Use VS Code with JSON extensions
- **Validation**: Check JSON syntax before submitting
- **Testing**: Run application with your translations
- **Screenshots**: Provide UI screenshots with translations

### Recognition
- **Credits**: All translators credited in application
- **Community**: Special Discord roles for contributors
- **Updates**: Priority notifications for translation updates
- **Beta Access**: Early access to new features for testing

---

**Thank you for helping make Monster Hunter Wilds accessible to hunters worldwide! 🐲🌍** 