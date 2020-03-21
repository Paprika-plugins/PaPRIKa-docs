***************
Getting started
***************


In order to use the PaPRIKa Toolbox, you need some input data that represents all criteria used in the Official PaPRIKa
method.

All needed data are vector or raster layer that can be load in QGIS.

.. warning:: All input layers need to be in the same projected CRS

Catchment Area
---------------

This layer must contains a unique feature which represent the catchment area of your study area.
It's used to define the extent of the rasters layers build by the different algorithms.

*  Layer type: Vector layer
*  Geometry type : Polygon
*  Fields needed : No field needed

P Factor
--------

Soil
+++++

A polygon containing a representation of the different types of soil present
in your catchment area.

*  Layer type: Vector layer
*  Geometry type: Polygon
*  Fields needed: An integer field containing value between 0 and 5 that represent the protectivness of the soil

Epikarst (optional)
++++++++++++++++++++
