# Python Starter

> [Python](https://www.python.org/) Starter Template

This template was inspired by [pypa/sampleproject](https://github.com/pypa/sampleproject).

## Setup

### Package Information

See [setup.py](./setup.py)

Check the package classifier here: [PyPI Classifiers](https://pypi.org/classifiers/)

Reference: [Building and Distributing Packages with Setuptools](https://setuptools.readthedocs.io/en/latest/setuptools.html)

### GitHub Workflow

See [python.yml](./.github/workflows/python.yml)

Check `pytest --cov=package_name --cov-report=xml` in line 81, and fix it to your package name.

Implemented Jobs:

- Lint with [Flake8](https://flake8.pycqa.org/)
- Test with [pytest](https://docs.pytest.org/)
- Code Coverage with [pytest-cov](http://pytest-cov.rtfd.org/) and [Codecov](http://codecov.io/)

### Badges for Documentation

See [Shields.io](https://shields.io/)

Package Version:

```markdown
[![PyPI](https://img.shields.io/pypi/v/package_name?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/package_name/)
```

Required Python Version:

```markdown
[![Python](https://img.shields.io/pypi/pyversions/package_name?logo=python&logoColor=white&style=for-the-badge)](https://www.python.org/)
```

GitHub Workflow Status:

```markdown
[![GitHub Workflow](https://img.shields.io/github/workflow/status/author_name/package_name/Python?logo=github&logoColor=white&style=for-the-badge)](https://github.com/author_name/package_name/actions)
```

Code Coverage with [Codecov](http://codecov.io/):

```markdown
[![Codecov](https://img.shields.io/codecov/c/gh/author_name/package_name?logo=codecov&logoColor=white&style=for-the-badge)](https://codecov.io/gh/author_name/package_name)
```

Package Downloads:

```markdown
[![Downloads](https://img.shields.io/pypi/dm/package_name?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/package_name/)
```

Package License:

```markdown
[![License](https://img.shields.io/pypi/l/package_name?style=for-the-badge)](./LICENSE)
```

## Test

### Run [pytest](https://docs.pytest.org/)

```bash
$ pytest
```

### Code Coverage with [pytest-cov](http://pytest-cov.rtfd.org/)

```bash
$ pytest --cov=package_name
```

If you need the output in html format:

```bash
$ pytest --cov=package_name --cov-report=html
```

See [pytest-cov Reporting](https://pytest-cov.readthedocs.io/en/latest/reporting.html)

## Deploy

### Create `requirements.txt`

```bash
pip freeze > requirements.txt
```

### Fix `LICENSE`

Delete the original [LICENSE](./LICENSE) file or change it to your license file.

### Packaging Project

```bash
$ pip install --user --upgrade setuptools wheel
$ python ./setup.py sdist bdist_wheel
```

### Check Project Package

```bash
$ pip install --user --upgrade twine
$ twine check dist/*
```

### Update Package to [PyPI](https://pypi.org/)

```bash
$ twine upload dist/*
```

If you want to upload the package to [Test PyPI](https://test.pypi.org/), use `--repository testpypi` option.

Reference: [Packaging Python Projects](https://packaging.python.org/tutorials/packaging-projects/)

## License

```text
Copyright (c) 2020 Seungjae Park

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

Python Starter is licensed under the [MIT License](./LICENSE).
