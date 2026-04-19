# Installation

## Prerequisites

- Python 3.12+
- [Poetry](https://python-poetry.org/docs/#installation)
- tox (`pip install tox`)

## Quick Start

```bash
poetry install
tox
```

## Development Workflow

Run individual quality gates:

```bash
tox -e py313    # tests + coverage
tox -e lint     # auto-fix linting and formatting
tox -e lint-ci  # lint check without auto-fix (CI mode)
tox -e type     # mypy type checks
tox -e clean    # erase coverage data
```

Alternatively, use the provided convenience script for a one-step setup:

```bash
source venv.sh
```

See [README.md](README.md) for full configuration reference.
