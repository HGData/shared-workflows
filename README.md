# shared-workflows

[![CI](https://github.com/HGData/shared-workflows/actions/workflows/main.yml/badge.svg)](https://github.com/HGData/shared-workflows/actions/workflows/main.yml)

## Overview

A repository to house GitHub Actions [reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows).

## Usage

Consume shared workflows as a discrete job
```yaml
jobs:
  dependabot:
    uses: hgdata/shared-worflows/.github/workflows/dependabot-auto-merge.yml@main
    secrets:
      token: ${{ secrets.ACTIONS_REPO_TOKEN }}
```
