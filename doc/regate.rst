.. ReGaTE documentation master file, created by
   sphinx-quickstart on Mon Jun 29 16:39:40 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.
   
.. _regate guide:

ReGaTE Guide
============

In order to run ReGaTE you need an account on a galaxy workbench with an API Key, see galaxy documentation if necessary (https://wiki.galaxyproject.org/Learn/API).

* Type:

  "``regate.py -h``"
  to see all options available.

* Type:

  "``regate.py --galaxy_url your_galaxy_url --api_key your_galaxy_api_key --edam_file src/regate/data/yaml_mapping.yaml --tool_dir jsons_output``"
  
  to obtain a list of json files which are the description of each tool installed in your galaxy from a toolshed.
  
  yaml_mapping.yaml is a mapping file between the EDAM ontology and the galaxy extension in a yaml format. You can generate a new version of this file with remag.py see :ref:`remag options section <remag guide>`.