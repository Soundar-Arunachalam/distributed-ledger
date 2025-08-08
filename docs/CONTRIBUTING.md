
---

## **4) CONTRIBUTING.md** (docs)
```markdown
# Contributing Guide

## Workflow
1. Fork the repo and clone locally
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Make changes and commit with a clear message
4. Push to your fork and open a PR to `develop`

## Commit Messages
Use conventional commits:
- `feat: add block validation`
- `fix: resolve transaction signature bug`
- `docs: update architecture diagram`

## Code Style
- TypeScript strict mode
- ESLint + Prettier
- 2-space indentation

## Tests
- Write unit tests for all new code
- Ensure `npm test` passes before PR

## Pull Request Process
- Fill PR template
- Link related issues
- Pass CI checks before merge
