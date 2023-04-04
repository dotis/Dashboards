## Outstanding tasks for L2 processing and dashboards

### L2 processing status
### Moving to using only GOM as an ROI (will remove FK and FGB)


| MODA      |   L3_1D   |  CLIM   |  MEAN_7D |  MEAN_8D? |  ERDDAP | 
| --------- | --------- | ------- | -------- | --------- | ------- |
| OC        |   done    |  done   |   need   |   need?   |    ?    |
| SSTN      |   done    |  done   |   done   |   need?   |    ?    |
| SST       |  working  |  need   |   need   |   need?   |   need  |
| RRS       |   need    |  need   |   need   |   need?   |   need  |
MODA prods: chlor_a, Rrs_667, ABI, Kd_490


| VSNPP     |   L3_1D   |  CLIM   |  MEAN_7D |  MEAN_8D? |  ERDDAP | 
| --------- | --------- | ------- | -------- | --------- | ------- |
| OC        |   done    |  done   |   need   |    need   |   need  |
| SSTN      |   done    |  done   |   need   |    need   |   need  |
| SST       |  working  |  need   |   need   |    need   |   need  |
| RRS       |   need    |  need   |   need   |   need?   |   need  |
VSNPP prods: chlor_a, Rrs_671, Kd_490

### MODA 250-m processing for CoPE and BG 
### Make OC L2/L3 at 250-m for Rrs_667
### Make IOP/OC L2/L3 at 1-km for chl, adg, apg
### Make L3 SSTN at 1-km - order L2
| MODA-250  |     L2    |  L3_1D  |   CLIM?  |   MEAN?   |  
| --------- | --------- | ------- | -------- | --------- | 
| TB        |  done     |  need   |   need?  |   need?   |
| USVI      |  done     |  need   |   need?  |   need?   | 
| BEL       | waiting   |  need   |   need?  |   need?   | 


### Outstanding tasks:
1. Run MODA and VSNPP for GOM(OC and SST4/N first)
2. Run new CLIMs for GOM OC and SST with all prods; SST4 is done); need CLIMs for all VSNPP
3. Check ERDDAP status for GOM datasets
4. Convert sat. data extraction routines to use GOM roi. Combine (and reduce) FK and FGB extraction points/polys.
5. Push files needed for dashboards to git using upload_files.sh (this is working, just need to push the correct files once converted to GOM).
6. Add Rrs vis products to GoM product suite (separate files w/Rrs at viz bands)
