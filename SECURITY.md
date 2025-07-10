# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| 1.0.0   | ✅ Yes    |

---

**This project is a refactored and extended version based on the original SuperClaude project.**

Original Author: [SuperClaude Repository](https://github.com/NomenAK/SuperClaude)

Major refactoring, security enhancements, and ongoing maintenance are provided by the SuperGemini team. For details on changes, see CHANGELOG.md.

---

## Reporting Security Vulnerabilities

We take security seriously. If you discover a security vulnerability, please follow these steps:

### 🔒 Private Reporting (Preferred)

1. **Do NOT** create a public issue
2. Email security details to: <sincerehamill@protonmail.com>
3. Include "SuperGemini Security" in the subject line
4. Provide a detailed description of the vulnerability

### 📝 Required Information

Please include:
- Description of the vulnerability
- Steps to reproduce the issue
- Potential impact assessment
- Any suggested fixes or mitigations
- Your contact information for follow-up

### ⏱️ Response Timeline

- **24 hours**: Initial acknowledgment
- **72 hours**: Preliminary assessment
- **7 days**: Detailed response with next steps
- **30 days**: Resolution target (depending on complexity)

## Security Considerations

### Configuration Framework Security
- SuperGemini is a configuration framework, not executable software
- No network connections or data transmission
- Files are stored locally in ~/.gemini/
- Shell scripts have limited system access
- Template reference system (@pattern) validated for integrity

### Installation Security
- install.sh performs file operations only
- No sudo/admin privileges required
- Backup existing configurations before installation
- All operations within user home directory

### Usage Security
- Configuration files are read-only for Gemini CLI
- No sensitive data stored in configurations
- Slash commands execute through Gemini CLI's security model
- MCP integrations follow Gemini CLI's sandbox restrictions

## Best Practices

### For Users
- Review install.sh before execution
- Keep SuperGemini updated
- Report suspicious behavior
- Use official installation methods only

### For Contributors
- Follow secure coding practices
- No hardcoded secrets or credentials
- Validate all user inputs
- Test security implications of changes

## Scope

This security policy covers:
- SuperGemini configuration files
- Installation scripts
- GitHub repository security
- Community interaction security

## Disclaimer

SuperGemini is provided "as is" without warranty. While we strive for security, users are responsible for:
- Reviewing code before installation
- Using in appropriate environments
- Following Gemini CLI security guidelines
- Backing up existing configurations

---

**Acknowledgement:**
This project is refactored from SuperClaude. We thank the original authors and contributors for their foundational work.

**Questions?** Contact <insert-maintainer-email>

*SuperGemini v1.0.0 | Security-conscious configuration framework*