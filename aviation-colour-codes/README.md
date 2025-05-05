# Volcanic Aviation Colour Codes

An [Aviation Colour Code (ACC)](https://www.geonet.org.nz/about/volcano/acc) system is used to provide the aviation community with information about volcanic activity and the potential presence of volcanic ash in the atmosphere. It is defined by the International Civil Aviation Organisation ([ICAO](https://www.icao.int/)). The ACC for New Zealand volcanoes is set by the Volcano Monitoring Group at GNS Science. It is publicised using a [VONA](https://www.aviation.govt.nz/airspace-and-aerodromes/meteorology/met-developments/volcanic-hazards/), which is sent to relevant members of the aviation community, on the [GeoNet Website](https://www.geonet.org.nz/volcano/acc), and in the heading of many [Volcanic Activity Bulletins (VAB)](https://www.geonet.org.nz/volcano/vab).

GNS Science started to set Aviation Colour Codes in August 2009. While [Volcanic Alert Level (VAL)](https://www.geonet.org.nz/about/volcano/val) and ACC can both change in response to increases or decreases in volcanic activity, changes in ACC are not directly related to changes in VAL, or vice versa.

The GeoNet website contains a [brief explanation of Aviation Colour Codes](https://www.geonet.org.nz/about/volcano/acc).

## Description of Files and Data Fields

The files in this repository contain a complete record of Aviation Colour Codes at New Zealand volcanoes.

Each file is in comma-separated values ([CSV](https://en.wikipedia.org/wiki/Comma-separated_values)) format. Files are named _ACC_volcano-name.csv_. Te Reo volcano names do not contain macrons.

| Field | Description |
| --- | --- |
| PeriodStart UTC | The UTC date and time for the start of the period of the ACC shown, in [ISO8601 format](https://en.wikipedia.org/wiki/ISO_8601) |
| PeriodEnd UTC | The UTC date and time for the end of the period of the ACC shown, in [ISO8601 format](https://en.wikipedia.org/wiki/ISO_8601) |
| ACC | The ACC colour for that period |

- The dates and times of changes in ACC are provided only in UTC. This is because they are only provided to and used by the aviation community in UTC.
- The ACC is a colour, and can be, in order of increasing severity, "Green", "Yellow", "Orange", or "Red".

### PeriodStart and PeriodEnd ###
The PeriodStart and PeriodEnd have been sourced from the issue time of the VONA that was used to publicise a change in ACC. In some cases the original VONA was not available, but a VAB, which also shows the ACC was available, so the VAB issue time was used. The error introduced by this is likely to be less than one hour.

There are errors on the issue time of some VONA, caused by incorrect conversion from local time to UTC. Where this has been recognised, knowledge of the volcanic activity and the issue time of a related VAB have been used to determine the correct ACC change time. This problem is know for one or two VONAs related to the 2012 eruptive activity of Tongariro.

## Current ACC
The current ACC for all New Zealand volcanoes can be view on the [GeoNet website](https://www.geonet.org.nz/volcano/acc). An accompanying map shows the location of each volcano.
