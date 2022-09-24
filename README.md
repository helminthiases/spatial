<br>

[Geospatial Variables](#geospatial-variables)
 * [WaSH](#wash)
 * [Elevation](#elevation)
 * [Population Density](#population-density)

<br>
<br>

## Geospatial Variables

<br>

Remember, each observation of an ESPEN STH experiments data set - the data set of a country across years - includes the variables

<br>

variable | description
:--- | :---
iso2 | The ISO 3166-1 alpha-2 country code, i.e., the two-letter country code.
iso3 | The ISO 3166-1 alpha-3 country code, i.e., the three-letter country code.
admin1_id | A country's administrative division 1 code.
admin2_id | A country's administrative division 2 code.
longitude | The longitude geographic co&ouml;rdinate value.
latitude | The latitude geographic co&ouml;rdinate value.

<br>

and much more.  Due to the presence of the latitude & longitude values, we can extract feature value estimates from 
geospatial variable objects.  Hence, the focus herein is the derivation of features estimates of interest, per location 
within a STH ESPEN data set.  Initially, the features of interest are 

* WASH (water, sanitation, and hygiene) features.
* Population density.
* Elevation.

Future options include _land surface temperature_ and _enhanced vegetation index_.

<br>
<br>

### WaSH

The WaSH data is courtesy of [IHME WaSH](https://www.healthdata.org/research-article/mapping-geographic-inequalities-access-drinking-water-and-sanitation-facilities-low)


<br>
<br>

### Elevation

The list below summarises a set of [World Climate](https://worldclim.org/data/worldclim21.html) elevations maps.  The maps are
derivations/versions of the  [Shuttle Radar Topography Mission's](https://lpdaac.usgs.gov/products/srtmgl1v003/) elevation
maps.  In terms of the Soil Transmitted Helminths Project, elevation values per location are extracts from the **30 seconds map**.

* [30 seconds](https://biogeo.ucdavis.edu/data/worldclim/v2.1/base/wc2.1_30s_elev.zip)
* [2.5 minutes](https://biogeo.ucdavis.edu/data/worldclim/v2.1/base/wc2.1_2.5m_elev.zip)
* [5 minutes](https://biogeo.ucdavis.edu/data/worldclim/v2.1/base/wc2.1_5m_elev.zip)
* [10 minutes](https://biogeo.ucdavis.edu/data/worldclim/v2.1/base/wc2.1_10m_elev.zip)

The Shuttle Radar Topography Mission (SRTM) maps are explorable via  [earth explorer](https://earthexplorer.usgs.gov); 
try [Shuttle Radar Topography Mission (SRTM) 1 Arc-Second Global data/map](https://earthexplorer.usgs.gov).

<br>
<br>

### Population Density

* Repository: https://geodata.ucdavis.edu/geodata/pop

The population data is courtesy of [Socioeconomic Data & Applications](https://sedac.ciesin.columbia.edu/data/collection/gpw-v4/documentation).  Its map collection 
resides at [population density data details](https://sedac.ciesin.columbia.edu/data/collection/gpw-v4/whatsnew).  These maps are accessible via the ``r`` library
[`geodata`](https://github.com/rspatial/geodata#data).

Additionally, UC Davis stores copies of these map: [population density data](https://geodata.ucdavis.edu/geodata/pop/)

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>