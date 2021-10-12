# Catalogues of Historic Volcanic Activity
Catalogues of historic volcanic activity are reproduced from published scientific studies. The role of this repository is to make the activity catalogues available in an easily accessible format. Users are directed to the original studies that created the catalogues for details of scope, methodology, limitations, etc.

## Origin and Ownership of Catalogues
Catalogues have typically been compiled using a range of resources including, but not restricted to, published scientific papers, historic newspaper and photograph collections, government documents and reports, and oral histories and traditions.

Catalogues compiled by staff at GNS Science are owned by it's Volcano Monitoring Group (VMG). The VMG is responsible for providing updates to the catalogues, either when new activity is deemed to warrant inclusion, or when a change to an existing record is required. If required, updates will be made approximately annually. There are currently no catalogues compiled by researchers outside GNS Science, but if that occurs, similar procedures will be put in place.

## Data Quality and Related Considerations
The quality of the observations and descriptions in a catalogue vary from record to record. In particular, as activity has often been reported in newspapers, sometimes days or even weeks later, the exact date of activity may be uncertain. In these cases, the catalogue compiler has made a decision about when activity most likely occurred. How this has been dealt with may vary from case to case, and from catalogue to catalogue.

To be useful for time-series analysis and visualization, every activity observation needs to have a date (year, month, and day) of occurrence, and this needs to have a consistent format. If a date is uncertain, e.g. just the year or the year and month are known, then some assumptions have been made to assign a year, month, and day to the actvity. In all cases, the original assessment by the catalogue compiler of when activity most likely occurred and the uncertainty is preserved, so users have the option to deal with these records as they see fit.

No changes to the content of textural or numeric fields have been made to catalogues, even if errors were noted.

### Single Observation per Record
For further analysis it is highly desirable that activity catalogues have a single observation per data record. Situations where this does not hold in the original published catalogues are typically when more than one location is attributed to a single observation of activity, and when the same activity is noted to have occurred over several consecutive days. In some cases, it has been necessary to edit records so there is a single observation per record.

#### Multiple Locations Example
|Date LocalTime|Location|other columns not shown|
|---|---|---|
|1923-03-17|Red Crater and Te Maari|other information|

Has been edited to
|Date LocalTime|Location|other columns not shown|
|---|---|---|
|1923-03-17|Red Crater|other information|
|1923-03-17|Te Maari|other information|

#### Multiple Dates Example
|Date Comment|Activity Description|other columns not shown|
|---|---|---|
|1882 June 12-13|Steam columns|other information|

Has been edited to
|Date LocalTime|Date Comment|Activity Description|other columns not shown|
|---|---|---|---|
|1882-06-12|1882 June 12-13|Steam columns|other information|
|1882-06-13|1882 June 12-13|Steam columns|other information|

## Errors and Ommissions, and Updates
Comments about errors and omissions in the content in the catalogues should be taken up with the Volcano Monitoring Group at GNS Science (<info@gns.cri.nz>), or directly with the compiler for catalogues that originate outside GNS Science. Those groups will assess all requests for content changes.

### Routine Catalogue Updates
When new volcanic activity occurs, new data records will be added to catalogues. This will not be done immediately, but typically once a year. Material on the most recent activity at all volcanoes in New Zealand can be found in [Volcanic Alert Bulletins](https://www.geonet.org.nz/volcano/vab/).

## #1 Historic Volcanic Activity at Ruapehu
This catalogue is from a [report](https://shop.gns.cri.nz/sr_2013-045-pdf/) by Brad Scott at GNS Science. It contains details of eruptive activity at Ruapehu from 1830 to 2012. The full reference to the catalogue is `Scott, B.J. 2013 A revised catalogue of Ruapehu volcano eruptive activity : 1830-2012. Lower Hutt, N.Z.: GNS Science. GNS Science report 2013/45 107 p.`.

### Description of Data Fields
|Field|Description|
|---|---|
|Date LocalTime|The date of the eruption or other volcanic activity. The dates are in local time (NZST or NZDT). No times are recorded in the catalogue.|
|Date Comment|If the Date of activity is uncertain, then this field contains the compiler's original 'best understanding' of when the activity occurred, with any information about uncertainty.|
|Activity Description|A short description of the type of activity that occurred.|
|Activity Scale|An ordinal scale (1-5) describing the size of an eruption. Refer to the [report](https://shop.gns.cri.nz/sr_2013-045-pdf/) for further details.|
|Additional Details|Additional details of the activity in the Description field.|
|References|Sources of information used by the catalogue compilers that describe the activity. These are typically references to historic resources, such as newspapers, books, and government or other reports. Refer to the [report](https://shop.gns.cri.nz/sr_2013-045-pdf/) for further details.|

#### Activity Scale
Refer to the [report](https://shop.gns.cri.nz/sr_2013-045-pdf/) for further details.
|Activity Scale|Observed Effects|
|---|---|
|0|Crater Lake steaming, hotter than normal (i.e., above 30-35<sup>o</sup>C) creating additional interest, but no observations (or confirmation) of activity in lake.|
|1|Small phreatic eruptions confined to Crater Lake.|
|2|Phreatic or phreatomagmatic eruption accompanied by surges; material deposited outside Crater Lake, but still confined to the crater basin. May produce larger flows/floods in Whangaehu Valley.|
|3|Deposition of material outside the crater basin; possible remobilisation/lahars in upper catchments and Whangaehu valley; OR small scale explosive eruptions/intermittent ash emission when no lake is present.|
|4|Material deposited well outside the crater basin onto the summit plateau and outer flanks. Lahars possible in several catchments; OR explosive ash eruptions when no lake is present producing columns up to 10000 ft.|
|5|Large scale explosive eruption displacing moderate volumes of the lake, lahars in all/most major valleys. The summit and slopes covered, with ashfall off the cone; OR explosive eruptions when no lake is present producing tall (> 10000 ft) eruption columns and ashfall off the cone.|

## #2 Historic Volcanic Activity at Tongariro

This catalogue is from a [report](https://shop.gns.cri.nz/sr_2014-020-pdf/) and a [paper](https://www.sciencedirect.com/science/article/pii/S0377027314001127?via%3Dihub) by Brad Scott and Sally Potter at GNS Science. It contains details of eruptive activity at Tongariro from the 1846 to 2013. The full reference to the catalogue is `Scott, B.J.; Potter, S.H. 2014 Catalogue of historical eruptive activity and volcanic unrest at Mt. Tongariro : 1846-2013. Lower Hutt, N.Z.: GNS Science. GNS Science report 2014/20 70 p.`, and to the accompanying paper is `Scott, B.J.; Potter, S.H. 2014 Aspects of historical eruptive activity and volcanic unrest at Mt. Tongariro, New Zealand: 1846–2013. Journal of Volcanology and Geothermal Research 286 (2014) 263-276, http://dx.doi.org/10.1016/j.jvolgeores.2014.04.003`.

### Description of Data Fields
|Field|Description|
|---|---|
|Date LocalTime|The date of the eruption or other volcanic activity. The dates are in local time (NZST or NZDT). No times are recorded in the catalogue.|
|Date Comment|If the Date of activity is uncertain, then this field contains the compiler's original 'best understanding' of when the activity occurred, with any information about uncertainty.|
|Location|Activity from Tongariro volcano can originate from one of several craters or areas on the volcano. The location indicates where the catalogue compilers considered the activity most likely originated. See below for further details.|
|Activity Description|A short description of the type of activity that occurred.|
|Certainty|The measure of certainty assigned to the activity observations by the catalogue compilers. See below for further details.|
|References|Sources of information used by the catalogue compilers that describe the activity. These are typically references to historic resources, such as newspapers, books, and government or other reports. Refer to the [report](https://shop.gns.cri.nz/sr_2014-020-pdf/)  or [paper](https://www.sciencedirect.com/science/article/pii/S0377027314001127?via%3Dihub) for further details.|

### Location Information
Activity from Tongariro volcano can originate from one of several craters or areas on the volcano. The location indicates where the catalogue compilers considered the activity most likely originated. The locations that appear in the catalogue are: 'Ketetahi', 'Lower Te Maari', 'Ngauruhoe', 'Red Crater', 'Red Crater or Te Maari', 'South Crater', 'Te Maari', 'Tongariro', 'Upper Te Maari', '(Upper?) Te Maari', and 'unknown'. Refer to the original [report](https://shop.gns.cri.nz/sr_2014-020-pdf/) for a discussion on the local names and the history of their usage, and for historic and modern maps showing the locations.

### Certainty Descriptors
The catalogue compilers assigned a certainty measure to the reported activity. This is intended to represent how confident they were that the reported activity actually occurred. The certainty descriptors that appear in the catalogue are: 'Confirmed', 'Discounted', 'Eruptions unlikely', 'Possible', 'Probable', and a blank entry. Refer to the original [report](https://shop.gns.cri.nz/sr_2014-020-pdf/) for a discussion on the difficulties of working with historical information.
|Certainty Descriptor|Meaning|
|---|---|
|Blank entry|Unable to assess the observation. Presented so future workers can make their own choice. Information is often as limited as “steam seen at Tongariro or Red Crater”. In this case, it may not be an eruption, but could be related to volcanic unrest.|
|Confirmed|Reliable accounts/source, first person observations, science papers and cross referencing/triangulation in social science.|
|Discounted|Some form of account/observation that allows it to be discredited. Similar threshold to confirmed. The misuse of the names Tongariro and Ngauruhoe was often the reason, that is, activity could often be ascribed to Ngauruhoe.|
|Eruptions unlikely|Usually associated with unrest phenomena, no evidence for an eruption.|
|Possible|Less likely than probable, usually one account, but it lacks substance (unknown source) and cannot be cross referenced.|
|Probable|More likely than possible, usually only one account, but that has some strength (reliable observer/source), but lacks cross refencing.|
