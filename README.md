# grib-tables

This tables are dumped from https://ftp.cpc.ncep.noaa.gov/wd51we/wgrib2/grib2/wgrib2/gribtables/

Access with pygrib likes ->

```python
raw = pygrib.index(filename, 'parameterCategory', 'parameterNumber')

# For example, EXNPR on KMA GRIB2

EXNPR = raw.select(parameterCategory=3, parameterNumber=192)

# Your codes
```
