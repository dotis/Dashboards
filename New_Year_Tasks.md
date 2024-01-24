### Dashboard tasks at the beginning of each calendar year
1. Change date of 7-day sat. mean file generation (move up one day)
2. For sat. data extractions, run full extraction on all files to update the .mat files
3. Then, update the "time cut" in the MAT2CSV.M routines to reflect Jan. 1 and Dec. 31 respectively
4. Need to add new year to list of files for SEUS dash for 41008 Gray's Reef buoy. This routine needs to be streamlined. The 2024 .nc file is not ready. The 2023 file is complete, but is still on a 10 minute time interval. At some point, the 2023 1-hour file will become available along with the 2024 10-min file. Check periodically and make this switch. There has to be a better way(?!?)

### 2024 Tasks
1. Clean up routines! - move all to DBv23 directory
2. In particular, NDBC and USGS routines need to be made consistent. .nc files should be named X.nc (not X.txt!)
3. Put obsolete routines in "old" directory
4. If NERRS data cannot be accessed using Tylar's method, move to NDBC and append to files downloaded from CDMO.
5. Document and create a flow chart.

