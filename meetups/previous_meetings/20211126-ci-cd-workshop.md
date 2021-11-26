# CI/CD workshop

Date: 26/11/2021, 1pm UK time

Contributors: @mloning, @ltsaprounis

---

## :bulb: What do you want to learn? 
- [name=fkiraly] CI/CD for sktime end-to-end, especially release related
- [name=Svea] 
- [name=ltsaprounis] CI but mostly CD for sktime
- [name=kejsitake] General introduction
- [name=Amrith] Github actions
- [name=lmmentel] overview of the current CI/CD flows and how far from the ideal state we are?
- [name=luca] CI/CD end-to-end
---

## :books: Suggested topics

### Overview
1. CI/CD platforms
1. Unit tests using pytest
2. Code quality checks: flake8, black, isort, pydocstyle, etc.
3. Pre-commit hooks and pre-commit package
4. Online docs
5. CI (continuous integration testing)
6. CD (packaging and distribution)

---

### :construction: CI/CD platforms
Free compute time on:
* Azure DevOps
* Appveyor
* GitHub Actions (direct integration with GitHub)
* ReadTheDocs

### Unit tests using pytest
* automatic unit tests for API compliance for estimator scitypes 
* testing compiled package rather than source code
* setup.cfg configuration

### :mag: Code quality checks: flake8, black, isort, etc.
* format checks PEP8
* auto-formatting with black
* imports order with isort
* pydocstyle for docstrings quality
* setup.cfg configuration

### Pre-commit hooks and pre-commit package
* basic checks on changed files before committing

### Online docs
* Sphinx 
* pydocstyle using NumPy convention
* pytest with doctest for docstring examples
* ReadTheDocs

###  CI (continuous integration testing)
* code quality checks: pre-commit on changed files in PR
* examples notebooks
* unit tests on different operating systems and Python versions
* generate online docs 
* test coverage using codecov
* conditionalty: unit tests only run if code quality checks pass
* CI badges (shields.io)

### :package: CD (packaging and distribution)
why do we need CD?
* not pure Python package, sktime contains some pre-compiled code (Cython)
* some code needs to be pre-compiled
* compilation is specific to operating systems and Python versions
* we need distribution different wheels for different operating systems and Python versions 

CD process
* build package
* unit tests
* upload it to PyPI
* tags & releases

helper script: `build_tools/make_release.py` or `make release`

### Developer workflow
* Running GitHub Actions locally: https://github.com/nektos/act
* Running manylinux images locally: https://gist.github.com/mloning/9773af828cc654b6b690bc7dcc1013b0
