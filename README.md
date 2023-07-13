# opendata

Creating Geoparquet files:

GeoParquet file with GeoArrow

```
  $ ogr2ogr gemeenten2016_arrow.parquet gemeenten2016.geojson  \
  -lco COMPRESSION=BROTLI \
  -lco GEOMETRY_ENCODING=GEOARROW \
  -lco POLYGON_ORIENTATION=COUNTERCLOCKWISE \
  -lco ROW_GROUP_SIZE=9999999
```

GeoParquet file with WKB

```
$ ogr2ogr gemeenten2016_wkb.parquet gemeenten2016.geojson  \
  -lco COMPRESSION=BROTLI \
  -lco GEOMETRY_ENCODING=WKB \
  -lco POLYGON_ORIENTATION=COUNTERCLOCKWISE \
  -lco ROW_GROUP_SIZE=9999999
```

GeoArrow file:


```
$ ogr2ogr gemeenten2016.arrow gemeenten2016.geojson  
```