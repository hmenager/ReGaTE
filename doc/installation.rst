.. ReGaTE Registration of Galaxy Tools in Elixir
 Authors: Olivia Doppelt-Azeroual, Fabien Mareuil
 ReGate is distributed under the terms of the GNU General Public License (GPLv2). 
 See the COPYING file for details.
 ReGaTE documentation master file, created by sphinx-quickstart

.. _installation:


************
Installation
************


ReGaTE dependencies
===================

ReGaTE is compatible with version 2.7 of Python. It also requires a set of python libraries: *PyYAML*, *rdflib*, *requests*, *cheetah*, *configparser*, *bioblend*, and *lxml*. These dependencies are automatically installed by the ReGaTE installation procedure. The lxml library requires the python header files, so this means that if you are installing on an ubuntu machine for instance, you must have installed the python-dev package. 

Installation procedure
======================
We recommend to use a virtualenv in order to avoid conflicts with your system configuration. The steps of this procedure are detailed below.

First install virtualenv::

    pip install virtualenv

Then, create a virtual environnement::

    virtualenv ReGaTE_env
And, activate it:: 

    cd ReGaTE_env
    source bin/activate

To install ReGaTE::

    git clone https://github.com/C3BI-pasteur-fr/ReGaTE.git
    cd ReGaTE
    python setup.py install

To install its dependencies::

    pip install -r requirements.txt


.. warning::
  if you update the version of ReGaTE, do not forget to uninstall the previous one! 

Uninstalling ReGaTE
========================

To uninstall ReGaTE (the last version installed), run::

    pip uninstall regate

