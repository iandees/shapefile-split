shapefile-split
===============

A simple python script to split a shapefile into smaller pieces.

Known Issues
------------

1. It will be very slow unless you add a [shapefile index](http://gdal.org/ogr/drv_shapefile.html) to speed up the spatial operations. For example:

   `ogrinfo file1.shp -sql "CREATE SPATIAL INDEX ON file1"`

2. There will be duplicate features at the split edges. This can be fixed in the future.

