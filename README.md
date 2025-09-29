# Cursor Rules

Shared Cursor AI rules for development workflows and best practices.

## Overview

This repository contains reusable Cursor AI rules that can be shared across multiple projects. The rules are organized by category and can be selectively used in different projects.

## Structure

```
cursor-rules/
├── README.md
├── web-development/
│   ├── modern-web-development.mdc
│   ├── react-nextjs.mdc
│   ├── typescript.mdc
│   └── tailwind-css.mdc
├── workflows/
│   ├── github-operations.mdc
│   ├── git-branching.mdc
│   └── code-review.mdc
├── languages/
│   ├── python.mdc
│   ├── javascript.mdc
│   └── go.mdc
└── templates/
    ├── bug-report.mdc
    ├── feature-request.mdc
    └── pr-template.mdc
```

## Usage

### Option 1: Git Submodule (Recommended)

1. Add this repository as a submodule to your project:
   ```bash
   git submodule add https://github.com/delwinbest/cursor-rules.git .cursor/rules-shared
   ```

2. Create symlinks to the rules you want to use:
   ```bash
   mkdir -p .cursor/rules
   ln -s ../rules-shared/web-development/modern-web-development.mdc .cursor/rules/
   ln -s ../rules-shared/workflows/github-operations.mdc .cursor/rules/
   ```

### Option 2: Direct Clone

1. Clone the repository into your project:
   ```bash
   git clone https://github.com/delwinbest/cursor-rules.git .cursor/rules-shared
   ```

2. Create symlinks as needed.

## Available Rules

### Web Development
- **modern-web-development.mdc**: Comprehensive rules for modern web development with TypeScript, React, Next.js, Supabase, and more
- **react-nextjs.mdc**: Specific rules for React and Next.js development
- **typescript.mdc**: TypeScript best practices and conventions
- **tailwind-css.mdc**: Tailwind CSS styling guidelines

### Workflows
- **github-operations.mdc**: GitHub workflow, branching strategy, and issue management
- **git-branching.mdc**: Git branching conventions and practices
- **code-review.mdc**: Code review guidelines and checklists

### Languages
- **python.mdc**: Python development best practices
- **javascript.mdc**: JavaScript conventions and patterns
- **go.mdc**: Go language guidelines

### Templates
- **bug-report.mdc**: Bug report templates and guidelines
- **feature-request.mdc**: Feature request templates
- **pr-template.mdc**: Pull request templates

## Contributing

1. Fork this repository
2. Create a feature branch
3. Add or modify rules
4. Test with your projects
5. Submit a pull request

## License

MIT License - feel free to use and modify for your projects.
