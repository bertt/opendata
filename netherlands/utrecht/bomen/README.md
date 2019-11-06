Bomen utrecht

Source: https://utrecht.dataplatform.nl/#/data/afa19ac8-e63e-4e27-a42e-3bb4f9082c59

```
$ wget https://ckan.dataplatform.nl/dataset/afa19ac8-e63e-4e27-a42e-3bb4f9082c59/resource/2d6893b4-d56d-4865-b6cc-0bda42e547f5/download/bomen_gisib_utrecht.csv
$ ogr2ogr -f geojson 190313_bomen.geojson -oo X_POSSIBLE_NAMES=longitude -oo Y_POSSIBLE_NAMES=latitude -oo KEEP_GEOM_COLUMNS=NO bomen_gisib_utrecht.csv
```

2019-1107: Now the trees seems to be on ArcGIS platform, retrieve with:

```
$ curl https://services7.arcgis.com/KTZrsPfJ9TQsZVGk/arcgis/rest/services/Bomenkaart/FeatureServer/0//query?where=1%3D1&objectIds=&time=&geometry=&geometryType=esriGeometryEnvelope&inSR=&spatialRel=esriSpatialRelIntersects&resultType=none&distance=0.0&units=esriSRUnit_Meter&returnGeodetic=false&outFields=&returnGeometry=true&featureEncoding=esriDefault&multipatchOption=xyFootprint&maxAllowableOffset=&geometryPrecision=&outSR=4326&datumTransformation=&applyVCSProjection=false&returnIdsOnly=false&returnUniqueIdsOnly=false&returnCountOnly=false&returnExtentOnly=false&returnQueryGeometry=false&returnDistinctValues=false&cacheHint=false&orderByFields=&groupByFieldsForStatistics=&outStatistics=&having=&resultOffset=&resultRecordCount=&returnZ=false&returnM=false&returnExceededLimitFeatures=true&quantizationParameters=&sqlFormat=none&f=pgeojson&token= 
```
