.. ReGaTE documentation master file, created by
   sphinx-quickstart on Mon Jun 29 16:39:40 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.
   
.. _remag guide:

ReMaG Guide
============

In order to run ReMaG you need a description file of the EDAM ontology in the owl format https://github.com/edamontology/edamontology.git, EDAM_X.owl file.

* Type:

  "``remag.py -h``"
  to see all options available.
  
* The execution of remag give an yaml file, a mapping between galaxy extension and edam format/data, to obtain it:

-- With a mapping tsv file (first column: galaxy extension, second column the edam format: fomat_XXX, third column: description), type:

  "``remag.py --mapping_file mapping --output_yaml myyaml.yaml --edam_file EDAM_X.owl``"


-- With a datatype_conf with edam_type attribut, type:

  "``remag.py --datatype_conf yourdatatype --output_yaml myyaml.yaml --edam_file EDAM_X.owl``"

-- With a recent galaxy (https://github.com/galaxyproject/galaxy.git, for the moment the dev branch is necessary to have the edam format, you need an account and an api key on this galaxy), type:

  "``remag.py --galaxy_url a_galaxy_url --api_key the_galaxy_api_key --output_yaml myyaml.yaml --edam_file EDAM_X.owl``"
  
 