# Contributing Guide

Thank you for your interest in contributing to this project.

## Workflow

- `main`: stable releases
- `develop`: integration branch
- `feature/<name>`: new features
- `hotfix/<name>`: critical fixes

All work should be done in feature branches and merged into `develop`.

## Commit Convention

This project follows Conventional Commits:

- `feat(scope): description`
- `fix(scope): description`
- `chore(scope): description`
- `docs(scope): description`
- `test(scope): description`

Examples:
- `feat(auth): add refresh token rotation`
- `chore(ci): add github actions workflow`

## Pull Requests

- Always open PRs against `develop`
- Keep PRs small and focused
- Describe what was changed and why
