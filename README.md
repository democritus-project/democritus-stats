# Democritus Stats

[![PyPI](https://img.shields.io/pypi/v/d8s-stats.svg)](https://pypi.python.org/pypi/d8s-stats)
[![CI](https://github.com/democritus-project/d8s-stats/workflows/CI/badge.svg)](https://github.com/democritus-project/d8s-stats/actions)
[![Lint](https://github.com/democritus-project/d8s-stats/workflows/Lint/badge.svg)](https://github.com/democritus-project/d8s-stats/actions)
[![codecov](https://codecov.io/gh/democritus-project/d8s-stats/branch/main/graph/badge.svg?token=V0WOIXRGMM)](https://codecov.io/gh/democritus-project/d8s-stats)
[![The Democritus Project uses semver version 2.0.0](https://img.shields.io/badge/-semver%20v2.0.0-22bfda)](https://semver.org/spec/v2.0.0.html)
[![The Democritus Project uses black to format code](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://choosealicense.com/licenses/lgpl-3.0/)

Democritus functions<sup>[1]</sup> for working with statistics.

[1] Democritus functions are <i>simple, effective, modular, well-tested, and well-documented</i> Python functions.

We use `d8s` (pronounced "dee-eights") as an abbreviation for `democritus` (you can read more about this [here](https://github.com/democritus-project/roadmap#what-is-d8s)).

## Installation

```
pip install d8s-stats
```

## Usage

You import the library like:

```python
from d8s_stats import *
```

Once imported, you can use any of the functions listed below.

## Functions

  - ```python
    def statistical_overview(
        data, *, data_is_sample: bool = False, result_if_no_mode: Any = None, raise_error_if_no_mode: bool = True
    ):
        """Return an overview of the data's statistical properties."""
    ```
  - ```python
    def mode(data, *, result_if_no_mode: Any = None, raise_error_if_no_mode: bool = True):
        """Return the item in the data which occurs the greatest number of times."""
    ```
  - ```python
    def variance(data, *, data_mean=None, data_is_sample: bool = False):
        """Return the variance of the data (assuming the data represents an entire population)."""
    ```
  - ```python
    def stdev(data, *, data_mean=None, data_is_sample: bool = False):
        """Return the standard deviation of the data (assuming the data represents an entire population)."""
    ```
  - ```python
    def mean(iterable):
        """Return the average of the list."""
    ```
  - ```python
    def harmonic_mean(iterable):
        """Return the harmonic mean of the list."""
    ```
  - ```python
    def geometric_mean(iterable):
        """Return the geometric mean of the list."""
    ```

## Development

👋 &nbsp;If you want to get involved in this project, we have some short, helpful guides below:

- [contribute to this project 🥇][contributing]
- [test it 🧪][local-dev]
- [lint it 🧹][local-dev]
- [explore it 🔭][local-dev]

If you have any questions or there is anything we did not cover, please raise an issue and we'll be happy to help.

## Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and Floyd Hightower's [Python project template](https://github.com/fhightower-templates/python-project-template).

[contributing]: https://github.com/democritus-project/.github/blob/main/CONTRIBUTING.md#contributing-a-pr-
[local-dev]: https://github.com/democritus-project/.github/blob/main/CONTRIBUTING.md#local-development-
