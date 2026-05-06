# Security Policy

## Reporting a vulnerability

If you discover a security vulnerability in any AscensRun repository, please report it privately to the AscensRun security contact. Do not open a public issue.

Use one of the following channels:

- GitHub Private Vulnerability Reporting on the affected repository (Security tab > Report a vulnerability)
- Direct email to the AscensRun maintainer

We aim to acknowledge receipt within 2 business days and to provide a status update or remediation plan within 7 business days.

## Supported versions

All AscensRun repositories track the latest commit on `main`. Older revisions are not supported. Apply patches by updating to the latest tagged release or `main`.

## Disclosure policy

Issues are disclosed publicly only after a fix is available and deployed. We coordinate disclosure timelines with reporters when responsible-disclosure conventions apply.

## Hardening posture

All repositories in the organization apply these baseline controls:

- Branch protection on `main` and `develop` via repository rulesets
- Required pull request review
- Required linear history
- Secret scanning and push protection
- Weekly Dependabot version and security updates
- Continuous integration with linting, secret detection, and security scans on every pull request

## Contact

Security contact: through GitHub at @Vedric.
