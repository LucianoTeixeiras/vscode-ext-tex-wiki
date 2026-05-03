# 01 - Development Environment

## Required Tools

- Visual Studio Code
- Node.js
- npm
- Git
- GitHub CLI
- TypeScript

## Current Project Stack

- Runtime: Node.js
- Language: TypeScript
- Editor platform: VS Code Extension API
- Documentation format: Markdown
- Diagram format: Mermaid
- Package manager: npm
- Repository host: GitHub

## Useful Commands

Install dependencies:

```bash
npm install
```

Compile the extension:

```bash
npm run compile
```

Run the extension locally:

```text
Press F5 in VS Code
```

Check Git status:

```bash
git status --short --branch
```

## Local Workspace Convention

The parent folder stores multiple extension projects:

```text
vscode-ext/
  tex-wiki/
  another-extension/
```

Each extension folder is an independent Git repository.

GitHub repositories use the `vscode-ext-*` prefix:

```text
vscode-ext-tex-wiki
```
