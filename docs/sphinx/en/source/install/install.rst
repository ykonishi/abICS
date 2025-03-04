.. highlight:: none

Prerequisites
~~~~~~~~~~~~~~~~~~~~~~

abICS requires Python3 (>=3.7).

The following Python packages are required.

- numpy
- scipy
- toml
- mpi4py
- pymatgen (>=2019.12.3)
- qe-tools

These are installed automatically but mpi4py and pymatgen need extra software-packages before installing them.

- mpi4py needs one of the MPI implementations, e.g., Open MPI.
- pymatgen needs Cython::

   $ pip3 install cython

.. To use VASP as a solver, a patch must be applied to use MPI_COMM_SPAWN. If you wish to use it, please contact us (the e-mail address is written in :doc:`../contact/index` ).

Install from PyPI
~~~~~~~~~~~~~~~~~~~~

Since abICS is registered in PyPI users can install abICS easily::

   $ pip3 install abics

If you want to install abICS locally because, for example, you have no permission to write files, the following command::

   $ pip3 install --user abics

installs abICS below a directory ``~/.local`` .
If you want to install abICS into another directory, use the ``--prefix=DIRECTORY`` option (``DIRECTORY`` is the path to the directory where abICS will be installed) .

Install from source
~~~~~~~~~~~~~~~~~~~~~~

Download
..............

The source codes of abICS can be obtained from `GitHub page <https://github.com/issp-center-dev/abICS>`_ .

``$ git clone https://github.com/issp-center-dev/abICS``

  
Directory structure
.......................

The directory structure of abICS is given as follows:

:: 

 .
 |-- COPYING
 |-- README.md
 |-- abics/
 |   |-- __init__.py
 |   |-- applications/
 |   |-- exception.py
 |   |-- mc.py
 |   |-- mc_mpi.py
 |   |-- replica_params.py
 |   |-- scripts/
 |   |-- util.py
 |-- docs/
 |   |-- sphinx/
 |-- examples/
 |-- pyproject.toml
 |-- test/
 |-- tests/
 

A set of python modules are located in the ``abics`` directory.


      
Install
...........

- Pass the location of the root directory of abICS as an argument of ``pip3 install`` :

   $ pip3 install ./abICS

Uninstall
~~~~~~~~~~

- ``pip3 uninstall abics`` uninstalls abics from your machine.
