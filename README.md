[![License Apache2](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
[![release-please](https://github.com/okdp/gh-workflows/actions/workflows/release-please.yml/badge.svg)](https://github.com/okdp/gh-workflows/actions/workflows/release-please.yml)
<p align="center">
    <img width="400px" height=auto src="https://okdp.io/logos/okdp-inverted.png" />
</p>

Collection of github actions [reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows) and [actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions#about-custom-actions) shared by the OKDP platform components (helm charts, docker images, etc)

# Using the reusable workflows

The example below shows how to reuse the workflow ```helm-lint.yml``` with the version ```main``` in your github repository:

```console
name: ci 
on:
  push:
jobs:
  ci:
    name: ci
    uses: okdp/workflows/.github/workflows/helm-lint.yml@main
```
