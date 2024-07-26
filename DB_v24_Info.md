### Dashboard processing tasks (6/6/24) - Data wiped from tpa_pgs

#### Existing items
1. Move to VSNPP for dashboards - stop MODA data on 12/31/22 (order and keep IOP files for entire MODA record)
2. ERDDAP 1D files should be automated (need for July Walton Smith cruise)
3. ERDDAP files - 1D and 7D means now have yyyyMMdd date format, change in dataset.xml files and reload dune w/new files
 

### Tasks to rebuild and streamline
#### Processing codes now on "/srv/homes/DB_files/DB_v24/"

### Dashboard satellite products to serve on IMaRS ERDDAP  
Do we need to even serve MODA and VSNPP SST? Why not serve only OC/IOP and use GHRSST MUR SST?  
However. these are daily (not available weekly)  
Why does IMaRS ERDDAP show max dates a few days behind source ERDDAP (NOAA Coastwatch)  

#### GOM
1. MODA OC 2002-present (chlor_a, Rrs_667, ABI, Kd_490 - w/R2022.0.1 correction) 
2. VSNPP OC (chlor_a, Rrs_671, Kd_490)
#### SEUS
1. MODA OC 2002-present (chlor_a, Rrs_667, ABI, Kd_490 - w/R2022.0.1 correction)
2. VSNPP OC (chlor_a, Rrs_671, Kd_490)

### Buoys (via SECOORA ERDDAP)
#### SEUS (STD_MET)
1. 41004 (Charleston): 1995-present (2013 is missing)
2. 41008 (GRNMS): 1997-present
3. 41112 (Fernandina): 2006-present
#### GOM (TEMP/SAL)
1. Bob Allen Key
2. Butternut Key
3. Little Rabbit Key
4. Peterson Key
5. Whipray Basin



