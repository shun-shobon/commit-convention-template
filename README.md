# Commit Convention Template

[![Action Status][github-actions-icon]][github-actions-href]
[![Commitizen friendly][commitizen-icon]][commitizen-href]

> Template for adhering commit convention

# Usage

```shell script
# install dependencies
$ yarn install

# commit with commitizen
$ yarn cz

# commit with commitizen (Linux / MacOS only)
# commitizen runs automatically when commit
$ git commit
```

Commitlint runs automatically after commit by husky.
Also, when you push to github, commitlint runs on ci by github actions.
This ensures that commit convention are always adhering.

Commitizen is useful for committing based on commit convention.
When you commit with commitizen, you'll be prompted to fill out any required commit fields at commit time.
Commitizen run automatically when committing by husky, but fails on windows.
So, if you use this repository on windows, please delete `husky.hooks.prepare-commit-msg` in `package.json`.

[github-actions-icon]: https://github.com/shun-shobon/commit-convention-template/workflows/Commitlint/badge.svg
[github-actions-href]: https://github.com/shun-shobon/commit-convention-template/actions
[commitizen-icon]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[commitizen-href]: http://commitizen.github.io/cz-cli/
