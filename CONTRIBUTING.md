# Contributing to AscensRun repositories

Thanks for considering a contribution. This document covers the standards that apply across all 13 AscensRun repositories.

## Workflow

1. Fork or branch from `develop`
2. Create a feature branch named `feature/<short-description>`, `fix/<short-description>`, or `chore/<short-description>`
3. Run the local quality gates before pushing:
   - `yamllint --strict .`
   - `ansible-lint --profile=production`
   - `detect-secrets scan --baseline .secrets.baseline`
   - `pre-commit run --all-files`
4. Open a pull request targeting `develop`
5. Continuous integration must pass (yamllint, ansible-lint, detect-secrets, security scan, Molecule)
6. At least one approving review is required before merge

## Commit messages

Conventional Commits format. Allowed types:

- `feat:` new feature
- `fix:` bug fix
- `chore:` housekeeping that does not change behavior
- `docs:` documentation only
- `refactor:` code change that neither fixes a bug nor adds a feature
- `test:` adding or fixing tests
- `ci:` CI configuration changes

Keep commits atomic. Write the message in English. Explain the why, not just the what.

## Code style

- All output in English: code, comments, docs, commits, branches
- Quote shell variables, set `set -euo pipefail` at the top of bash scripts
- Pin Docker base images and GitHub Actions to specific versions or SHAs
- Do not commit secrets, tokens, or unencrypted credentials
- Encrypt all secrets through Ansible Vault and reference them via `vault_*` variable names

## Reporting issues

Open an issue on the affected repository with reproduction steps, expected behavior, and observed behavior. For security vulnerabilities, follow `SECURITY.md` instead.
