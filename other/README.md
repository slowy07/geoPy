## tutorial how to using geopandas jupyter notebook
you need install package for import geopandas
```bash
!apt install gdal-bin python-gdal python3-gdal --quiet
!apt install python3-rtree --quiet
!pip install git+git://github.com/geopandas/geopandas.git --quiet
!pip install descartes --quiet
!pip install geopy
!pip install plotly_express
!pip install ipython-autotime
```

import pandas and geopandas
```python
import pandas as pd
import geopandas as gpd
import geopy
from geopy.geocoders import Nominatim
from geopy.extra.rate_limiter import RateLimiter
import matplotlib.pyplot as plt
import folium
from folium.plugins import FastMarkerCluster
#for importing geopandas and other
```
you can change the place
```python
locator = Nominatim(user_agent="myGeocoder")
location = locator.geocode("Monas, Jakarta, Indonesia") #place, city, country
```
for import csv to colab ipynb you need import code 
```python
from google.colab import files
data_to_load = files.upload()
```
and upload your csv files into colab and execute it
