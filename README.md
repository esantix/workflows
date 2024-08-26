# Workflows

Collection of reusable Github Action Workflows


#### Usage example or flake8 on other repo

```yml
name: Code quality

on:
  pull_request:
    branches:
      - main

jobs:
  flake8:
    uses: esantix/workflows/.github/workflows/pytho_flake8.yml@main
    with:
        ignore-codes: E501,E502

```