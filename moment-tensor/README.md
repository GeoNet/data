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
Mxx, Mxy, Mxz, Myy, Myz, Mzz | moment tensor elements - scale 1E20 dyne.cm |
VR | percent variance reduction for solution |
Tva, Tpl, Taz | value, plunge and azimuth for tension axis |
Nva, Npl, Naz | value, plunge and azimuth for null axis |
Pva, Ppl, Paz | value plunge and azimuth for compression  axis. |
Method | method used to calculate solution (see table below for dates) |


Method ID | Dates Used
-------| -----------
1 | 2003/08/21 to 2020/06/18
2 | since 2020/06/19


### Notes:
- Moment tensor element scale is 1E20 dyne.cm, i.e. moment tensor elements need to be multiplied by 1E20 to convert to dyne.cm.
- The Dusky Sound (20090715092200) earthquake is the USGS W-phase solution as a reliable regional moment tensor solution could not be calculated.
- The Kaikoura (20161113110200) earthquake is the USGS W-phase solution as a reliable regional moment tensor solution could not be calculated.
- Event ID's with 9999999 are events for which no event ID is currently available.
- Beginning 5 September 2012 event ID/location/ML come from SeisComP3
- n/a values are for solutions from external agencies where the parameters were not available. 

## Moment Tensor Methods

### Method 1
Solutions calculated using code from Doug Dreger at Berkeley Seismological laboratory and documented in Ristau, J. (2013). 

### Method 2
Solutions are calculated using inversion code from Charles Ammon at Penn State University. Code is available from Hermann, R.B. (2013); http://www.eas.slu.edu/eqc/eqccps.html. All solutions since 18/06/2020 are calculated with this method, along with a number of past earthquakes. 

### Reference Papers

Ristau, J. (2013). "Update of Regional Moment Tensor Analysis for Earthquakes in New Zealand and Adjacent Offshore Regions". *Bulletin of the Seismological Society of America*., ***103***, 2520-2533. https://doi.org/10.1029/93JB00023

Herrmann, R. B. (2013). "Computer programs in seismology: An evolving tool for instruction and research", *Seism. Res. Lettr.* ***84***, 1081-1088. https://doi:10.1785/0220110096
