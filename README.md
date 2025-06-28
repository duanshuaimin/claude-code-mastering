# Mastering Claude Code
## The Revolution in AI Pair Programming

**Author**: Minho Hwang (robin.hwang@kakaocorp.com)
**Publication Date**: June 2025

This is a complete guide to Claude Code, written in English.

## 📚 Book Structure

### 🏗️ Basics (Chapters 1-3)
- **Chapter 1**: What is Claude Code?
- **Chapter 2**: Installation and Initial Setup
- **Chapter 3**: Mastering Basic Usage

### ⚙️ Configuration (Chapters 4-6)
- **Chapter 4**: Customizing Projects with CLAUDE.md
- **Chapter 5**: Best Practices for Each Framework
- **Chapter 6**: Utilization Strategies for Each Language

### 🚀 Advanced (Chapters 7-9)
- **Chapter 7**: Efficient Development Workflow
- **Chapter 8**: Multitasking and Parallel Processing
- **Chapter 9**: Automation and CI/CD Integration

### 💼 Practical Application (Chapter 10)
- **Chapter 10**: Building a Web Application (Real-world Project)

### 👥 Team Collaboration (Chapters 11-13)
- **Chapter 11**: GitHub Actions and Claude Code Action
- **Chapter 12**: Utilizing Claude Code in a Team
- **Chapter 13**: Case Studies of Claude Code Usage by Organization

### 📖 Conclusion
- **Conclusion**: The Future of Development with AI

## 📁 File Structure

```
claude-code-mastering/
├── 📄 README.md                              # This file
├── 📁 docs/                                  # GitHub Pages deployment files
│   ├── 📄 index.html                         # GitHub Pages main page
│   ├── 📄 claude-code-mastering-complete.html  # Complete book HTML
│   ├── 📄 claude-code-mastering-complete.md    # Combined Markdown
│   ├── 📄 claude-code-mastering-complete.pdf   # Complete book PDF
│   └── 📄 style.css                          # HTML/PDF styles
├── 📁 book/                                  # Completed book content (Markdown)
│   ├── 📄 00-preface.md                      # Preface
│   ├── 📄 01-chapter1.md                     # Chapter 1: What is Claude Code?
│   ├── 📄 02-chapter2.md                     # Chapter 2: Installation and Initial Setup
│   ├── 📄 03-chapter3.md                     # Chapter 3: Mastering Basic Usage
│   ├── 📄 04-chapter4.md                     # Chapter 4: Customizing Projects with CLAUDE.md
│   ├── 📄 05-chapter5.md                     # Chapter 5: Best Practices for Each Framework
│   ├── 📄 06-chapter6.md                     # Chapter 6: Utilization Strategies for Each Language
│   ├── 📄 07-chapter7.md                     # Chapter 7: Efficient Development Workflow
│   ├── 📄 08-chapter8.md                     # Chapter 8: Multitasking and Parallel Processing
│   ├── 📄 09-chapter9.md                     # Chapter 9: Automation and CI/CD Integration
│   ├── 📄 10-chapter10.md                    # Chapter 10: Building a Web Application
│   ├── 📄 11-chapter11.md                    # Chapter 11: GitHub Actions and Claude Code Action
│   ├── 📄 12-chapter12.md                    # Chapter 12: Utilizing Claude Code in a Team
│   ├── 📄 13-chapter13.md                    # Chapter 13: Case Studies of Claude Code Usage by Organization
│   └── 📄 99-conclusion.md                   # Conclusion: The Future of Development with AI
├── 📁 scripts/                               # Conversion scripts
│   ├── 🔧 create-complete-book.sh            # Script to create the complete book
│   ├── 🔧 html-to-pdf.js                     # HTML→PDF conversion tool
│   ├── 🔧 enhanced-pdf-generator.js          # Advanced PDF generator
│   └── 🔧 check-pdf-pages.js                 # PDF page verification tool
├── 📁 raw/                                   # Original materials and drafts
│   ├── 📄 claude-code-action.md              # Claude Code Action guide
│   ├── 📄 claude-code-best-practices-en.md   # Original best practices (English)
│   ├── 📄 claude-code-book-outline.md        # Book outline
│   └── 📄 usecase.md                         # Use case drafts
```

## 🚀 Quick Start

### 📖 Reading

**Read Online**
- [📄 Read on GitHub Pages](https://revfactory.github.io/claude-code-mastering/) - Complete HTML version (includes Mermaid diagrams)
- [📖 Individual Chapter Markdown](book/) - Read on GitHub

**Read by Downloading**
- [📄 Complete Book PDF](docs/claude-code-mastering-complete.pdf) - For offline reading
- [📄 Complete Book HTML](docs/claude-code-mastering-complete.html) - Local HTML version

### 🔧 Book Generation

**Requirements**
```bash
# macOS/Linux
brew install pandoc node

# Or use system package manager
# Ubuntu: sudo apt install pandoc nodejs npm
# CentOS: sudo yum install pandoc nodejs npm

# Install Puppeteer for PDF generation (if needed)
npm install puppeteer
```

**Usage**
```bash
# 1. Grant execution permission
chmod +x scripts/create-complete-book.sh

# 2. Generate complete book (HTML + PDF)
./scripts/create-complete-book.sh

# 3. Check generated files
# - docs/claude-code-mastering-complete.html  (Complete book HTML)
# - docs/claude-code-mastering-complete.pdf   (Complete book PDF)
# - docs/claude-code-mastering-complete.md    (Combined Markdown)
# - docs/index.html (For GitHub Pages - auto-updated)
```

**Notes**
- PDF generation requires Puppeteer (`npm install puppeteer`)
- To generate HTML only, comment out the PDF generation part in the script
- Mermaid diagrams render correctly only in HTML

## 🎯 Key Features

- ✅ **Complete English Support** - Tailored guide for English-speaking developers
- ✅ **Practical Content** - Real-world examples applicable immediately
- ✅ **Step-by-Step Learning** - Structured composition from beginner to advanced
- ✅ **Team Collaboration Guide** - Utilization beyond individual use, at the team level
- ✅ **Reflects Latest Technology** - Includes latest development trends as of 2025
- ✅ **Supports Various Formats** - Provides Markdown, HTML, PDF
- ✅ **Mermaid Diagrams** - Rich diagrams to aid visual understanding
- ✅ **GitHub Pages Support** - Read directly online

## 🤝 Contributing

This project is open source! Contributions are welcome.

**How to Contribute**

1. 📝 Register an Issue if you find typos or areas for improvement
2. 🔀 Propose direct modifications via Pull Request
3. 🌟 Support the project by starring it
4. 📢 Share with fellow developers

## 📄 Copyright and License

**© 2025 Minho Hwang (robin.hwang@kakaocorp.com). All rights reserved.**

**Unauthorized Distribution Prohibited**: Unauthorized reproduction, distribution, transmission, or publication of this work is prohibited by copyright law.

**Permitted Scope**
- ✅ Viewing for personal learning and research purposes
- ✅ Citation for non-commercial educational purposes (with source attribution)
- ✅ Reporting typos and suggesting improvements via GitHub Issues

**Prohibited Actions**
- ❌ Commercial use, reproduction, or distribution
- ❌ Creation of derivative works without author's consent
- ❌ Unauthorized reprinting of all or part of the content

## 🙏 Acknowledgements

- **Anthropic**: Development and support of Claude Code
- **Development Community**: Feedback and ideas
- **Open Source Tools**: Pandoc, Puppeteer, Mermaid.js, etc.

---

**Happy AI Developing!** 🤖💻

> "AI is not a tool to replace developers, but a tool to expand their capabilities."