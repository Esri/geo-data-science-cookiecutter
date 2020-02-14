# [GeoAI-Cookiecutter](https://arcgis.github.io/geoai-cookiecutter)

[GeoAI-Cookiecutter Project Homepage](https://arcgis.github.io/geoai-cookiecutter)

GeoAI-Cookiecutter strives to streamline and promote use of best practices for projects combining Geography and Artificial Intelligence through a logical, reasonably standardized, and flexible project structure.

GeoAI-Cookiecutter project grew out of a need within the Advanced Analytics team at Esri to streamline project bootstrapping, encourage innovation, increase repeatability, encourage documentation, and encourage best practices.

## Requirements to use the cookiecutter template:
 * ArcGIS Pro 2.4 or greater (Python 3.6 and Conda come with it)
 * [Cookiecutter](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0

``` bash
> conda install -c conda-forge cookiecutter
```


## To start a new project, run:

``` bash
> cookiecutter https://github.com/ArcGIS/geoai-cookiecutter
```

## The resulting directory structure

The directory structure of your new project will look like this: 

```
    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data`
    ├── make.bat           <- Windows batch file with commands like `make data`
    ├── setup.py           <- Setup script for the library ({{ cookiecutter.support_library }})
    ├── .env               <- Any environment variables here - created as part of project creation, 
    │                         but NOT syncronized with git repo for project.                
    ├── README.md          <- The top-level README for developers using this project.
    ├── arcgis             <- Root location for ArcGIS Pro project created as part of
    │   │                     data science project creation.
    │   ├── {{ cookiecutter.project_name }}.aprx <- ArcGIS Pro project.    
    │   └── {{ cookiecutter.project_name }}.tbx  <- ArcGIS Pro toolbox associated with the project.
    ├── scripts            <- Put scripts to run things here.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   │   └── interim.gdb
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   │   └── processed.gdb
    │   └── raw            <- The original, immutable data dump.
    │       └── raw.gdb
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    ├── notebooks          <- Jupyter notebooks. Naming convention is a 2 digits (for ordering),
    │   │                     descriptive name. e.g.: 01_exploratory_analysis.ipynb
    │   └── notebook_template.ipynb
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    ├── environment.yml    <- The requirements file for reproducing the analysis environment. This 
    │                         is generated by running `conda env export > environment.yml` or
    │                         `make env_export`.                         
    └── src                <- Source code for use in this project.
        └── {{ cookiecutter.support_library }} <- Library containing the bulk of code used in this 
                                                  project. 
```

## Licensing
Copyright 2020 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's [LICENSE](LICENSE?raw=true) file.
