# Contributing to GitHub Copilot CLI

Thank you for your interest in contributing to GitHub Copilot CLI! This document provides guidelines and instructions for contributing.

---

## 🌟 Ways to Contribute

### 1. Report Bugs
Found a bug? Help us fix it!

- **Search existing issues** to avoid duplicates
- **Use the bug report template** when creating new issues
- **Include reproduction steps** and system information
- **Attach logs** from `~/.copilot/logs/` if relevant

### 2. Suggest Features
Have an idea for improvement?

- **Check the roadmap** to see if it's already planned
- **Open a feature request** with clear use cases
- **Describe the problem** you're trying to solve
- **Consider implementation** challenges

### 3. Improve Documentation
Documentation is always appreciated!

- **Fix typos** and clarify confusing sections
- **Add examples** for common use cases
- **Translate documentation** to other languages
- **Create tutorials** and guides

### 4. Submit Code
Ready to code? Here's how:

- **Fork the repository**
- **Create a feature branch**
- **Write tests** for your changes
- **Follow coding standards**
- **Submit a pull request**

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** v22 or higher
- **npm** v10 or higher
- **Git** for version control
- **Active Copilot subscription** for testing

### Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/copilot-cli.git
cd copilot-cli

# Install dependencies (when available)
npm install

# Run tests (when available)
npm test

# Build the project (when available)
npm run build
```

---

## 📝 Coding Standards

### Code Style

- **Use TypeScript** for type safety
- **Follow ESLint rules** (when configured)
- **Write meaningful comments** for complex logic
- **Keep functions small** and focused

### Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): brief description

Detailed explanation (optional)

Fixes #123
```

**Types:**
- `feat:` New features
- `fix:` Bug fixes
- `docs:` Documentation changes
- `style:` Code style changes (formatting)
- `refactor:` Code refactoring
- `test:` Adding or updating tests
- `chore:` Maintenance tasks

**Examples:**
```
feat(models): add support for GPT-4 Turbo

docs: update installation instructions for Windows

fix(session): prevent corruption after network interruption
Fixes #351
```

### Pull Request Guidelines

1. **Create a descriptive title** following commit message conventions
2. **Reference related issues** (e.g., "Fixes #123")
3. **Describe your changes** in the PR description
4. **Include test results** or manual testing steps
5. **Update documentation** if needed
6. **Keep PRs focused** - one feature/fix per PR

---

## 🧪 Testing

### Running Tests

```bash
# Run all tests
npm test

# Run specific test suite
npm test -- --grep "session"

# Run with coverage
npm run test:coverage
```

### Writing Tests

- **Test behavior, not implementation**
- **Use descriptive test names**
- **Cover edge cases** and error conditions
- **Mock external dependencies**

Example:
```typescript
describe('Session Management', () => {
  it('should persist session state after interruption', async () => {
    // Arrange
    const session = new Session();
    
    // Act
    await session.interrupt();
    const restored = await Session.restore();
    
    // Assert
    expect(restored.messages).toEqual(session.messages);
  });
});
```

---

## 🐛 Debugging

### Enable Debug Logging

```bash
# Set log level in config
copilot config set log_level debug

# Or use environment variable
export COPILOT_LOG_LEVEL=debug
copilot
```

### Common Issues

**Issue:** Tests failing locally
- Ensure Node.js version matches requirements
- Clear `node_modules` and reinstall
- Check for conflicting global packages

**Issue:** Can't reproduce bug
- Check system information (OS, shell, terminal)
- Review logs in `~/.copilot/logs/`
- Try in a clean environment

---

## 📚 Documentation

### Where to Update Docs

- **README.md** - Installation and quick start
- **ROADMAP.md** - Future plans and features
- **changelog.md** - Version history
- **docs/** - Detailed guides (when available)

### Documentation Style

- **Use clear, concise language**
- **Include code examples**
- **Add screenshots** for UI features
- **Keep it up-to-date** with code changes

---

## 🔍 Code Review Process

### What We Look For

1. **Functionality** - Does it work as intended?
2. **Tests** - Are changes adequately tested?
3. **Code Quality** - Is it maintainable and readable?
4. **Performance** - Does it introduce bottlenecks?
5. **Security** - Are there any vulnerabilities?
6. **Documentation** - Is it properly documented?

### Response Times

- **Initial review:** Within 3-5 business days
- **Follow-up reviews:** Within 2 business days
- **Urgent fixes:** Within 24 hours

---

## 🏆 Recognition

Contributors will be:
- **Listed in release notes** for significant contributions
- **Added to CONTRIBUTORS.md** file
- **Mentioned in social media** announcements
- **Eligible for swag** (if program exists)

---

## 📞 Getting Help

### Where to Ask Questions

- **GitHub Discussions** - General questions and ideas
- **GitHub Issues** - Bug reports and feature requests
- **Discord/Slack** - Real-time chat (if available)
- **Email** - For security issues: security@github.com

### Community Guidelines

- **Be respectful** and inclusive
- **Provide constructive feedback**
- **Help others** when you can
- **Follow the Code of Conduct**

---

## 📜 License

By contributing, you agree that your contributions will be licensed under the same license as the project (see LICENSE.md).

---

## 🙏 Thank You!

Your contributions make GitHub Copilot CLI better for everyone. We appreciate your time and effort!

**Happy Contributing! 🚀**

