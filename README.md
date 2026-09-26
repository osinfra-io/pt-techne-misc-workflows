# Miscellaneous Called Workflows

[![Dependabot](https://img.shields.io/github/actions/workflow/status/osinfra-io/pt-techne-misc-workflows/dependabot.yml?style=for-the-badge&logo=github&color=2088FF&label=Dependabot)](https://github.com/osinfra-io/pt-techne-misc-workflows/actions/workflows/dependabot.yml)

Reusable GitHub Actions workflows for common platform repository automation. Consumers pin the workflow source to a full commit SHA and pass the inputs, secrets, and permissions declared by the selected workflow.

## Consumer workflows

| Workflow | Purpose |
| --- | --- |
| [`add-to-project.yml`](.github/workflows/add-to-project.yml) | Add repository work items to the organization project |
| [`build-and-push.yml`](.github/workflows/build-and-push.yml) | Build and publish a container image |
| [`dependabot.yml`](.github/workflows/dependabot.yml) | Apply the shared Dependabot automation policy |
| [`nuclei.yml`](.github/workflows/nuclei.yml) | Run Nuclei security scanning |
| [`release.yml`](.github/workflows/release.yml) | Publish repository releases from version tags |

Files prefixed with `local-` are maintenance workflows for this repository, not reusable consumer interfaces.
