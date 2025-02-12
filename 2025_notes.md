#### Dashboard notes for 2025

Issues:
1. MODIS will end soon
 - Depracate new file ingests (end on 12/31/22)
2. Continue VIIRS-SNPP production
3. Operationalize PACE production (need for nflh)
 - Get files via CMR (OBPG subscriptions will end at some point)
 - Two filestreams: AOP and BGC. Could also add IOP.
 - How to get recent files w/bash scripting (ask Tylar)?
 - Need to clean up the bash scripts
 - Climatologies for PACE? - Use one year, or use MODIS?
 - nflh is part of the "AOP" filestream
 - Two file collections in CMR: Normal and "NRT", which goes about a month back in time
 - Need to periodically download the older "non-NRT" files 
PACE products to serve:
 - Rrs
 - nflh
 - chlor_a
 - Rrs_665 (susp. sed. proxy)
 - Kd_490
