# Checkout private actions

## Table of contents

- [Usage](#usage)
- [Inputs](#inputs)
  - [`actions`](#actions)
  - [`directory`](#directory)
  - [`token`](#token)
- [About](#about)

## Usage

```yaml
name: "Example workflow"
on: push
jobs:
  ci:
    runs-on: ubuntu-latest
    steps:
    - uses: rainspell/ga-checkout-private-actions@v0.1.0
      with:
        # List of private actions to clone. Must be an array where each entry matches `owner/repo@ref` format.
        # Type: string[]
        # REQUIRED
        actions: ''

        # Directory where action repositories will be cloned.
        # Type: string
        # Default: ./.github/actions
        directory: ''

        # Repository **PAT** (personal access token) or GITHUB_TOKEN.
        # Type: string
        # REQUIRED
        token: ''

```
## Inputs

### `actions`

List of private actions to clone. Must be an array where each entry matches `owner/repo@ref` format.

**Type**: `string[]`

⚠️ **Required**

---

### `directory`

Directory where action repositories will be cloned.

**Type**: `string`

**Default**: `./.github/actions`

---

### `token`

Repository **PAT** (personal access token) or GITHUB_TOKEN.

**Type**: `string`

⚠️ **Required**



## About
This action was **automatically generated**

---
© 2021 Rainspell 🌧️
