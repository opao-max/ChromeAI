# Contributing

Thanks for your interest in improving this project! This document explains how
to set up a development environment and get your changes merged.

## Development setup

```bash
git clone https://github.com/opao-max/ChromeAI.git
cd ChromeAI
node --version   # requires Node.js 20+
npm install
```

## Workflow

1. Fork the repository and create a branch from `main`:
   `git checkout -b feat/short-description`
2. Make your change, keeping commits focused and using
   [Conventional Commits](https://www.conventionalcommits.org/):
   `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`.
3. Before pushing, run the same checks as CI:

```bash
npm run typecheck
npm run lint
npm test
```

4. Push your branch and open a Pull Request, filling in the PR template.

## Code style

- TypeScript strict mode is required; avoid `any` unless justified.
- Format with Prettier; lint with ESLint (configs are in the repo).
- Add or update unit tests for behavior changes.
- Keep public APIs backward compatible where possible; document breaking
  changes in the PR description and `CHANGELOG.md`.

## Reporting bugs

Please use the Bug Report issue template and include a minimal reproduction.

## License

By contributing, you agree that your contributions will be licensed under the
repository's MIT License.

