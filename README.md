# Tex Wiki

Tex Wiki is a VS Code extension that will generate a detailed project wiki from the directory currently open in VS Code.

GitHub repository convention:

- Local folder: `tex-wiki`
- GitHub repository: `vscode-ext-tex-wiki`

## Current Stage

This is the minimal starting point of the project.

Available command:

- `Tex Wiki: Generate Wiki`

The command creates a `tex-wiki/README.md` file in the active workspace with an initial wiki outline and a Mermaid flow diagram.

## Development Setup

Requirements:

- Node.js
- npm
- Visual Studio Code
- TypeScript knowledge
- Basic understanding of the VS Code Extension API

Install dependencies:

```bash
npm install
```

Compile:

```bash
npm run compile
```

Run locally:

1. Open this folder in VS Code.
2. Press `F5`.
3. In the Extension Development Host window, open a folder.
4. Run `Tex Wiki: Generate Wiki` from the Command Palette.

## Stack

- TypeScript
- Node.js
- npm
- VS Code Extension API
- Mermaid diagrams
- Markdown
- VSCE, later, for packaging and publishing

## Learning Path

1. TypeScript fundamentals.
2. Node.js project structure and npm scripts.
3. VS Code commands and activation events.
4. File system access through the VS Code Extension API.
5. Markdown generation.
6. Mermaid diagram generation.
7. Extension packaging with `@vscode/vsce`.
8. Marketplace publishing workflow.

## Roadmap

- Generate wiki pages from the workspace directory tree.
- Add configurable ignore patterns.
- Detect project stack automatically.
- Generate architecture pages.
- Generate Mermaid diagrams for dependency and execution flows.
- Package the extension as `.vsix`.
- Publish to the Visual Studio Marketplace.
