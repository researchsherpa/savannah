# Extract Savannah GA Polygon

The Code-for-Atlanta team needs the polygon for Savannah GA to support their treepedia project.  This is an example of how to extract the information from an open data source published by [Savannah Area GIS Open Data](https://data-sagis.opendata.arcgis.com/) portal.

Could do this with simple command line utility, but wanted to explore the data set so decided on a notebook.

## Contents

- Data directory contains the input shape file from SAGIS

- Data directory will be used for the output geojson file.

- Notebooks directory contains the notebook to display and extract required data

- Notebook can be explored with binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/researchsherpa/savannah/main?urlpath=lab)


## Setting Up Local Env

I use jupyter lab with ipywidgets and ipyleaflet for my development. It may not be the standard.  I've tried to seperate a base environment with the needed analysis packages.  Anaconda is required with this approach.  This is the way I do it so your mileage may vary.

  1. Assuming anaconda is installed, environment.yml can be used to build a baseline lab env with conda:  `conda env create -f environment.yml`
  
  2. Activate the new env: `conda activate savannah`
  
  3. Once the python env is done set up the js packages with: `jupyter labextension install @jupyter-widgets/jupyterlab-manager jupyter-leaflet`
  
  4. At this point you will have a working jupyter lab with the necessary widgets and executing jupyter lab inside the savannah env will start a local version of jupyter lab