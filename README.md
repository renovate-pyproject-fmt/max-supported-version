# [Renovate][renovate] configuration for updating [`pyproject-fmt`][pyproject-fmt]`.max-supported-version`

## Usage

```json
{
  "extends": [
    "github>renovate-pyproject-fmt/max-supported-version"
  ]
}
```

## How it works

- Adds `customManager`.
  - `depTypeTemplate = max_supported_version` is specified to separate it from other updates and achieve the following.
- Adds `groupName` in `packageRules` for `depType = max_supported_version` to separate branches / PRs from other updates.

[renovate]: https://github.com/renovatebot/renovate
[pyproject-fmt]: https://pypi.org/project/pyproject-fmt/
