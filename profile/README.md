# AscensRun ⚙️

> Production-grade Ansible automation for AGL infrastructure operations.

## What we run

- 🐧 **Linux** — baseline hardening, orchestration, package lifecycle
- 🪟 **Windows** — Active Directory operations, compliance, password lifecycle
- 🌐 **Network** — Cisco, Aruba, Fortinet (FortiManager + FortiGate firewall)
- 💻 **Virtualization** — VMware vSphere credentials, Cyllene, VxRail
- 🎫 **Service Desk** — automated user provisioning and password reset workflows
- 🌍 **Africa infrastructure** — country-specific operations across the AGL footprint

## Standards

Every repository in this org follows:

- 📐 Production-grade structure (roles + playbooks + inventory + CI)
- 🔐 Branch protection (rulesets), secret scanning, push protection
- ✅ CI pipeline (yamllint, ansible-lint production profile, detect-secrets, security scan, Molecule)
- 📝 Conventional commits + Gitflow (`main` ← `develop` ← `feature/*`)
- 🧪 Pre-commit hooks aligned with the CI pipeline
- 🔁 Automated dependency updates via Dependabot

## Repository naming

`ansible-<domain>-<function>` — for example `ansible-network-fortimanager`, `ansible-windows-operations`.

## Operations platform

All playbooks are executed through Semaphore UI (production) with audit trails, scheduled runs, and approval gates for high-blast-radius operations.

## Contact

Owned and maintained by the AscensRun DevOps team for Africa Global Logistics (AGL).
