## MBON data dashboards

### Notes for 2026

#### New dashboard: REACH  
 - NE GoM
 - Will serve MODIS, VIIRS, PACE images, time series at sampling locations
 - Will use new grafana geomap plugin for map
 - Should add shapefile for Rice's Whale habitat
 - Other items to add to map: depth contours?
 - Use Quarto report for station data (species counts, phytopl. abs., etc.)


#### Update maps on other DB's to use geomap
Layers to add:
 - NMS bounds (shapefile)
 - Artificial reefs (SEUS - shapefile)
 - Discharge gauges (point data in CSV)
 - Buoy locations (point data in CSV)
 - NERR locations (point data in CSV)
 - Other shapefiles (COAST, Cumberland Is. Nat. Seashore, etc.)
 - Detailed view of Gray's REEF NMS (boundary, research area, benthic cover, buoy location)
 - Bathymetry?
 - Rivers, ports, state boundaries, etc.


For shapefiles, can convert to geojson in MATLAB, otherwise use CSV

### USGS API has been deprecated - need to update
Test URL for MissRv:

https://api.waterdata.usgs.gov/ogcapi/v0/collections/daily/items?f=csv&lang=en-US&limit=50000&properties=monitoring_location_id,parameter_code,statistic_id,time,value,unit_of_measure,approval_status&skipGeometry=true&sortby=%2Btime&offset=0&datetime=2000-01-01T00%3A00%3A00Z%2F..&monitoring_location_id=USGS-07374000&parameter_code=00060&statistic_id=00003

The API call above is working. Will need to modify for GH.

API docs are found here (can test and generate URL):
https://api.waterdata.usgs.gov/ogcapi/v0/openapi?f=html#/daily/getDailyFeatures

On the webpage, there is an option to "Download data", but I can't tell how to do that using the URL directly  

