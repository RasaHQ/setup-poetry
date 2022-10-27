# Setup Poetry action

This action sets up
* python
* poetry
* dependency caching

The action is build as a composite action, reusing existing actions.

## Inputs

## `python-version`

**Required** The version of python to install.

## `poetry-version`

**Required** The version of poetry to install.

## `venv-path`

The directory for the virtual environment of poetry dependencies. The directory
should be in the same directory as `pyproject.toml`. By default, set to `.venv`.

## Example usage

```yaml
- name: Setup poetry 🦄
  uses: rasahq/setup-poetry@v2
  with:
    python-version: "3.9"
    poetry-version: "1.2.1"
    venv-path: .venv
```
