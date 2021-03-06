# pyOptSparse - PYthon OPTimization (Sparse) Framework

[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
[![Build Status](https://travis-ci.com/mdolab/pyoptsparse.svg?branch=master)](https://travis-ci.com/mdolab/pyoptsparse)
[![Coverage Status](https://coveralls.io/repos/github/mdolab/pyoptsparse/badge.svg?branch=master)](https://coveralls.io/github/mdolab/pyoptsparse?branch=master)
[![Documentation Status](https://readthedocs.com/projects/mdolab-pyoptsparse/badge/?version=latest)](https://mdolab-pyoptsparse.readthedocs-hosted.com/en/latest/?badge=latest)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![DOI](https://joss.theoj.org/papers/10.21105/joss.02564/status.svg)](https://doi.org/10.21105/joss.02564)

pyOptSparse is an object-oriented framework for formulating and solving nonlinear constrained optimization problems in an efficient, reusable, and portable manner.
It is a fork of pyOpt that uses sparse matrices throughout the code to more efficiently handle large-scale optimization problems.
Many optimization techniques can be used in pyOptSparse, including both gradient-based and gradient-free methods.
A visualization tool called OptView also comes packaged with pyOptSparse, which shows the optimization history through an interactive GUI.
An example output from OptView is shown below.

![Example](doc/OptView.png)

## Optimizer Support
pyOptSparse provides Python interfaces for a number of optimizers.
ALPSO, CONMIN, IPOPT, NLPQLP, NSGA2, PSQP, SLSQP, ParOpt and SNOPT are currently tested and supported.
NOMAD interface is also provided, but it is not tested nor supported.

We do not provide the source code for SNOPT and NLPQLP, due to their restrictive license requirements.
Please contact the authors of the respective optimizers if you wish to obtain them.
Furthermore, ParOpt and IPOPT are available as a open source package but must be installed separately.
Please see the documentation page of each optimizer for purchase and installation instructions.

## Documentation
Please see the [documentation](https://mdolab-pyoptsparse.readthedocs-hosted.com/) for installation details and API documentation.

## Testing
Testing is done with the `testflo` package developed by the openMDAO team, which can be installed via `pip install testflo`.
To run the tests, simply type `testflo .` in the root directory.

## Citation
If you use pyOptSparse, please see [this page](https://mdolab-pyoptsparse.readthedocs-hosted.com/en/latest/citation.html) for citation information.

## License
pyOptSparse is licensed under the GNU Lesser General Public License.
See `LICENSE` for the full license.

## Copyright
Copyright (c) 2011 University of Toronto\
Copyright (c) 2014 University of Michigan\
Additional copyright (c) 2014 Gaetan K. W. Kenway, Ruben Perez, Charles A. Mader, and\
Joaquim R. R. A. Martins\
All rights reserved.
