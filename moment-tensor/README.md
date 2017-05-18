# Moment Tensors

The moment tensor solution describes the source mechanism of an earthquake - the geometry of how the fault ruptured in the earthquake. 

Once the required broadband seismometers were deployed, GeoNet has been able to compute moment tensor solutions for earthquakes since August 2003 for moderate (magnitude >4) earthquakes. These are not currently integrated with QuakeML output from the earthquake catalogue. At the moment these are computed manually and the csv is updated shortly afterwards. 

Fields | Description |
-------| ----------- |
EVENT_ID | CUSP/SeisComP3 event ID |
Date | yyyymmddhhmm00 |
Latitude/Longitude | epicentre latitude and longitude |
strike1/dip1/rake1 | strike/dip/rake of nodal plane 1 |
strike2/dip2/rake2 | strike/dip/rake of nodal plane 2 |
ML | local magnitude |
Mw | moment magnitude |
Mo | seismic moment (dyne.cm) |
CD | centroid depth (km) |
NS | number of stations used to calculate solution |
DC | percent double-couple |
Mxx, Mxy, Mxz, Myy, Myz, Mzz | moment tensor elements |
VR | percent variance reduction for solution |
Tva, Tpl, Taz | value, plunge and azimuth for tension axis |
Nva, Npl, Naz | value, plunge and azimuth for null axis |
Pva, Ppl, Paz | value plunge and azimuth for compression  axis. |

### Notes:
- The Dusky Sound (20090715092200) earthquake is the USGS W-phase solution as a reliable regional moment tensor solution could not be calculated.
- The Kaikoura (20161113110200) earthquake is the USGS W-phase solution as a reliable regional moment tensor solution could not be calculated.
-  Event ID's with 9999999 are events for which no event ID is currently available.
-  Beginning 5 September 2012 event ID/location/ML come from SeisComP3
-  n/a values are for solutions from external agencies where the parameters were not available. 
