## Explanation of columns in flatfiles

| Column name  | Description   |
| ------------- | ------------- |
| CuspID | GeoNet event identification number |
| Origin time    | Origin time of earthquake in UTC  |
| Record | Record name |
| Mw | Moment magnitude |
| MwUncert | Uncertainty in moment magnitude estimate |
| TectClass | Tectonic classification, either 'crustal', 'interface' or 'slab' |
| Mech | Focal mechanism, as defined by McVerry et al., (2006)
| | S → strike-slip, with rake angle δ, −33 ≤ δ ≤ 33, 147 ≤ δ ≤ 180, −180 ≤ δ ≤ −147 |
| | N → normal, −146 ≤ δ ≤ −34 |
| | R → reverse, 67 ≤ δ ≤ 123 |
| | O → oblique with a reverse component, 34 ≤ δ ≤ 66, 124 ≤ δ ≤ 146 |
| | U → unknown |
| PreferredFaultPlane | 1 if one fault plane orientation is preferred out of the two conjugate fault planes in the moment tensor |
| | 0 if the preferred fault plane is unknown |
| Strike | Strike angle (degrees)|
| | If PreferredFaultPlane = 1, this is the likely fault strike, otherwise it is only one of two possible strikes |
| Dip | Dip angle (degrees) |
| Rake | Rake angle (degrees) |
| Location | Reference for the preferred location |
| | special → special studies (see references)
| | geonet → standard GeoNet catalogue |
| | nlloc → relocation using the NonLinLoc algorithm |
| | simulps → relocation using the SimulPS algorithm |
| | irisdmc → the IRIS DMC catalogue (mostly for older events) |
| HypLat | Hypocenter latitude |
| HypLon | Hypocenter longitude |
| StationLat | Latitude of recording station |
| StationLon | Longitude of recording station |
| HypN | Northing of hypocenter in NZMG co-ordinates (metres) |
| HypE | Easting of hypocenter in NZMG co-ordinates (metres) |
| StationN | Northing of recording station in NZMG co-ordinates (metres) |
| StationE | Easting of recording station in NZMG co-ordinates (metres) |
| LENGTH_km | Inferred rupture length along strike (km) |
| WIDTH_km | Inferred down-dip rupture width (km) |
| Repi_km | Epicentral distance (km) |
| Rhyp_km | Hypocentral distance (km) |
| Rjb_km | Joyner-Boore distance (km) |
| Rrup_km | Closest distance from station to rupture plane (km) |
| Rx_km | Hanging wall distance metric Rx (km) |
| Ry_km | Hanging wall distance metric Ry (km) |
| Rvol_km | Volcanic path distance (km) |
| HypDepth_km | Hypocenter depth (km) |
| ZTOR_km | Depth to top of rupture plane (km) |
| HWFW | Hanging wall flag |
| | hw → Station located on hanging wall |
| | fw → Station located on foot wall |
| | nu → No hanging wall effects |
| SiteCode | GeoNet station identifier |
| SiteClass1170 | NZS1170.5:2004 site classification |
| Vs30 | Time-averaged shear-wave velocity in the top 30 m (m/s) |
| Vs30Uncert | Quality of V<sub>S30</sub> estimate |
| Tsite | Low-strain fundamental site period (s) |
| TsiteUncert | Quality of T<sub>site</sub> estimate |
| Z1 | Depth below ground surface to a shear-wave velocity of 1 km/s (m) |
| Z1Uncert | Quality of Z<sub>1</sub> estimate |
| Directivity | Identified directivity pulse |
| | 1 → pulse-like motions have been identified |
| | 0 → pulse-like motions have not been identified |
| Pulse_or | Orientation of identified directivity pulse |
| | either equals the component orientation in degrees, or -99999 if not applicable |
| Pulse_T | Period of identified directivity pulse |
| | either equals the period in seconds, or -99999 if not applicable |
| S_Trigger_Flag | Flag indicating whether the recording triggered between the P and S arrivals |
| | 1 → the recording triggered after the P-arrival (beginning of recording may not be captured) |
| | 0 → a clear P-arrival was observed |
| fcButterHP | Corner frequency of Butterworth high-pass filter (Hz) |
| finiLP | Initiation frequency of the low-pass sinuosoidal transition filter (Hz) |
| fmin | Minimum usable frequency of the recording (Hz) |
| fmax | Maximum usable frequency of the recording (Hz) |
| References | Published references associated with the event location, moment tensor, fault plane solution etc. |

The columns of ground motion data then follow. For example ‘f100.0000SA_RotD50’ is the spectral acceleration for a SDOF
oscillator with resonant frequency of 100 Hz, and the definition of horizontal component is RotD50. Ground motion values of
-99999 represent oscillator frequencies outside the minimum usable frequency of a given recording. PSA values are given in units
of g, peak ground velocities are given in m/s and Fourier amplitudes are in g · s. For the significant duration flatfile, the data
are provided for D<sub>5−75%</sub>, D<sub>5−95%</sub> and D<sub>20−80%</sub>, for the two as-recorded horizontal components (H1 and H2), as well as for the
geometric mean (GM). All duration data are provided in units of seconds.
