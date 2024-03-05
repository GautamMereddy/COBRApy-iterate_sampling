================================================================
COBRApy - Iterative Sampling
================================================================

Jason H. Yang Lab @ Rutgers New Jersey Medical School

Author: Gautam Mereddy

Date: March 5, 2024



What is COBRApy?
================

COBRA methods are widely used for genome-scale modeling of metabolic networks in
both prokaryotes and eukaryotes. **COBRApy** is a constraint-based modeling
package that is designed to accommodate the biological complexity of the next
generation of COBRA models and provides access to commonly used COBRA methods,
such as flux balance analysis, flux variability analysis, and gene deletion
analyses.

More information about opencobra is available at the `website
<http://opencobra.github.io/>`_.

What is iterate sampling?
=========================

In src/cobra/sampling, an additional script called iterate_sampling.py has been added which includes additional functions that allow for the automatic flux sampling of multiple genome-scale metabolic models simultaneously through a single function, iterate_pysampling(). The iterate_pysampling() function uses parallel processing to sample multiple genome-scale model files (in Matlab's .mat format) in a specified directory using the same sampling parameters for each model. This function was designed to be used in conjunction with our other R-based, in-house pipeline iterate_iMAT (based off the ruppinlab/gembox repository). The iterate_pysampling() function outputs two tab-delimited files for each genome-scale model that contain the flux sampling results and the summary statistics for these sampling results.

All functions in iterate_sampling.py have been tested with the following specifications:

- Python 3.7.11

- CORBApy 0.21.0

- Gurobi 9.5.2

Installation
============

To Use pip to `install COBRApy from PyPI <https://pypi.org/project/cobra/>`_ (we
recommend doing this inside a `virtual environment
<http://docs.python-guide.org/en/latest/dev/virtualenvs/>`_)::

    pip install cobra

If you want to load MATLAB models, you will need additional dependencies. Please
install::

    pip install cobra[array]

For further information, please follow the `detailed installation instructions
<INSTALL.rst>`_.

To add iterate_sampling.py to an already-made installation of COBRApy, move iterate_sampling.py to src/cobra/sampling.
