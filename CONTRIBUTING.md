# Contributing to Monster Hunter Wilds Offline Setup Assistant

Thank you for your interest in contributing to the Monster Hunter Wilds Offline Setup Assistant! 🎮

## 🎯 Ways to Contribute

### 🐛 Bug Reports
Found a bug? Help us squash it!
- Use the [Bug Report Template](.github/ISSUE_TEMPLATE/bug_report.md)
- Include system specifications (OS, hardware, game version)
- Describe steps to reproduce the issue
- Attach screenshots or error logs if possible

### 💡 Feature Requests
Have an idea for improvement?
- Use the [Feature Request Template](.github/ISSUE_TEMPLATE/feature_request.md)
- Explain the problem your feature would solve
- Describe your proposed solution
- Consider how it fits with the project's offline focus

### 🌍 Translations
Help make the tool accessible worldwide!
- Check existing translations in `/locales/`
- Follow the translation guide in `/docs/translation-guide.md`
- Test translations with the actual interface
- Ensure gaming terminology is accurate

### 📝 Documentation
Improve guides and documentation:
- Setup instructions and troubleshooting
- FAQ updates and user guides
- Video tutorial scripts
- Code documentation and comments

### 🔧 Code Contributions
Technical improvements and new features:
- Bug fixes and performance optimizations
- New launcher features and configuration options
- UI/UX improvements
- Platform compatibility enhancements

## 🚀 Getting Started

### Prerequisites
- Git installed and configured
- Development environment for your contribution type:
  - **Code**: Python 3.8+, Qt6, or web technologies
  - **Documentation**: Markdown editor
  - **Translations**: Text editor with UTF-8 support

### Setting Up Development Environment

1. **Fork the Repository**
   ```bash
   # Fork on GitHub, then clone your fork
   git clone https://github.com/YOUR_USERNAME/monster-hunter-wilds-offline-setup-assistant
   cd monster-hunter-wilds-offline-setup-assistant
   ```

2. **Install Dependencies**
   ```bash
   # Install development dependencies
   pip install -r requirements-dev.txt
   
   # Install pre-commit hooks
   pre-commit install
   ```

3. **Create Feature Branch**
   ```bash
   git checkout -b feature/my-awesome-feature
   # or
   git checkout -b bugfix/fix-launcher-crash
   # or
   git checkout -b docs/update-setup-guide
   ```

## 📋 Development Guidelines

### Code Standards
- **Language**: Python 3.8+ for core functionality
- **Style**: Follow PEP 8 with 88-character line limit
- **Documentation**: Docstrings for all public functions
- **Testing**: Write tests for new functionality

### Commit Message Format
```
type(scope): brief description

Detailed explanation of changes if needed

Fixes #123
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

**Examples:**
```
feat(launcher): add Steam Deck graphics presets

Added optimized graphics presets specifically for Steam Deck:
- Low power mode for extended battery life
- Balanced mode for good performance/battery ratio
- Performance mode for best visuals

Fixes #156
```

### Pull Request Process

1. **Before Submitting**
   - Ensure your code follows the style guidelines
   - Run tests and verify they pass
   - Update documentation if needed
   - Test on multiple platforms if possible

2. **PR Description Template**
   ```markdown
   ## What does this PR do?
   Brief description of changes
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Documentation update
   - [ ] Translation
   
   ## Testing
   - [ ] Tested on Windows
   - [ ] Tested on Linux
   - [ ] Tested on macOS
   - [ ] Added/updated tests
   
   ## Screenshots
   If applicable, add screenshots
   
   ## Checklist
   - [ ] Code follows style guidelines
   - [ ] Self-review completed
   - [ ] Documentation updated
   - [ ] No breaking changes (or clearly noted)
   ```

3. **Review Process**
   - Maintainers will review within 48-72 hours
   - Address feedback promptly
   - Be open to suggestions and improvements
   - Squash commits if requested

## 🎮 Gaming-Specific Guidelines

### User Experience Focus
- **Simplicity**: Gaming tools should be intuitive
- **Performance**: Minimal impact on game performance
- **Compatibility**: Support various game configurations
- **Offline First**: All features must work without internet

### Testing with Real Game
- Test with actual Monster Hunter Wilds installation
- Verify compatibility with different game versions
- Check mod compatibility when possible
- Test various graphics settings and hardware configurations

### Community Feedback
- Engage with Monster Hunter community for feature ideas
- Consider feedback from different types of players (casual, hardcore, speedrunners)
- Respect Capcom's intellectual property and terms of service

## 🛡️ Security Considerations

### Safe Practices
- Never include game files or copyrighted content
- Don't implement game cracks or piracy tools
- Ensure offline tools don't compromise game integrity
- Respect user privacy and data security

### Code Security
- Validate all user inputs
- Use secure file handling practices
- Don't store sensitive information
- Follow secure coding guidelines

## 🎯 Community Standards

### Be Respectful
- Respectful communication in all interactions
- Constructive feedback and suggestions
- Help newcomers and answer questions
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md)

### Gaming Community Values
- Share knowledge about Monster Hunter mechanics
- Help players enjoy the game offline
- Respect different playstyles and preferences
- Contribute to a positive gaming community

## 📞 Getting Help

### Community Support
- 💬 [Discord Server](https://discord.gg/mhwilds-offline) - Real-time help
- 🐛 [GitHub Issues](https://github.com/Hunter-Wilds-Offline-Setup-Assistant/monster-hunter-wilds-offline-setup-assistant/issues) - Bug reports and feature requests
- 📝 [Discussions](https://github.com/Hunter-Wilds-Offline-Setup-Assistant/monster-hunter-wilds-offline-setup-assistant/discussions) - General questions

### Documentation
- 📖 [Setup Guide](docs/setup-guide.md)
- 🔧 [Development Docs](docs/development.md)
- 🌍 [Translation Guide](docs/translation-guide.md)

## 🏆 Recognition

### Contributors Hall of Fame
All contributors are recognized in:
- README.md credits section
- Annual contributor highlights
- Discord special roles
- Community shoutouts

### Contribution Levels
- **🌟 First-time Contributor**: Welcome package and guidance
- **🔥 Regular Contributor**: Special Discord role and early access
- **💎 Core Contributor**: Maintainer consideration and special recognition
- **🏆 Community Champion**: Lifetime recognition for outstanding contributions

---

Thank you for helping make Monster Hunter Wilds more accessible to the offline gaming community! 🐲 