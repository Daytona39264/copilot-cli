# GitHub Copilot CLI - Development Roadmap

**Last Updated:** November 9, 2025  
**Current Version:** 0.0.347

---

## 🎯 Immediate Priorities (Next 2-4 weeks)

### Performance & Stability
- [ ] Reduce token consumption and API round trips (ongoing optimization)
- [ ] Improve session state persistence for large conversations
- [ ] Fix flickering issues across different terminal emulators
- [ ] Optimize file write performance, especially on Windows

### User Experience
- [ ] Complete multi-line input support for all terminal types
- [ ] Improve `/terminal-setup` wizard for better onboarding
- [ ] Enhanced error messages with actionable troubleshooting steps
- [ ] Add interactive tutorial for first-time users

### Feature Completion
- [ ] Full Kitty protocol support (currently behind feature flag)
- [ ] Complete proxy support for all Node.js versions
- [ ] Expand MCP server marketplace/directory
- [ ] Add session export/import functionality

---

## 📋 Short-term Goals (1-3 months)

### Developer Tools Integration
- [ ] Better integration with popular shells (zsh, bash, fish, PowerShell)
- [ ] Support for tmux and screen sessions
- [ ] Integration with popular CI/CD tools
- [ ] Enhanced git workflow commands

### AI Model Support
- [ ] Add more model options (GPT-4, Gemini, etc.)
- [ ] Model performance comparison tools
- [ ] Custom model fine-tuning support
- [ ] Local model support for offline work

### Collaboration Features
- [ ] Share session transcripts with team members
- [ ] Collaborative debugging sessions
- [ ] Team-wide MCP server configurations
- [ ] Session templates for common workflows

### Documentation & Testing
- [ ] Comprehensive API documentation
- [ ] Unit test coverage > 80%
- [ ] Integration test suite
- [ ] Performance benchmarking framework

---

## 🚀 Long-term Vision (3-6 months)

### Platform Expansion
- [ ] Browser-based terminal for web access
- [ ] Mobile companion app for notifications
- [ ] VS Code extension deep integration
- [ ] JetBrains IDE plugin

### Advanced AI Capabilities
- [ ] Multi-agent workflows
- [ ] Code review automation
- [ ] Security vulnerability detection
- [ ] Performance profiling and optimization suggestions

### Enterprise Features
- [ ] Advanced access controls and permissions
- [ ] Audit logging and compliance reporting
- [ ] Self-hosted deployment options
- [ ] Custom model hosting

### Community & Ecosystem
- [ ] Plugin marketplace
- [ ] Community-contributed MCP servers
- [ ] Open API for third-party integrations
- [ ] Developer certification program

---

## 🐛 Known Issues Being Tracked

### High Priority
- Premium request counting accuracy (v0.0.345-346 fixes deployed)
- Context truncation warnings (addressed in v0.0.334)
- Session state corruption after crashes
- Windows PowerShell profile conflicts

### Medium Priority
- OAuth login hangs in certain SSH environments
- File path extraction edge cases
- Unicode character rendering issues
- Tab completion after certain slash commands

### Low Priority
- Markdown rendering color consistency
- Timeline scrollbar width optimization
- Session history size limits
- Model picker UX improvements

---

## 📊 Success Metrics

### Performance
- **Target:** < 2s average response time
- **Target:** < 50% token reduction from current baseline
- **Target:** 99.9% uptime for API endpoints

### User Satisfaction
- **Target:** 4.5+ star rating
- **Target:** < 5% error rate per session
- **Target:** 80%+ feature adoption rate

### Growth
- **Target:** 100K+ active users by Q2 2026
- **Target:** 1M+ monthly sessions
- **Target:** 500+ community-contributed MCP servers

---

## 🤝 How to Contribute

We welcome contributions! Here's how you can help:

1. **Report Issues:** Use GitHub Issues for bugs and feature requests
2. **Submit PRs:** Check our contribution guidelines
3. **Write Documentation:** Help improve our docs
4. **Share Feedback:** Join discussions in GitHub Discussions
5. **Build MCP Servers:** Extend CLI capabilities

---

## 📅 Release Schedule

- **Weekly:** Bug fixes and minor improvements
- **Bi-weekly:** New features and enhancements
- **Monthly:** Major version updates with breaking changes (if needed)
- **Quarterly:** Platform reviews and roadmap updates

---

## 💡 Feature Requests

Have an idea? We'd love to hear it!

- Open an issue with the `feature-request` label
- Join the discussion in our community forums
- Vote on existing feature requests

---

*This roadmap is subject to change based on user feedback, technical constraints, and business priorities.*

