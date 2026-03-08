# Techne Team Instructions

## Repository Overview

- **`pt-techne-opentofu-workflows`** — Reusable GitHub Actions called workflows for OpenTofu + GCP deployments (OIDC auth, state encryption, job summaries, approval gates)
- **`pt-techne-pre-commit-hooks`** — Pre-commit hooks for IaC validation (`tofu fmt`, `tofu validate`, `tofu test`, docs generation, security scanning)
- **`pt-techne-misc-workflows`** — Reusable called workflows for common automation (build-and-push, Dependabot, Nuclei)
- **`pt-techne-opentofu-codespace`** — GitHub Codespace configuration for standardized IaC developer environments

## Conventions

- When modifying reusable workflows or hooks, create a new version tag after merging. Consumer repos must then update their SHA references to the new tag.
