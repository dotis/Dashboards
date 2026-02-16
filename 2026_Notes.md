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

https://waterdata.usgs.gov/monitoring-location/USGS-07374000/#dataTypeId=daily-00060-0&period=periodOfRecord&showFieldMeasurements=false&format=rdb,1.0

This seems to work, but leads to a webpage.  

On the webpage, there is an option to "Download data", but I can't tell how to do that using the URL directly  

