### Documentation for Grafana dashboards (FGBNMS, FKNMS, FWC, SEUS/GRNMS)

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
Single bash script to download data and run ML scripts below which generate .csv output files  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/cron_USGS_disch_gh_dbv24.sh" 

Three subsequent ML scripts to generate .csv files for individual dashboards (called by bash script above)  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_FGB_dbv24.m"  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_FK_dbv24.m"  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/TXT2CSV_USGS_SEUS_dbv24.m"  


### NDBC Buoy data (temperature, salinity, meteorological and wave data)  
Single bash script to get current year and last 45 days of data (these need to be merged to each other and to historical data)  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/cron_NDBC_buoys_dbv24.sh"  

#### Meteorological and wave data
These data come in three separate streams, which must be merged
1. Historical: raw .nc ("dods") files for each year prior to current year
2. Current year data in .nc format
3. Last 45 days data comes as a text file.
API links to these files are found in the .sh file above ("cron_NDBC_buoys_dbv24.sh")

Intermediate directories:  
Historical raw data data (.nc files):  
/srv/imars-objects/tpa_pgs/rois2/gom/NDBC_temp/historical_nc_raw  
Current year and last 45 days data:  
/srv/imars-objects/tpa_pgs/rois2/gom/NDBC_temp/

ML script to download raw .nc files for a particular buoy:  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/NDBC_dods_download_loop.m"   

Two ML scripts to convert raw .nc files to .csv
Historical (this script only needs to be run at the beginning of each calendar year when new "dods" files become available:
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/NC2CSV_SEUS_NDBC_dbv24_stdmet_Historical.m"   

Current year and last 45 days:
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/NC2CSV_SEUS_NDBC_dbv24_stdmet_Current.m"    

ML script to append "Current" data file to "Historical" data file:  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/NDBC_SEUS_APPEND.m" 

#### Temperature and Salinity data (NPS buoys in Florida Bay)
ML script to get recent temp/sal data:  
"/srv/imars-objects/homes/dotis/DB_files/DB_v24/NC2CSV_NDBC_FK_TEMPSAL_dbv24.m"  


In process: Set up curl calls to SECOORA URL to get all temp and salinity data without needing to merge  



### OUTPUT
.csv file output is written to the following directories:  
All .csv output goes here - satellite time series, river discharge, NDBC buoy data, etc.  
/srv/imars-objects/tpa_pgs/rois2/gom/csv_ts_data/data/  
/srv/imars-objects/tpa_pgs/rois2/seus/csv_ts_data/data/  

#### All .csv output files need to be pushed to the Google data bucket, which is done via cron by Tylar Murray at root level  




