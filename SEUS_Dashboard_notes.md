## SEUS Dashboard Notes    
### For details on workflows for all boards go here: 
https://github.com/USF-IMARS/l2-processing/edit/main/documentation/DB_v2023_processing.md

### USGS Discharge

Stations:
1. Gray's Reef
- USGS 02228295 CUMBERLAND SOUND AT SEA CAMP DOCK, NR ST MARYS, GA
- USGS 02226180 BRUNSWICK RIVER AT ST. SIMONS ISLAND, GA
- USGS 022035975 HUDSON CREEK AT MERIDIAN LANDING, NEAR MERIDIAN,GA (Has a lot of WQ params! - DO, Turb, Sal, pH)
2. Monitor
- USGS 02084472 PAMLICO RIVER AT WASHINGTON, NC (Has WQ params - DO, Sal, pH)
- USGS 02108566 NORTHEAST CAPE FEAR R NR BURGAW, NC  (Has WQ params - DO, Sal, pH)
- USGS 02105769 CAPE FEAR R AT LOCK 1 NR KELLY, NC (Has WQ params - DO, Sal, pH)
- USGS 0209205053 SWIFT CREEK AT HWY 43 NR STREETS FERRY, NC
- USGS 02106500 BLACK RIVER NEAR TOMAHAWK, NC
- USGS 02093000 NEW RIVER NEAR GUM BRANCH, NC

### NBDC Buoys
Gray's Reef
Station 41008 (met only)

### NERRS WQ
NERRS current data - All files are kept in /srv/imars-objects/tpa_pgs/rois/seus/NERRSWQ_tmp
1. Sap Island SAQG1 (sapldq - Lower Duplin) Last 45 days of data (https://www.ndbc.noaa.gov/data/realtime2/SAQG1.ocean - file is good)
  - 6 params (1999-present) - Temp,Sal,DO_mgl,Depth,pH,Turb
  - Sapelo Island National Estuarine Research Reserve
2. ACE Basin ACQS1 (acegp - Grove Plantation) Last 45 days of data (https://www.ndbc.noaa.gov/data/realtime2/ACQS1.ocean - file is good)
  - 6 params (2016-present) - Temp,Sal,DO_mgl,Depth,pH,Turb
  - Ashepoo-Combahee-Edisto (ACE) Basin National Estuarine Research Reserve
3. Winyah Bay WYSS1 (niwws - Winyah Bay Surface) - Last 45 days of data (https://www.ndbc.noaa.gov/data/realtime2/WYSS1.ocean - file is good)
  - 7 params (2016-present) - Temp,Sal,DO_mgl,Depth,pH,Turb,ChlFluor
  - North Inlet-Winyah Bay National Estuarine Research Reserve
4. Zeke's Basin ZBQN7 (noczb - Zekes's Basin) Last 45 days of data (https://www.ndbc.noaa.gov/data/realtime2/ZBQN7.ocean - file is empty)
  - 7 params (2002-present) - Temp,Sal,DO_mgl,Depth,pH,Turb,ChlFluor
  - North Carolina National Estuarine Research Reserve
5. GuanTM GTQF1 (gtmpc - Pellicer Creek) Last 45 days of data (https://www.ndbc.noaa.gov/data/realtime2/GTQF1.ocean - file is truncated; only showing a few hours of data)
  - 7 params (2001-present) - Temp,Sal,DO_mgl,Depth,pH,Turb,ChlFluor(starts late)
  - Guana Tolomato Matanzas National Estuarine Research Reserve

loc_IDs={'sapldq','acegp','niwws','noczb','gtmpc'};

### Meeting w/Jen D, Chris S and Tylar M on 8/16/23
GRNMS interests:
1. Nutrient fluxes and WQ from NERRS sites (SAP, ACE, GUANTM)
    a. Nutrients are only updated annually
2. Connectivity from shore to reef (winds? currents?)
3. Boat Traffic
4. Bathymetry features and how they affect conditions.

### Questions on NERRS WQ data
1. Which station(s) at each NERR to use (there are at least four stations at each NERR)
   a. Plot, map and compare - show to GR staff
2. How to grab data? - Grab recent data only and merge w/historical data? - Ask Melissa
3. How to request w/XML protocol? - Ask Tylar
4. Start w/Sapelo, ACE and GUANTM
5. Compare to USGS

   
