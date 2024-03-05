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

Our aim with COBRApy is to provide useful, efficient infrastructure for:

- creating and managing metabolic models
- accessing popular solvers
- analyzing models with methods such as FVA, FBA, pFBA, MOMA etc.
- inspecting models and drawing conclusions on gene essentiality, testing
  consequences of knock-outs etc.

Our goal with COBRApy is for it to be useful on its own, and for it to be the
natural choice of infrastructure for developers that want to build new COBRA
related python packages for e.g. visualization, strain-design and data driven
analysis. By re-using the same classes and design principles, we can make new
methods both easier to implement and easier to use, thereby bringing the power
of COBRA to more researchers.

The documentation is browseable online at `readthedocs
<https://cobrapy.readthedocs.org/en/stable/>`_ and can also be `downloaded
<https://readthedocs.org/projects/cobrapy/downloads/>`_.

Please use the `Google Group <http://groups.google.com/group/cobra-pie>`_ for
help. By writing a well formulated question, with sufficient detail, you are
much more likely to quickly receive a good answer! Please refer to these
`StackOverflow guidelines <https://stackoverflow.com/help/how-to-ask>`_ on how
to ask questions.  Alternatively, you can use `gitter.im
<https://gitter.im/opencobra/cobrapy>`_ for quick questions and discussions
about COBRApy (faster response times). Please keep in mind that answers are
provided on a volunteer basis.

More information about opencobra is available at the `website
<http://opencobra.github.io/>`_.

If you use COBRApy in a scientific publication, please cite
`doi:10.1186/1752-0509-7-74 <http://dx.doi.org/doi:10.1186/1752-0509-7-74>`_

Installation
============

Use pip to `install COBRApy from PyPI <https://pypi.org/project/cobra/>`_ (we
recommend doing this inside a `virtual environment
<http://docs.python-guide.org/en/latest/dev/virtualenvs/>`_)::

    pip install cobra

If you want to load MATLAB models, you will need additional dependencies. Please
install::

    pip install cobra[array]

For further information, please follow the `detailed installation instructions
<INSTALL.rst>`_.
