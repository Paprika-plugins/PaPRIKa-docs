***************
Getting started
***************


In order to use the PaPRIKa Toolbox, you need some input data that represents all criteria used in the Official PaPRIKa
method. If you're not familiar with the PaPRIKa methods please have a look at
`the official guide <http://infoterre.brgm.fr/rapports/RP-57527-FR.pdf>`_
to understand well all the needed input and the workflow.

All needed datas are vector or raster layer that can be loaded by QGIS.

.. warning:: All input layers need to be in the same projected CRS

Catchment Area and resolution
---------------

This layer must contains a unique feature which represent the catchment area of your study area.
It's used to define the extent of the raster layers build by the different algorithms.
the vulnerability map expected resolution expressed in project unit. This
resolution should be coherent with data resolution.

*  Layer type: Vector layer
*  Geometry type : Polygon
*  Fields needed : No field needed



P Factor
----------

Soil
++++++

A polygon layer containing a representation of the different types of soil present
in your catchment area.

*  Layer type: Vector layer
*  Geometry type: Polygon
*  Fields needed: An integer field containing value between 0 and 4 that represent the protectivness of the soil
*  Must cover all the catchment area to get relevant results

Unsaturated Zone
+++++++++++++++++

A Raster layer with classes from 0 to 4 that represent the thickness of the unsaturated zone

*  Layer type: Raster layer
*  Constraints: 1 band with integer values between 0 and 4

Epikarst (optional)
+++++++++++++++++++++

An optional polygon layer containing a representation of area where an Epikarstic layers acts as a protector of the resource.
in your catchment area.

*  Layer type: Vector layer
*  Geometry type: Polygon
*  Fields needed: An integer field containing value between 1 and 4 that represent the protectivness of the soil

Sinking stream catchment (optional)
+++++++++++++++++++++++++++++++++++++

An optional polygon layer that represent an area of run off that end in the catchment area

*  Layer type: Vector layer
*  Geometry type: Polygon
*  Fields needed: An integer field containing value between 1 and 4

R Factor
----------

Lithology
+++++++++++

Structure (optional)
++++++++++++++++++++++

I Factor
----------

DEM
+++++

Karst Features (optional)
++++++++++++++++++++++++++

Ka Factor
----------

Karst Features (optional)
+++++++++++++++++++++++++++



