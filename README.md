# GitHub Workflows

![License](https://badgen.net/github/license/getindata/github-workflows/)
![Release](https://badgen.net/github/release/getindata/github-workflows/)

<p align="center">
  <img height="150" src="https://getindata.com/img/logo.svg">
  <h3 align="center">We help companies turn their data into assets</h3>
</p>

---
This repository is a collection of reusable GitHub Actions workflows aimed at providing a centralized library for commonly used tasks. 

By maintaining a single source of truth for these workflows, we can ensure consistency, reduce duplication, and simplify maintenance across multiple projects.

## USAGE

Place this sample workflow file into your project's `.github/workflows` folder. It utilizes the `gh-create-release.yml` workflow from this repository.

```yaml
name: Create new release with changelog

on:
  pull_request_target:
    types: [closed]

jobs:
  release:
    uses: getindata/github-workflows/.github/workflows/gh-create-release.yml@<branch_or_tag_name>

```

## NOTES

For additional examples and information on limitations, inheritance, inputs, outputs, and more, consult the official GitHub [documentation](https://docs.github.com/en/actions/using-workflows/reusing-workflows#overview).

## CONTRIBUTING

Contributions are very welcomed!

Start by reviewing [contribution guide](CONTRIBUTING.md) and our [code of conduct](CODE_OF_CONDUCT.md). After that, start coding and ship your changes by creating a new PR.

## LICENSE

Apache 2 Licensed. See [LICENSE](LICENSE) for full details.

## AUTHORS

<!--- Replace repository name -->
<a href="https://github.com/getindata/github-workflows/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=getindata/github-workflows" />
</a>

Made with [contrib.rocks](https://contrib.rocks).
