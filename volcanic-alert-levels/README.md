# Volcanic Alert Levels

New Zealand uses a Volcanic Alert Level (VAL) system to define the current status of each volcano. This is used to guide any appropriate response. The VAL is decided by a Volcano Monitoring Group at GNS Science; it is publicised using a [Volcanic Alert Bulletin](https://www.geonet.org.nz/volcano/vab/) (VAB), and on the [GeoNet Website](https://www.geonet.org.nz/).

## VAL Versions
New Zealand has had three versions of its VAL system. The current [VAL](https://www.geonet.org.nz/about/volcano/val) system, version 3, was first used in July 2014. A [publication](https://link.springer.com/article/10.1186/s13617-014-0013-7) dicusses the use of volcanic alert levels and development of version 3.

| VAL Version | Dates Used |
| --- | --- |
| 1 | 1994-12-01 to 1995-09-11 |
| 2 | 1995-09-12 to 2014-06-30 |
| 3 | since 2014-07-01 |

### Version 1
| VAL | Scientific Interpretation |
| --- | --- |
| 1 |  Initial sign of volcano reawakening; no eruption imminent; possible minor activity |
| 2 |  Indicators of intrusion process or significant change in on-going eruptive activity |
| 3 |  If increasing trends continue there is a real possibility of hazardous eruptive activity |
| 4 |  Hazardous volcanic eruption is now imminent |
| 5 |  Destruction within the Permanent Danger Zone (red zone) and significant risk over wider area |

### Version 2
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

The files in this repository contain all recorded VAL changes at New Zealand volcanoes.

Files exist for each volcano at which the VAL has been changed. If a file does not exist, then the VAL has never been changed, and has always been zero.

| Field | Description |
| --- | --- |
| Date UTC | The UTC date and time of a VAL change, ISO8601 format |
| Date NZtime | The NZST or NZDT date and time of a VAL change |
| VAL | The numeric VAL value assigned on that date |
| Description | The description of the VAL value |
| VAL Version | The version number of the VAL system used on the date of the change |

- The date and time of a VAL change is provided in UTC to support easy integration with other GeoNet data sets which also use UTC. 
- Stakeholder groups that may be more interested in response actions to VAL changes are more likely to work in local time; a VAL change is also provided in NZST or NZDT to support those users.
- For some older VAL changes, the date of a change is know, but not the time. In those cases, the time has arbitrarily been set to 12:00:00, midday NZ local time.
- The VAL value is numeric, ranging from 1 to 5 in version 1, and 0 to 5 in versions 2 and 3.
- The description gives the officially agreed meaning of the VAL value.
- The VAL version shows the version in operation when the VAL change was made.

### Initial Value
The first data row in the file establishes the initial VAL for that volcano, in the VAL version when a VAL for that volcano was first assigned. In the current VAL version, version 3, all volcanoes have a 'base' VAL of zero, but in practice, Ruapehu and Whakaari/White Island have never had a VAL lower than 1.

An initial VAL value facilitates easier visualization of VAL changes.

## Current VAL
The current VAL values for all New Zealand volcanoes can be view on the [GeoNet website](https://www.geonet.org.nz/volcano). An accompnaying map shows the location of each volcano.
