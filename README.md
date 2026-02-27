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
  - `depTypeTemplate = max-supported-version` is specified to separate it from other updates and achieve the following.
- Adds `packageRules` for `depType = max-supported-version` the following:
  - `groupName` to separate branches / PRs from other updates.
  - `commitMessageTopic` to replace `dependency {{depName}}` (`dependency Python`) with more helpful `max_supported_version in pyproject.toml`.

[renovate]: https://github.com/renovatebot/renovate
[pyproject-fmt]: https://pypi.org/project/pyproject-fmt/
