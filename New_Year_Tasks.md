### Dashboard tasks at the beginning of each calendar year
1. Change date of 7-day sat. mean file generation (move up one day)
2. For sat. data extractions, run full extraction on all files to update the .mat files (needs to be less than 365 days behind current files)
3. Then, update the "time cut" in the MAT2CSV.M routines to reflect Jan. 1 and Dec. 31 respectively
4. All buoy data now comes from the SECOORA ERDDAP site. There is no longer the need to get updated .txt files directly from NDBC.

### 2025 Tasks
1. Document and create a flow chart.
2. Explore grafana geomap plugin (use test dashboard)
3. Bring FGB, FK and FWC boards current using new grafana version
4. Improve 7D MEAN scripts - scrub entire directory and then run ALL files (will remove stray non-7D files)


