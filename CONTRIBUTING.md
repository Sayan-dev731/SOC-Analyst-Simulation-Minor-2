# 🤝 Contributing to SOC Analyst Simulation

First off, thank you for considering contributing to this project! 🎉

This project is an educational simulation focused on network traffic analysis and SOC operations. Whether you're fixing bugs, improving documentation, or adding new features, your contributions are welcome!

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Process](#development-process)
- [Submission Guidelines](#submission-guidelines)
- [Style Guidelines](#style-guidelines)
- [Community](#community)

---

## 📜 Code of Conduct

This project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainer.

---

## 🎯 How Can I Contribute?

### 🐛 Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title** - Descriptive summary of the issue
- **Description** - Detailed explanation of the problem
- **Steps to reproduce** - List of steps to recreate the bug
- **Expected behavior** - What you expected to happen
- **Actual behavior** - What actually happened
- **Screenshots** - If applicable
- **Environment** - OS, Wireshark version, etc.

**Template:**

```markdown
**Bug Description:**
[Clear description of the bug]

**Steps to Reproduce:**
1. Step one
2. Step two
3. ...

**Expected Behavior:**
[What should happen]

**Actual Behavior:**
[What actually happens]

**Environment:**
- OS: [e.g., Windows 11]
- Wireshark Version: [e.g., 4.0.3]
- Additional context: [any other relevant information]
```

### 💡 Suggesting Enhancements

Enhancement suggestions are welcome! Please provide:

- **Clear title** - Concise summary of the enhancement
- **Detailed description** - Explain the feature and its benefits
- **Use case** - Describe scenarios where this would be useful
- **Possible implementation** - If you have ideas on how to implement it
- **Alternatives considered** - Other approaches you've thought about

### 📝 Improving Documentation

Documentation improvements are always appreciated! You can help by:

- Fixing typos or grammatical errors
- Adding more detailed explanations
- Creating tutorials or guides
- Improving existing examples
- Translating documentation
- Adding more screenshots or diagrams

### 🔬 Adding New Analysis Techniques

If you have new investigation techniques or analysis methods:

1. Ensure they are relevant to SOC operations
2. Provide clear documentation
3. Include step-by-step instructions
4. Add screenshots if applicable
5. Explain the value it adds

### 📸 Contributing Screenshots

High-quality screenshots are essential for this project:

- Use clear, high-resolution images
- Highlight important elements
- Add descriptive captions
- Ensure no sensitive information is visible
- Use consistent naming conventions
- Optimize file sizes

---

## 🚀 Getting Started

### Prerequisites

- Git installed on your system
- Wireshark (latest version recommended)
- Basic understanding of network protocols
- Familiarity with PCAP analysis

### Setting Up Development Environment

1. **Fork the repository**
   ```bash
   # Click the 'Fork' button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/SOC-Analyst-Simulation-Minor-2.git
   cd SOC-Analyst-Simulation-Minor-2
   ```

3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/Rakhikumari006/SOC-Analyst-Simulation-Minor-2.git
   ```

4. **Verify remotes**
   ```bash
   git remote -v
   ```

---

## 🔄 Development Process

### Branching Strategy

We follow a simple branching model:

- `main` - Stable, production-ready code
- `feature/feature-name` - New features
- `bugfix/bug-description` - Bug fixes
- `docs/documentation-update` - Documentation changes
- `enhancement/improvement-name` - Enhancements

### Creating a Branch

```bash
# Update your local main branch
git checkout main
git pull upstream main

# Create and switch to a new branch
git checkout -b feature/your-feature-name
```

### Making Changes

1. **Make your changes** in your feature branch
2. **Test thoroughly** - Ensure nothing is broken
3. **Commit regularly** with clear messages
4. **Keep commits atomic** - One logical change per commit

### Commit Message Guidelines

Write clear, descriptive commit messages:

**Format:**
```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Formatting, missing semicolons, etc.
- `refactor:` - Code restructuring
- `test:` - Adding tests
- `chore:` - Maintenance tasks

**Examples:**
```bash
feat(analysis): Add new TCP stream analysis technique

docs(readme): Update installation instructions

fix(screenshots): Correct image path references

style(markdown): Improve formatting and consistency
```

### Keeping Your Fork Updated

```bash
# Fetch upstream changes
git fetch upstream

# Merge upstream changes into your local main
git checkout main
git merge upstream/main

# Update your feature branch
git checkout feature/your-feature-name
git rebase main
```

---

## 📤 Submission Guidelines

### Pull Request Process

1. **Ensure your code is up to date**
   ```bash
   git checkout main
   git pull upstream main
   git checkout feature/your-feature-name
   git rebase main
   ```

2. **Push your changes**
   ```bash
   git push origin feature/your-feature-name
   ```

3. **Create Pull Request**
   - Go to your fork on GitHub
   - Click "Pull Request" button
   - Select your feature branch
   - Fill out the PR template

### Pull Request Template

```markdown
## Description
[Provide a clear description of your changes]

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Enhancement
- [ ] Other (please describe)

## Related Issue
Fixes #[issue-number]

## Changes Made
- [List specific changes]
- [Be detailed and clear]

## Screenshots (if applicable)
[Add screenshots to demonstrate changes]

## Testing
- [ ] I have tested these changes
- [ ] No existing functionality is broken
- [ ] Documentation has been updated

## Checklist
- [ ] My code follows the style guidelines
- [ ] I have performed a self-review
- [ ] I have commented my code where necessary
- [ ] I have updated the documentation
- [ ] My changes generate no new warnings
- [ ] I have checked for typos and grammatical errors
```

### Review Process

- Maintainers will review your PR
- They may request changes or ask questions
- Be responsive to feedback
- Once approved, your PR will be merged

---

## 🎨 Style Guidelines

### Documentation Style

- **Use clear, concise language**
- **Include examples** where helpful
- **Add screenshots** for visual clarity
- **Use proper markdown formatting**
- **Check spelling and grammar**
- **Use emojis sparingly** for visual organization

### Markdown Formatting

```markdown
# H1 for main titles
## H2 for sections
### H3 for subsections

**Bold** for emphasis
*Italic* for technical terms
`code` for commands and file names

- Bullet points for lists
1. Numbered lists for steps

> Blockquotes for important notes

```code blocks for commands```
```

### Screenshot Guidelines

- **Format:** JPEG or PNG
- **Resolution:** Minimum 1280x720
- **Size:** Optimize to keep under 500KB
- **Naming:** Descriptive names (e.g., `tcp-stream-analysis.jpeg`)
- **Content:** Ensure no sensitive data is visible
- **Annotations:** Add arrows or highlights if needed

### File Organization

```
screenshots/
  ├── analysis/
  │   ├── initial-pcap-load.jpeg
  │   └── protocol-hierarchy.jpeg
  ├── investigation/
  │   └── tcp-stream-follow.jpeg
  └── results/
      └── flag-extraction.jpeg
```

---

## 💬 Community

### Communication Channels

- **GitHub Issues** - Bug reports and feature requests
- **Pull Requests** - Code contributions and discussions
- **Discussions** - General questions and conversations

### Getting Help

If you need help:

1. Check existing documentation
2. Search closed issues
3. Ask in GitHub Discussions
4. Create a new issue with the `question` label

### Recognition

All contributors will be acknowledged! Contributors will be:

- Listed in the project documentation
- Mentioned in release notes
- Credited in relevant sections

---

## 🏆 Recognition

### Contributors

We appreciate all contributions, big or small! 

**Want to see your name here?** Make a contribution! 🌟

---

## ❓ Questions?

If you have questions not covered in this guide, feel free to:

- Open an issue with the `question` label
- Start a discussion in GitHub Discussions
- Reach out to the maintainer

---

## 📚 Additional Resources

- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [How to Write Good Commit Messages](https://chris.beams.io/posts/git-commit/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Wireshark Documentation](https://www.wireshark.org/docs/)

---

<div align="center">

**Thank you for contributing! 🎉**

Every contribution makes this project better for the cybersecurity learning community.

[⬆ Back to Top](#-contributing-to-soc-analyst-simulation)

</div>
