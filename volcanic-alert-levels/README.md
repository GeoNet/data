# Volcanic Alert Levels

New Zealand uses a Volcanic Alert Level (VAL) system to define the current status of each volcano. This is used to guide any appropriate response. The VAL is decided by a Volcano Monitoring Group at GNS Science; it is publicised using a [Volcanic Alert Bulletin](https://www.geonet.org.nz/volcano/vab/) (VAB), and on the [GeoNet Website](https://www.geonet.org.nz/).

## VAL Versions
New Zealand has had three versions of its VAL system. The current [VAL](https://www.geonet.org.nz/about/volcano/val) system, version 3, was first used in July 2014. A [publication](https://link.springer.com/article/10.1186/s13617-014-0013-7) discusses the use of volcanic alert levels and the development of version 3.

| VAL Version | Dates Used |
| --- | --- |
| 1 | 1994-12-01 to 1995-08-01* |
| 2 | 1995-08-01* to 2014-07-01 |
| 3 | since 2014-07-01 |

*The exact date of the start of version 2 is not recorded, but a Volcanic Alert Bulletin from September 1995 refers to the system being revised in August 1995.
### Version 1
Version 1 had no zero level. This meant that unless a volcano was at VAL 1 or higher, the VAL was not defined. Version 1 was only ever used for Ruapehu. 
| VAL | Scientific Interpretation |
| --- | --- |
| 1 |  Initial sign of volcano reawakening; no eruption imminent; possible minor activity |
| 2 |  Indicators of intrusion process or significant change in on-going eruptive activity |
| 3 |  If increasing trends continue there is a real possibility of hazardous eruptive activity |
| 4 |  Hazardous volcanic eruption is now imminent |
| 5 |  Destruction within the Permanent Danger Zone (red zone) and significant risk over wider area |

### Version 2
The exact date of the start of version 2 is not recorded, but a Ruapehu Volcanic Alert Bulletin from September 1995 refers to the system being revised in August 1995. There is no record of the initial values assigned to each volcano when version 2 was introduced. However, Volcanic Alert Bulletins for the Kermadec Islands (Raoul Island), Ngauruhoe, Taupo, and Tongariro refer either to the VAL remaining at 0, or increasing from 0. We can therefore infer that all volcanoes not assigned a non-zero VAL when version 2 was introduced were intended to have a VAL of 0.
| VAL | Volcanic Status |
| --- | --- |
| 0 | Usual dormant, or quiescent state |
| 1 | Signs of volcano unrest |
| 2 | Minor eruptive activity |
| 3 | Significant local eruption in progress |
| 4 | Hazardous local eruption in progress |
| 5 | Large hazardous eruption in progress |

### Version 3
More detailed documentation of version 3, is available on the [GeoNet website](https://www.geonet.org.nz/about/volcano/val).
| VAL | Volcanic Activity |
| --- | --- |
| 0 | No volcanic unrest |
| 1 | Minor volcanic unrest |
| 2 | Moderate to heightened volcanic unrest |
| 3 | Minor volcanic eruption |
| 4 | Moderate volcanic eruption |
| 5 | Major volcanic eruption |

## Description of Files and Data Fields

The files in this repository contain a complete record of VAL values at New Zealand volcanoes.

| Field | Description |
| --- | --- |
| PeriodStart UTC | The UTC date and time for the start of the period of the VAL shown, ISO8601 format |
| PeriodEnd UTC | The UTC date and time for the end of the period of the VAL shown, ISO8601 format |
| VAL | The numeric VAL value for that period |
| VAL System Version | The version number of the VAL system used for that period |
| Description | The description of the VAL value |
| PeriodStart NZtime | The NZST or NZDT date and time for the start of the period of the VAL shownn |
| PeriodStart NZtime | The NZST or NZDT date and time for the end of the period of the VAL shown |

- The dates and times of changes in VAL is provided in UTC to support easy integration with other GeoNet data sets which also use UTC. 
- Stakeholder groups that may be more interested in response actions to VAL changes are more likely to work in local time; the dates and tmes of VAL changes are also provided in NZST or NZDT to support those users.
- For some older VAL changes, the date of a change is know, but not the time. In those cases, the time has arbitrarily been set to 12:00:00, midday NZ local time.
- The VAL value is numeric; in version 1 ranging from 1 to 5 , and in versions 2 and 3 ranging from 0 to 5.
- The description gives the officially agreed meaning of the VAL value.
- The VAL version shows the version of the VAL system in operation when the VAL was at a particular level.

## Current VAL
The current VAL values for all New Zealand volcanoes can be view on the [GeoNet website](https://www.geonet.org.nz/volcano). An accompnaying map shows the location of each volcano.
