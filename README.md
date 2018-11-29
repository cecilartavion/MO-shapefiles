# Missouri Election Shapefile
This shapefile was compiled by the Harvard Election Data Archive and processed by members of the Voting Rights Data Institute. The Voting Rights Data Institute (VRDI) was a 2018 summer intensive sponsored by the Metric Geometry and Gerrymandering Group (MGGG) at Tufts and MIT, with major support from a Bose Research Grant at MIT and from the Jonathon M. Tisch College of Civic Life at Tufts.

## Sources
The raw, unprocessed shapefile comes from the Harvard Election Data Archive’s Missouri Data Files created in 2011 by Stephen Ansolabehere and Jonathan Rodden (available for download at https://dataverse.harvard.edu/dataset.xhtml?persistentId=hdl:1902.1/16795).

## Processing
The original shapefile was modified by members of VRDI so that it could be used in MGGG’s GerryChain. Nested precincts were merged into each other manually in QGIS.

## Metadata
- `STATEFP10`: State FIPS code
- `COUNTYFP10`: County FIPS code
- `VTDST10`: Voting tabulation district FIPS code
- `GEOID10`: VTD FIPS code
- `VTDI10`: 2010 Census voting district indicator
- `NAME10`: Voting tabulation district name
- `NAMELSAD10`: Translated statistical area description code
- `LSAD10`: 2010 Census legal/statistical area description code for voting district
- `MTFCC10`: MAF/TIGER feature class code
- `FUNCSTAT10`: 2010 Census functional status
- `ALAND10`: Area land (square meters)
- `AWATER10`: Area water (square meters)
- `INTPTLAT10`: Latitude of internal point
- `INTPTLON10`: Longitude of internal point
- `POP100`: Total population from 2010 Census
- `VAP`: Voting age population, or population over the age of 18, from 2010 Census
- `COUNTY`: County name
- `PR_RV08`: Number of votes for 2008 Republican presidential candidate
- `PR_DV08`: Number of votes for 2008 Democratic presidential candidate
- `PR_OTHV08`: Number of votes for 2008 other presidential candidates
- `USH_DV08`: Number of votes for 2008 Democratic US House candidate
- `USH_RV08`: Number of votes for 2008 Republican US House candidate
- `GOV_DV08`: Number of votes for 2008 Democratic gubernatorial candidate
- `GOV_RV08`: Number of votes for 2008 Republican gubernatorial candidate
- `LG_RV08`: Number of votes for 2008 Republican lieutenant governor candidate
- `LG_DV08`: Number of votes for 2008 Democratic lieutenant governor candidate
- `SS_DV08`: Number of votes for 2008 Democratic secretary of state candidate
- `SS_RV08`: Number of votes for 2008 Republican secretary of state candidate
- `TR_OTHV08`: Number of votes for 2008 other treasurer candidates
- `TR_DV08`: Number of votes for 2008 Democratic treasurer candidate
- `TR_RV08`: Number of votes for 2008 Republican treasurer candidate
- `AG_RV08`: Number of votes for 2008 Republican attorney general candidate
- `AG_DV08`: Number of votes for 2008 Democratic attorney general candidate
- `GOV_OTHV08`: Number of votes for 2008 other gubernatorial candidates
- `LG_OTH08`: Number of votes for 2008 other lieutenant governor candidates
- `SS_OTHV08`: Number of votes for 2008 other secretary of state candidates
- `P_08`: 2008 presidential two-party vote share
- `USH_08`: 2008 US House two-party vote share
- `GOV_08`: 2008 gubernatorial two-party vote share
- `TR_08`: 2008 treasurer two-party vote share
- `AG_08`: 2008 attorney general two-party vote share
- `LG_08`: 2008 lieutenant governor two-party vote share
- `AV`: Average two-party vote over all offices
- `NDV`: Normal vote for Democrats, computed as AV*2008 total presidential votes
- `NRV`: Normal vote for Republicans, computes as (1-AV)*2008 total presidential votes
- `CD`: Congressional district number

## Projection
This shapefile uses a WGS 84 UTM Zone 15N projection (EPSG:32615).

## Rating
We give this shapefile a C rating. As Jonathan Rodden states in the Missouri notes (available here: https://dataverse.harvard.edu/dataset.xhtml?persistentId=hdl:1902.1/16795), Missouri is a notoriously difficult state to collect reliable election data for below the county level. After the 2008 election the Harvard Election Data Archive had to contact election officials from individual municipalities to compile both tabular results and geodata. While this is the best election shapefile that exists publicly for Missouri, it is now at least six years out of date and is potentially unreliable in some places.
