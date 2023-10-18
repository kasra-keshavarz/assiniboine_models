Introduction
------------

This directory contains scripts to 1) extract the boundaries of the
Assiniboine River Basin, Canada, from the MERIT-Basins dataset as the base
geofabric for hydrological modelling experiment and 2) implement necessary
sanity checks on the extracted geofabric to assure it is ready for
modelling practices.


Datasets
--------

  * Geospatial fabrics:
  
    1. MERIT-Basins (version v0.7/v1.0, minor bug fix for coastline
    pixels): https://www.reachhydro.org/home/params/merit-basins
       
       This datasets was used as the base geofabric for the modelling
       practices. The dataset was accessed on February 27th, 2023.

    2. Boundary polygons for the ARB
    (provided by Dan Princz, last accessed on October 17th, 2023):

       This dataset was used the source geometry for the boundaries of the
       ARB.


   * Workflows:

     1. "pre-process_geofabric.ipynb"

        Containing scripts to subset layers 71 82 of the
	MERIT-Basins dataset for ARB boundaries

     2. "sanity-checks_geofabric.ipynb"

        Containing scripts to implement sanity checks on the extracted
	geofabric from the previous script

     3. hydrant (v0.1.0-dev0): https://github.com/kasra-keshavarz/hydrant

        Currently under development, this packages provides common
	functions for the analysis, manipulation, and sanity check of
	river and sub-basin geospatial fabrics within the context of
	hydrological modelling. It is worth noting that this package is
	used in the two scripts listed above


Last edited: October 18th, 2023
