# python-template

An opinionated project template for Python built with poetry/tox

## Overview

This is a template repository. It comes with support for the following:

- Unit testing via [pytest](https://docs.pytest.org/en/7.1.x/index.html)
- Code coverage via [coverage](https://coverage.readthedocs.io/en/6.5.0/index.html)
- Linting via [flake8](https://flake8.pycqa.org/en/latest/)
- Formatting via [yapf](https://github.com/google/yapf) and [isort](https://pycqa.github.io/isort/)
- Static type checking via [mypy](https://mypy.readthedocs.io/en/stable/index.html)
- Orchestration of the above quality gates via [tox](https://tox.wiki/en/latest/index.html)
- Dependency and module management via [poetry](https://python-poetry.org/)

## Template Usage

### Required Changes

To get started with this template, changes will need to be made to the module name in various locations.

- `pyproject.toml` attributes for name and package
- The `src/python_template` folder name
- `src/python_template/__init__.py` name variable

The `poetry.lock` file will need to be deleted so it can be regenerated with the new module's values

### Project Setup

The template comes provided with a `venv.sh` file for helping in the setup of a Python virtual environment.  The script will perform the following actions:

- Install the required developer tooling
- Create the virtual environment using `venv`
- Activate the virtual environment
- Upgrade pip
- Install the project dependencies
- Display outdated dependencies

This is purely for convienence. It can be ran again with the virtual environment created to perform an update and activate it.

## Reference Configuration

Project configuration options and flag referenced by the following locations.

### pytest

<https://docs.pytest.org/en/7.1.x/reference/reference.html#ini-options-ref>

### coverage

<https://coverage.readthedocs.io/en/6.5.0/config.html>

### tox

<https://tox.wiki/en/latest/config.html>

### mypy

<https://mypy.readthedocs.io/en/stable/config_file.html>

### isort

<https://pycqa.github.io/isort/docs/configuration/config_files.html>

### yapf

<https://github.com/google/yapf#knobs>

## flake8

<https://flake8.pycqa.org/en/latest/user/configuration.html>

### poetry

<https://python-poetry.org/docs/pyproject/>
