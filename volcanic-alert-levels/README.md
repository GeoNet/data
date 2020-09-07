# Volcanic Alert Levels

New Zealand uses a Volcanic Alert Level (VAL) system to define the current status of each volcano. This is used to guide any appropriate response. The VAL is decided by a Volcano Monitoring Group at GNS Science; it is publicised using a [Volcanic Alert Bulletin](https://www.geonet.org.nz/volcano/vab/) (VAB), and on the [GeoNet Website](https://www.geonet.org.nz/).

## VAL Versions
New Zealand has had three versions of its VAL system. The current [VAL](https://www.geonet.org.nz/about/volcano/val) system, version 3, was first used in July 2014.

| VAL Version | Dates Used |
| --- | --- |
| 1 | 1994-12-01 to 1995-09-11 |
| 2 | 1995-09-12 to 2014-06-30 |
| 3 | since 2014-07-01 |

### Version 1
| VAL | Volcanic Activity |
| --- | --- |
| 0 | activity 0 |
| 1 |  activity 1|
| 2 |  activity 2|
| 3 |  activity 3|
| 4 |  activity 4|
| 5 |  activity 5|

### Version 2
| VAL | Volcanic Activity |
| --- | --- |
| 0 | activity 0 |
| 1 |  activity 1|
| 2 |  activity 2|
| 3 |  activity 3|
| 4 |  activity 4|
| 5 |  activity 5|

### Version 3
More detailed documentation of version 3, is available on the [GeoNet website](https://www.geonet.org.nz/about/volcano/val).
| VAL | Volcanic Activity |
| --- | --- |
| 0 | No volcanic unrest |
| 1 |  Minor volcanic unrest |
| 2 |  Moderate to heightened volcanic unrest |
| 3 |  Minor volcanic eruption |
| 4 |  Moderate volcanic eruption |
| 5 |  Major volcanic eruption |

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
- The VAL value is numeric, ranging for 0 to 5 in the current version. All versions used 0-5???
- The description gives the officially agreed meaning of the VAL value.
- The VAL version shows the version in operation when the VAL change was made.

### Initial Value
The first data row in the file establishes the initial VAL for that volcano. While all volcanoes have a 'base' VAL of zero, in practice, Ruapehu and Whakaari/White Island have never had a VAL lower than 1.
An initial VAL facilitates easier visualization of VAL changes.

