# Development Workflow

## Local Development

Install dependencies:

```bash
npm install
```

Compile:

```bash
npm run compile
```

Run extension:

```text
Press F5 in VS Code
```

## Git Workflow

Recommended flow:

```bash
git status --short --branch
git add .
git commit -m "Describe the change"
git push
```

## Quality Gates

Before each push:

- Run `npm run compile`.
- Check generated documentation links.
- Keep the README and docs index updated.
- Avoid committing generated build output such as `dist/`.

## Development Loop

```mermaid
flowchart LR
    A[Plan feature] --> B[Implement]
    B --> C[Compile]
    C --> D[Test in Extension Host]
    D --> E[Update docs]
    E --> F[Commit and push]
```
