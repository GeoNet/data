# GNS Science Aotearoa New Zealand Earthquake Rupture Models 

The GNS Aotearoa New Zealand Earthquake Rupture Models dataset is a collection of rupture models for regional events.Currently, this repository contains 20 rupture modelsfrom 14 number of events.

A rupture model comprises a spatiotemporal description of the rupture process during an earthquake inferred from source inversion of either seismic recordings, geodetic measurements, or both. These models were provided by seismologists (authors) from GNS and other institutes worldwide. This repository is organized into directories (or folders) and sub-directories (or subfolders). The adopted structure puts the specific files according to events, authors of the rupture models, and multiple rupture models for the same event.

The following lists the earthquakes.

| Date       | Event                     | PublicID                                 |
| ---------- | ------------------------- | ---------------------------------------- |
| 05/03/2021 | [East Cape M7.3](20210305-east-cape)                | [2021p169083](https://www.geonet.org.nz/quakes/region/newzealand/2021p169083)
| 14/11/2016 | [Kaikoura M7.9](20161114-kaikoura)                | [2016p858000](https://www.geonet.org.nz/quakes/region/newzealand/2016p858000)
| 14/02/2016 | [Christchurch M5.7](20160214-christchurch)                | [2016p118944](https://www.geonet.org.nz/quakes/region/newzealand/2016p118944)
| 20/01/2014 | [Eketahuna M6.3](20140120-eketahuna)                | [2014p051675](https://www.geonet.org.nz/quakes/region/newzealand/2014p051675)
| 16/08/2013 | [Lake Grassmere M6.6](20130816-lake-grassmere)                | [2013p051675](https://www.geonet.org.nz/quakes/region/newzealand/2013p051675)
| 21/07/2013 | [Cook Strait M6.6](20130721-cook-strait)                | [2013p543824](https://www.geonet.org.nz/quakes/region/newzealand/2013p543824)
| 23/12/2011 | [Christchurch M6.1](20111223-christchurch)                | [3631380](https://www.geonet.org.nz/quakes/region/newzealand/3631380) and  [3631359](https://www.geonet.org.nz/quakes/region/newzealand/3631359)
| 13/06/2011 | [Christchurch M6.0](20110613-christchurch)                | [3528839](https://www.geonet.org.nz/quakes/region/newzealand/3528839)
| 22/02/2011 | [Christchurch M6.2](20110222-christchurch)                | [3468575](https://www.geonet.org.nz/quakes/region/newzealand/3468575)
| 04/09/2010 | [Darfield M7.2](20100904-darfield)                | [3366146](https://www.geonet.org.nz/quakes/region/newzealand/3366146)
| 15/07/2009 | [Dusky Sound M7.8](20090715-dusky-sound)                | [3124785](https://www.geonet.org.nz/quakes/region/newzealand/3124785)
| 20/12/2007 | [Gisborne M6.6](20071220-gisborne)                | [2839343](https://www.geonet.org.nz/quakes/region/newzealand/2839343)
| 15/10/2007 | [George Sound M6.7](20071015-george-sound)                | [2808298](https://www.geonet.org.nz/quakes/region/newzealand/2808298)
| 21/08/2003 | [Fiordland M7.2](20030821-fiordland)                | [2103645](https://www.geonet.org.nz/quakes/region/newzealand/2103645)


### File Formats

Each file for a rupture model will necessarily have the following:
- Slip (preferably in m or cm).
- Geographical coordinates: Latitude (in degrees), Longitude (in degrees),and Depth (in km) for the slip patches (or sub-faults).

More complete data for the rupture model will include:
- Rise time,  i.e.,  the slip duration at each point on the rupture plane)
- Rupture onset time (or simply, rupture time), i.e.,  the relative time when slip is initiated at a point on the rupture plane.
- In case of multi-window inversions, slip information for each time window.

The file formats curently available include CSV, FSP, and MAT.
- CSV format lists the rupture parameters in a comma-separated tabulated format.
- FSP (or Finite Source Parameters).
- MAT (which is Matlab structure format).

FSP and MAT are standard formats used in the SRCMOD database - a global repository of earthquake source models. More details can be found on the equake-rc site: 
[SRCMOD File Formats](http://equake-rc.info/SRCMOD/fileformats/).

Meta data for each model can be found in the FSP file and is also provided separate (model.meta) file. The metadata for a rupture model can include:
- Specific region, and Date (Month, Day, and Year) of the event.
- Magnitude (in Mw scale) and seismic moment (in Nm).
- Epicentral location (latitude and longitude in degrees).
- Hypocentral depth (in km).
- Focal mechanism with strike, dip, and rake angles in degrees.
- A very short description of the data used in the inversion.
- Inversion specific settings such as source time function,number and length of time windows, crustal structure, and spatial gridding.
- Number of fault segments or faults.
- Data sources such as external websites, supplementary to a published article, emailed by the authors, etc.
- Wherever information is not available, the entries are made to indicate that to the users (e.g., using ‘NaN’).
- Citation and reference.

The metadata file is written in the [TOML format](https://toml.io/en/).

### Disclaimer

These rupture models were either extracted from publications or submitted to us in electronic formats by the authors.These submissions may be inconsistent with coresponding publications, as they may be updated by the authors using new data or improved inversion technique.

NZ Earthquake Rupture Model is an outcome of effort to compile all data and meta-data  as completely and accurately as possible. In cases where parameters are not located/provided, we report them as <i> NaN</i> indicating  unknown.Please note that this repository vouches neither the veracity nor reliability of the rupture models, and also, the scientific rigor of the rupture models with respect to the actual rupture process of the earthquakes.

### Usage

The users should verify that the data are appropriate and accurate enough for their study.

Please cite this repository as follows:

GNS Science (2025). GNS Science Aotearoa New Zealand Earthquake Rupture Models Dataset. GNS Science, GeoNet. https://doi.org/10.21420/396B-3Y58

### Reference Papers for the Rupture Models

- Beavan J, Motagh M, Fielding E, Donnelly N, Collett D, 2012. Fault slip models of the 2010-2011 Canterbury, New Zealand, earthquakes from geodetic data, and observations of post-seismic ground deformation, New Zealand Journal of Geology and Geophysics 55(3). doi:10.1080/00288306.2012.697472
- Beavan, J., Samsonov, S., Denys, P., Sutherland, R., Palmer, N. and Denham, M., 2010. Oblique slip on the Puysegur subduction interface in the 2009 July MW 7.8 Dusky Sound earthquake from GPS and InSAR observations: implications for the tectonics of southwestern New Zealand. Geophysical Journal International, 183(3), pp.1265-1286.
- François-Holden, C., Bannister, S., Beavan, J., Cousins, J., Field, B., McCaffrey, R., McVerry, G., Reyners, M., Ristau, J. and Samsonov, S. (2008). "The Mw 6.6 Gisborne earthquake of 2007: Preliminary records and general source characterisation". Bulletin of the New Zealand Society for Earthquake Engineering, 41(4), 266-277, https://doi.org/10.5459/bnzsee.41.4.266-277.
- Hamling, I.J., D Anastasio, E., Wallace, L.M., Ellis, S., Motagh, M., Samsonov, S., Palmer, N. and Hreinsdóttir, S., 2014. Crustal deformation and stress transfer during a propagating earthquake sequence: The 2013 Cook Strait sequence, central New Zealand. Journal of Geophysical Research: Solid Earth, 119(7), pp.6080-6092.
- Holden (unpublished), also see Van Houtte, C., Bannister, S., Holden, C., Bourguignon, S. and McVerry, G., 2017. The New Zealand strong motion database. Bulletin of the New Zealand Society for Earthquake Engineering, 50(1), pp.1-20.
- Holden, C., Kaneko, Y., D Anastasio, E., Benites, R., Fry, B. and Hamling, I. (2017) The 2016 Kaikoura Earthquake Revealed by Kinematic Source Inversion and Seismic Wavefield Simulations: Slow Rupture Propagation on a Geometrically Complex Crustal Fault Network. Geophysical Research Letters, http://dx.doi.org/10.1002/2017GL075301.
- Kaiser, A., Holden, C., Hamling, I., et al. (2016). The 2016 Valentine Day Mw5.7 Christchurch earthquake: preliminary report. In Proceedings of Conference of the New Zealand Society for Earthquake Engineering, Paper number O-20, Christchurch, New Zealand, 1-3 April 2016.
- McGinty, P. and Robinson, R. (2007). The 2003 Mw 7.2 Fiordland subduction earthquake, New Zealand: aftershock distribution, main shock fault plane and static stress changes on the overlying Alpine Fault. Geophysical Journal International, 169(2), 579-592, https://doi.org/10.1111/j.1365-246X.2007.03336.x.
- Okuwaki, R., Hicks, S.P., Craig, T.J., Fan, W., Goes, S., Wright, T.J. and Yagi, Y., 2021. Illuminating a contorted slab with a complex intraslab rupture evolution during the 2021 Mw 7.3 East Cape, New Zealand earthquake. Geophysical Research Letters, 48(24), p.e2021GL095117.
- Petersen, T., Ristau, J., Beavan, J., Denys, P., Denham, M., Field, B., François-Holden, C., McCaffrey, R., Palmer, N., Reyners, M. and Samsonov, S., 2009. The Mw 6.7 George Sound earthquake of October 15, 2007: response and preliminary results. Bulletin of the New Zealand Society for Earthquake Engineering, 42(2), pp.129-141.