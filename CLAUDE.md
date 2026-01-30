# CLAUDE.md - AI Assistant Guide for MyWebsite

This document provides essential context and guidelines for AI assistants working on this repository.

## Project Overview

**Project Name**: MyWebsite
**Repository Owner**: cgcuevas
**Status**: Initial setup (greenfield project)
**Purpose**: Personal website project

This is a newly initialized repository ready for development. The project currently contains only the basic Git structure and a minimal README.

## Current Repository State

```
MyWebsite/
├── .git/           # Git repository metadata
├── CLAUDE.md       # This file - AI assistant guidelines
└── README.md       # Project readme (minimal)
```

### What Exists
- Git repository initialized
- Basic README.md with project title
- Feature branch structure for Claude development

### What Needs to Be Created
- Project source code (HTML, CSS, JavaScript, or chosen framework)
- Configuration files (.gitignore, package.json, etc.)
- Build/development tooling
- Testing infrastructure
- Documentation

## Development Guidelines

### Git Workflow

1. **Branch Naming**: Use descriptive branch names
   - Feature branches: `feature/<feature-name>`
   - Bug fixes: `fix/<issue-description>`
   - Claude AI branches: `claude/<identifier>`

2. **Commit Messages**: Follow conventional commits format
   ```
   type(scope): description

   [optional body]
   ```
   Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

3. **Before Committing**:
   - Ensure code is properly formatted
   - Verify no sensitive data (API keys, credentials) is included
   - Test changes locally when possible

### Code Conventions (To Be Established)

When adding code to this project, follow these principles:

1. **File Organization**:
   - Keep related files together
   - Use clear, descriptive file names
   - Separate concerns (HTML structure, CSS styling, JS behavior)

2. **Code Style**:
   - Use consistent indentation (recommend 2 spaces)
   - Add comments for complex logic
   - Keep functions small and focused

3. **Naming Conventions**:
   - Use descriptive variable and function names
   - Follow language-specific conventions (camelCase for JS, kebab-case for CSS classes)

## Common Tasks

### Starting Fresh Development

Since this is a new project, typical first steps include:

1. **Choose a technology stack** (static HTML, React, Vue, etc.)
2. **Initialize package management** if using Node.js:
   ```bash
   npm init -y
   ```
3. **Create .gitignore** for the chosen stack
4. **Set up basic project structure**

### Adding a Static Website

```bash
# Create basic structure
mkdir -p src/{css,js,images}
touch src/index.html src/css/styles.css src/js/main.js
```

### Adding a Node.js/Framework Project

```bash
# Initialize Node.js project
npm init -y

# Add development dependencies (example)
npm install --save-dev vite

# Create source directory
mkdir src
```

## Important Reminders for AI Assistants

1. **Read Before Modifying**: Always read existing files before making changes
2. **Minimal Changes**: Make only necessary changes; avoid over-engineering
3. **Security First**: Never commit sensitive data (credentials, API keys, tokens)
4. **Test Changes**: Verify changes work before committing when possible
5. **Clear Communication**: Explain what changes are being made and why
6. **Respect Existing Patterns**: Follow any conventions already established in the codebase

## Files to Never Commit

When development begins, ensure these are added to `.gitignore`:

```
# Dependencies
node_modules/

# Environment variables
.env
.env.local
.env.*.local

# Build outputs
dist/
build/

# IDE/Editor files
.idea/
.vscode/
*.swp
*.swo
.DS_Store

# Logs
*.log
npm-debug.log*

# Credentials (NEVER commit these)
*.pem
*.key
credentials.json
secrets.json
```

## Getting Help

- Check existing documentation in the repository
- Review commit history for context on past changes
- Consult framework/library documentation for technical questions

## Project Evolution

As this project grows, update this CLAUDE.md file to reflect:
- New directory structures
- Added dependencies and their purposes
- Build and deployment processes
- Testing procedures
- Any project-specific conventions

---

*Last updated: 2026-01-30*
*Repository initialized: 2022-09-28*
