# Architecture

## Current Architecture

The extension starts with a command registered in `src/extension.ts`.

```mermaid
flowchart TD
    A[VS Code Extension Host] --> B[activate]
    B --> C[Register command]
    C --> D[texWiki.generateWiki]
    D --> E[Read active workspace]
    E --> F[Create output folder]
    F --> G[Write Markdown file]
    G --> H[Open generated file]
```

## Planned Architecture

Future implementation should separate the extension into clear modules.

```mermaid
flowchart TD
    A[Command Handler] --> B[Workspace Scanner]
    B --> C[Project Analyzer]
    C --> D[Wiki Model]
    D --> E[Markdown Renderer]
    D --> F[Mermaid Renderer]
    E --> G[File Writer]
    F --> G
    G --> H[Generated Wiki]
```

## Suggested Source Structure

```text
src/
  extension.ts
  commands/
    generateWikiCommand.ts
  scanner/
    workspaceScanner.ts
    ignoreRules.ts
  wiki/
    wikiModel.ts
    markdownRenderer.ts
    mermaidRenderer.ts
  filesystem/
    wikiWriter.ts
```
