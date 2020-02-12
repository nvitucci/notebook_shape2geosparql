# notebook_shape2geosparql

A notebook on the usage of `shape2geosparql` with a few examples.

## Quick start

You need three libraries in order to use this notebook:

- Python 3 (download page here [here](https://www.python.org/downloads/));
- GDAL (installation instructions [here](https://trac.osgeo.org/gdal/wiki/DownloadingGdalBinaries));
- Fuseki GeoSPARQL server (latest downloadable JAR [here](https://repo1.maven.org/maven2/org/apache/jena/jena-fuseki-geosparql/3.14.0/jena-fuseki-geosparql-3.14.0.jar)).

Once you have Python 3 and GDAL installed, run the following:

```bash
$ git clone https://github.com/nvitucci/notebook_shape2geosparql
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

If the GDAL bindings cannot be installed, try running `$ pip install gdal==<VERSION>` where VERSION is the version of GDAL you installed on your system.

When all the packages are installed, run `jupyter notebook` and navigate to the notebook file. In a separate shell, run the Fuseki GeoSPARQL server as follows:

```bash
$ java -jar jena-fuseki-geosparql-3.14.0.jar -u
```

## Data

The data have been downloaded from the Open Data Trentino portal:

- http://webapps.comune.trento.it/cartografia/gis/dbexport?db=base&sc=mobilita&ly=stazioni&fr=shp
- http://webapps.comune.trento.it/cartografia/gis/dbexport?db=base&sc=mobilita&ly=zone_parcheggio&fr=shp

The shapefiles have been included in this repository for convenience.

