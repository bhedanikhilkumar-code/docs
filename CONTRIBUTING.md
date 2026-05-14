# Contributing to Nexus API Documentation

Thank you for your interest in contributing! This guide will help you get started.

## How to Contribute

### 1. Fork the Repository

Click the **Fork** button on GitHub to create your own copy.

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/docs.git
cd docs
```

### 3. Create a Branch

```bash
git checkout -b feature/your-feature-name
```

### 4. Make Your Changes

Edit the documentation files in the appropriate folders:
- `index.mdx`, `quickstart.mdx` - Home and getting started
- `essentials/*.mdx` - Core concepts and guides
- `api-reference/*.mdx` - API endpoint documentation
- `snippets/*.mdx` - Code examples and SDK docs

### 5. Preview Changes

Install Mintlify CLI and preview locally:

```bash
npm install -g mint
mint dev
```

Visit `http://localhost:3000` to see your changes.

### 6. Commit and Push

```bash
git add .
git commit -m "feat: add documentation for new feature"
git push origin feature/your-feature-name
```

### 7. Create a Pull Request

Open a PR on GitHub with a clear description of your changes.

## Documentation Guidelines

### Content Standards

- **Clear and concise** - Write for developers
- **Code examples** - Include working examples for all endpoints
- **Update navigation** - Add new pages to `docs.json`
- **Test locally** - Verify changes with `mint dev`

### Writing Style

- Use active voice
- Second person ("you")
- Sentence case for headings
- Code formatting for technical terms

### File Structure

```
docs/
├── index.mdx                 # Home page
├── quickstart.mdx           # Quick start guide
├── essentials/              # Core documentation
│   ├── auth.mdx
│   ├── api-keys.mdx
│   └── ...
├── api-reference/           # API endpoints
│   ├── users/
│   ├── projects/
│   └── analytics/
├── snippets/                # Code examples
│   ├── python.mdx
│   ├── javascript.mdx
│   └── curl.mdx
└── agent-ready/             # AI agent features
```

### Frontmatter

Every MDX file needs frontmatter:

```yaml
---
title: Page Title
description: Brief description of the page content
---
```

## Need Help?

- [Discord Community](https://discord.gg/nexus)
- [GitHub Issues](https://github.com/bhedanikhilkumar-code/docs/issues)
- [Email Support](mailto:support@nexus.dev)

## Code of Conduct

Please be respectful and constructive in all interactions. We follow the [Contributor Covenant](https://www.contributor-covenant.org/).