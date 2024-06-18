### Documentation for Grafana dashboards (FGBNMS, FKNMS, FWC, SEUS)

Main directory for code (MATLAB and bash scripts):    
/srv/imars-objects/homes/dotis/DB_files/DB_v24/  

### Data directories:  
GOM (FGBNMS, FKNMS and FWC):   
/srv/imars-objects/tpa_pgs/rois2/gom  

SEUS (GRNMS - could add others, like Monitor):     
/srv/imars-objects/tpa_pgs/rois2/seus   

### Satellite data  
TODO

### USGS River data (discharge and gage height)  
Single bash script to download data and run ML scripts which generate .csv files  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/cron_USGS_disch_gh_dbv24.sh" 

Three subsequent ML scripts to generate .csv files for individual dashboards  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_FGB_dbv24.m"  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_FK_dbv24.m"  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_SEUS_dbv24.m"  

### NDBC Buoy data (temperature, salinity, meteorological and wave data)  
Single bash script to get current year and last 45 days of data (these need to be merged to each other and to historical data)  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/cron_NDBC_buoys_dbv24.sh"  

#### Meteorological and wave data


#### Temperature and Salinity data (NPS buoys in Florida Bay)
In process: Try to set up curl calls to SECOORA URL to get all temp and salinity data without needing to merge  



### OUTPUT
.csv file output is written to the following directories:  
All .csv output goes here - satellite time series, river discharge, NDBC buoy data, etc.  
/srv/imars-objects/tpa_pgs/rois2/gom/csv_ts_data/data/  
/srv/imars-objects/tpa_pgs/rois2/seus/csv_ts_data/data/  

#### All .csv output files need to be pushed to the Google data bucket, which is done via cron by Tylar Murray at root level  




