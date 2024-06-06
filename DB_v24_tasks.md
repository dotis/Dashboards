### Dashboard processing tasks (6/6/24) - Data wiped from tpa_pgs

#### Existing items
1. Move to VSNPP for dashboards - stop MODA data on 12/31/22 (order and keep IOP files for entire MODA record)
2. New subscription for SEUS, VSNPP day/night (can we do with 1 subscription? - How to separate SSTN from SST?)
3. Stop MODA subscriptions (done)
4. Clean up and standardize routines in DB_v23 directory
5. How to setup script for 1-day "FL" files which go on ERDDDAP? - Currently just subsetting L3_1D files (because ERDDAP will not take files made w/gpt operator)
6. ERDDAP 1D files should be automated
 

#### Tasks to rebuild and streamline
#### Processing codes now on "/srv/homes/DB_files/DB_v24/"
1. New cron file on manglillo (copy over old cron from seashell)
2. xml and CLIM files still in old locations - move to DB_v24 for all roi
3. Merge GOM and SEUS code files
4. USGS - Recreate, need to find old USGS river data to merge w/new data
5. NDBC - Recreate, Streamline dods files
6. 








