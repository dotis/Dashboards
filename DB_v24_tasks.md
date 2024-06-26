### Dashboard processing tasks (6/6/24) - Data wiped from tpa_pgs

#### Existing items
1. Move to VSNPP for dashboards - stop MODA data on 12/31/22 (order and keep IOP files for entire MODA record)
2. New subscription for SEUS, VSNPP day/night (can we do with 1 subscription? - How to separate SSTN from SST?)
3. Stop MODA subscriptions (done) - Keep daytime MODA subscription for ABI even if data is suspect
4. Clean up and standardize routines in DB_v23 directory
5. How to setup script for 1-day "FL" files which go on ERDDDAP? - Currently just subsetting L3_1D files (because ERDDAP will not take files made w/gpt operator)
6. ERDDAP 1D files should be automated (need for July Walton Smith cruise)
 

#### Tasks to rebuild and streamline
#### Processing codes now on "/srv/homes/DB_files/DB_v24/"
1. New cron file on manglillo (copy over old cron from seashell) - How do 7D satellite means get to dune (Tylar's cron?)?
2. Note: bash scripts to ftp data from OB-DAAC are stored in home directory (these have been updated - currently 5 active subscriptions)
3. xml and CLIM files still in old locations - move to DB_v24 for all roi. XML files have been moved.
4. Merge GOM and SEUS code files
5. USGS - Recreate, need to find old USGS river data to merge w/new data
6. NDBC - Recreate, Streamline dods files
7. Process Rrs and IOP as separate streams for GOM only, leave SEUS for now, Mostafa will use Rrs in FL Keys
8. For VSNPP, nighttime sst is called "sstn" in L3 mosaiced files


### PRODUCT TABLE
G = GOM; S = SEUS  
MODA historical obs (2002 - 12/31/22) for all prods  
MODA subscriptions for OC only (ABI)
| MODA      |  L2_PASS  |  L3_1D  |   CLIM   | MEAN_7D |  ERDDAP | 
| --------- | --------- | ------- | -------- | ------- | ------- |
| OC        |   G,S     |    IP   |          |         |         |
| SST4      |   G,S     |         |          |         |         |
| SST       |   G,S     |         |          |         |         |
| IOP       |   G,S     |         |          |         |         |
| RRS       |   G,S     |         |          |         |         |
MODA OC prods: chlor_a, Rrs_667, ABI, Kd_490

All other dasshboard sat. products are from VIIRS
| VSNPP     |  L2_PASS  |  L3_1D  |   CLIM   | MEAN_7D | ERDDAP |         
| --------- | --------- | ------- | -------- | ------- | ------ |
| OC        |    G,S    |         |          |         |        |
| SSTN      |    G,S    |         |          |         |        |
| SST       |    G,S    |         |          |         |        |
| IOP       |    G,S    |         |          |         |        |
| RRS       |    G,S    |         |          |         |        |
VSNPP OC prods: chlor_a, Rrs_671, Kd_490

### MODA 250-m processing for Chelsea
| MODA-250  |     L2    |  L3_1D  |   CLIM?  |   MEAN?   |  
| --------- | --------- | ------- | -------- | --------- | 
| USVI      |           |         |          |           | 


### Buoys
#### SEUS
1. 41004 (Charleston): 1995-present (2013 is missing)
2. 41008 (GRNMS): 1997-present
3. 41112 (Fernandina): 2006-present
#### GOM
