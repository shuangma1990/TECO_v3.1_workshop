# TECO_v3.1_workshop
TECO_2.3 is developed based on the older versionTECO_2.2 used in the workshop in 2019.
The main updates of 2.3 is:
1. The complete freedom of choosing which parameters to constrain (9 soil-thermal-dynamic parameters newly added) upon your interest;
2. The complete freedom of using observation data streams to do DA for Carbon, or soil water, or soil temperature, snow depth, water table, or any combinations. (assign value to these logical terms in the name list file: do_co2_da; do_soilwater_da; do_soilt_da; do_snow_da; do_watertable_da;)
3. Added carbon balance equation at the end of methane module, to explicitly match the model output NEE to the observed NEE (in form of CO2 only). To calculate net C loss, add up NEE and CH4 emission.
4. use_xx_ob and obsfile_xx terms in the nameless should be always be assigned at the same time, the former term decides whether use (eg. cflux) observation or not for any DA of your choice, the later term points to the directory of observation file.


TECO_2.31 corrected dimension warning in the soil energy module when calculating temph2. 
