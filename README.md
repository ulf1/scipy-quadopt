[![PyPI version](https://badge.fury.io/py/scipy-quadopt.svg)](https://badge.fury.io/py/scipy-quadopt)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4284804.svg)](https://doi.org/10.5281/zenodo.4284804)

# scipy-quadopt
Wrapper and utility functions to apply scipy's SLSQP algorithm to quadratic optimization problems with resource constraints and upper boundaries.

## Appendix

### Installation
The `scipy-quadopt` [git repo](http://github.com/satzbeleg/scipy-quadopt) is available as [PyPi package](https://pypi.org/project/scipy-quadopt)

```
pip install scipy-quadopt
pip install git+ssh://git@github.com/satzbeleg/scipy-quadopt.git
```

### Install a virtual environment

```
python3.6 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt --no-cache-dir
pip install -r requirements-dev.txt --no-cache-dir
pip install -r requirements-demo.txt --no-cache-dir
```

(If your git repo is stored in a folder with whitespaces, then don't use the subfolder `.venv`. Use an absolute path without whitespaces.)

### Python commands

* Jupyter for the examples: `jupyter lab`
* Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
* Run Unit Tests: `pytest`
* Upload to PyPi with twine: `python setup.py sdist && twine upload -r pypi dist/*`

### Clean up 

```
find . -type f -name "*.pyc" | xargs rm
find . -type d -name "__pycache__" | xargs rm -r
rm -r .pytest_cache
rm -r .venv
```


### Support
Please [open an issue](https://github.com/satzbeleg/scipy-quadopt/issues/new) for support.


### Contributing
Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/scipy-quadopt/compare/).
