# @motionhungry/github-actions

This repository hosts a collection of reusable GitHub Actions designed to simplify and automate CI/CD workflows and other common automation tasks. These actions are crafted to be easily integrated into your projects, enhancing efficiency and reducing repetitive setup tasks.

## Available Actions

### Install PNPM

The `install-pnpm` action sets up your GitHub Actions runner with Node.js and installs dependencies using [pnpm](https://pnpm.io/), offering faster and more efficient dependency management.

#### Usage

To use the `install-pnpm` action in your workflow, add the following step:

```yaml
- name: Install dependencies with pnpm
  uses: motionhungry/github-actions/install-pnpm@v1
  with:
    fetch-depth: '1'  # Optional, the default is 1
    persist-credentials: true  # Optional, the default is true
```

#### Inputs

- `fetch-depth`: The depth of commits to fetch in the checkout step. Default is `1`.
- `persist-credentials`: Whether to persist credentials in the git config. Default is `true`.

## Getting Started
To get started with these actions, add them to your _.github/workflows/_ YAML files as described in the usage sections.

## Contributing
Contributions to expand and improve this collection are welcome! Please feel free to submit issues, pull requests, or suggest new actions that could benefit the community.

## License
This project is licensed under MIT License - see the LICENSE.txt file for details.
