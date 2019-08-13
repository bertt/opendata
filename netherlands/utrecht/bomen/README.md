Bomen utrecht

Source: https://utrecht.dataplatform.nl/#/data/afa19ac8-e63e-4e27-a42e-3bb4f9082c59

```
$ wget https://ckan.dataplatform.nl/dataset/afa19ac8-e63e-4e27-a42e-3bb4f9082c59/resource/2d6893b4-d56d-4865-b6cc-0bda42e547f5/download/bomen_gisib_utrecht.csv
$ ogr2ogr -f geojson 190313_bomen.geojson -oo X_POSSIBLE_NAMES=longitude -oo Y_POSSIBLE_NAMES=latitude -oo KEEP_GEOM_COLUMNS=NO bomen_gisib_utrecht.csv
```