# <img align="left" width="45" height="45" src="https://user-images.githubusercontent.com/1610100/201473670-e0e6bdeb-742f-4be1-a47a-3506309620a3.png"> Miscellaneous Called Workflows

[![Dependabot](https://img.shields.io/github/actions/workflow/status/osinfra-io/pt-techne-misc-workflows/dependabot.yml?style=for-the-badge&logo=github&color=2088FF&label=Dependabot)](https://github.com/osinfra-io/pt-techne-misc-workflows/actions/workflows/dependabot.yml)

Reusing workflows avoids duplication. This makes workflows easier to maintain and allows you to create new workflows
more quickly by building on the work of others, just as you do with actions.

Workflow reuse also promotes best practice by helping you to use workflows that are well designed, have already been
tested, and have been proved to be effective. Your organization can build up a library of reusable workflows that can
be centrally maintained.

## Reusing Workflows

Rather than copying and pasting from one workflow to another, you can make workflows [reusable](https://docs.github.com/en/actions/learn-github-actions/reusing-workflows). You and anyone with access to the reusable workflow can then call the reusable workflow from another workflow.

### Workflows

- [add-to-project.yml](.github/workflows/add-to-project.yml)
- [build-and-push](.github/workflows/build-and-push.yml)
- [dependabot.yml](.github/workflows/dependabot.yml)
- [nuclei.yml](.github/workflows/nuclei.yml)

```mermaid
graph LR
    A[Push tag v*] --> B[Release]
    C[pull_request_target] --> D[Dependabot]
    E[issues / pull_request opened] --> F[Add to GitHub projects]

    style A fill:#fff4e6,color:#000
    style B fill:#d4edda,color:#000
    style C fill:#fff4e6,color:#000
    style D fill:#d4edda,color:#000
    style E fill:#fff4e6,color:#000
    style F fill:#d4edda,color:#000
```
