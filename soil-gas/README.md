# Soil Gas
Soil gas data are collected manually by the Volcano Monitoring Group (VMG) at GNS Science to [monitor gas discharge rate through the ground in volcanic and geothermal areas](https://www.geonet.org.nz/volcano/how).

They are measured with a soil gas flux meter, a bucket-shaped metal accumulation chamber placed on the ground with the gases pumped through a back-pack analyser to derive a flux (emission rate). We can measure carbon dioxide (CO<sub>2</sub>), hydrogen sulphide (H<sub>2</sub>S), and methane (CH<sub>4</sub>) gases in this way.

Soil gas flux measurements were made regularly for monitoring changes at Whakaari White Island until the 2019 eruption. It that case, pegs were used to mark measurement points, so measurements could be made at exactly the same positions each time. Those data constitute a time-series, and are therefore available through [Tilde](https://tilde.geonet.org.nz/).

Soil gas flux measurements have also been made at Raoul Island, Ngauruhoe, Tongariro, and Moutohorā Whale Island volcanoes. In these cases, pegs were not used to mark measurement points, so measurements could not be made at exactly the same positions each time. Instead, measurements are made in broadly the same areas, but subject to constraints such as access and time availability, which will vary from survey to survey. For this reason, making the data available through Tilde is not an option. Those data are available through this repository.

## Data
The location of each gas flux measurement is measured by a phone with a built-in GPS and recorded alongside the flux measured. The ground temperature at a depth of 10 cm is measured immediately after the soil gas measurement by inserting a thermocouple in the ground at the middle where the chamber was located.

Measurement locations are provided in the [New Zealand Transverse Mercator 2000 (NZTM2000) grid](https://www.linz.govt.nz/guidance/geodetic-system/coordinate-systems-used-new-zealand/projections/new-zealand-transverse-mercator-2000-nztm2000), rather than latitude and longitude in the [World Geodetic System 1984 (WGS84)](https://www.linz.govt.nz/guidance/geodetic-system/coordinate-systems-used-new-zealand/geodetic-datums/world-geodetic-system-1984-wgs84) coordinate system that is commonly used for GeoNet spatial data.

## Description of Files and Data Fields
Each file in this repository contains the data collected from one survey of one volcanic area. Files are in CSV (comma-separated values) format.

### Filenames
A filename consists of three parts:
- The volcano name, e.g "MoutohoraWhaleIsland". If both Te Reo and English names are commonly used for the volcano, the Te Reo name is followed by the English name. There are no spaces in the volcano name, and no macrons are used for Te Reo names.
- The date the data were collected, e.g. "2025-01-29". This uses local time (NZST or NZDT). The date is separated from the volcano name by an underscore “\_”.
- A “csv” suffix. This indicates a CSV file format. The suffix is separated from the date by a dot “.”.
If measurements were carried out over more than one day, but are considered by the VMG  to represent a single dataset, they are provided as a single file without highlighting which observations were made on which day. However, the date part of the filename shows both measurement dates.

### Data Fields
| Field | Description |
| --- | --- |
| MeasurementNumber | A number assigned to a measurement location. Measurement numbers from one survey (data file) have no relation to measurement numbers from another survey (data file). |
| NZTM-mE | New Zealand Transverse Mercator projection East coordinate, in units of metres. |
| NZTM-mN | New Zealand Transverse Mercator projection North coordinate, in units of metres. |
| CO2 | Carbon dioxide (CO<sub>2</sub>) flux, in units of g/m<sup>2</sup>/day (grams per square metre per day). |
| CH4 | Methane (CH<sub>4</sub>) flux, in units of g/m<sup>2</sup>/day (grams per square metre per day). Not present if methane data were not collected. |
| H2S | Hydrogen sulphide (H<sub>2</sub>S) flux, in units of g/m<sup>2</sup>/day (grams per square metre per day). Not present if hydrogen sulphide data were not collected. |
| GroundTemperature | Temperature of the ground at a depth of approximately 10 cm, in units of <sup>o</sup>C (degrees Celsius). |

If no measurement was made, the corresponding field is empty. A zero flux indicates a measurement was made, but no gas was observed.

## References

The following references provide some background information on soil gas measurements and how the data are commonly used:

 - Cardellini, C., G. Chiodini, and F. Frondini, 2003. Application of stochastic simulation to CO2 flux from soil: Mapping and quantification of gas release, J. Geophys. Res., 108(B9), 2425, [doi:10.1029/2002JB002165](doi:10.1029/2002JB002165).
- Werner, C. and Cardellini, C., 2006. Comparison of carbon dioxide emissions with fluid upflow, chemistry, and geologic structures at the Rotorua geothermal system, New Zealand. Geothermics, 35, [doi.org/10.1016/j.geothermics.2006.02.006](doi.org/10.1016/j.geothermics.2006.02.006).
 - Yang, T.H.J., Chambefort, I., Rowe, M., Mazot, A., Seward, A., Werner, C., Fischer, T., Seastres, J., Siega, F., Macdonald, N. and Brakenrig, T., 2024. Variability in surface CO2 flux: Implication for monitoring surface emission from geothermal fields. Geothermics, 120, [doi.org/10.1016/j.geothermics.2024.102981](doi.org/10.1016/j.geothermics.2024.102981).
