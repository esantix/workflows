# Workflows

Collection of reusable Github Action Workflows


## Usage example

```yml
name: Code quality

on:
  pull_request:
    branches:
      - main

jobs:
  flake8:
    uses: esantix/workflows/.github/workflows/python_flake8.yml@main
    with:
      ignore-codes: E501,E502
```

## Testing

[![](https://github.com/esantix/workflows-testing/actions/workflows/test_workflows.yml/badge.svg)](https://github.com/esantix/workflows-testing/actions/workflows/test_workflows.yml)

Workflows are tested with mock repo: [esantix/workflows-testing](https://github.com/esantix/workflows-testing/actions)