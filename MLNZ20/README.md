# MLNZ20 
This file is an _evaluation dataset_ of the New Zealand Local network magnitude MLNZ20 dataset (Rhoades etal.,2020). It is derived from GeoNet Rapid event data processed offline and computed independently from the GeoNet Earthquake Catalogue.

It is a SeisComp magnitude evaluatation implementation  derived from _Rhoades et al._ (2021). 
This computation is originally based on a GNS Seiscomp Nightly V7.0 Pre-release implementation and will be upgraded over time (https://data.gempa.de/packages/Public/seiscomp/nightly/). Results are to be considered informational for science and development purposes and subject to modifications.

This dataset will be superseded once MLNZ20 will be fully implemented into GeoNet Rapid Earthquake Catalogue Production system.

## Evaluation Dataset description
MLNZ20 network magnitudes are processed routinely offline every month from GeoNet Rapid event automatic and manual solutions. More frequent updates are provided as required (e.g. in response to a large event). Data are extracted from computed seiscompxml event files and parsed into csv files.  

Only Events with both MLNZ20 and MLv magnitudes computed from observations are displayed.

The MLNZ20 dataset is computed from January 2024 onward. The dataset will be updated regularly and will be split in yearly files.

Fields | Description |
-------| ----------- |
ID | CUSP/SeisComP event ID |
OT | Event origin time format(UTC):yyyy-mm-ddThh:mm:ss.sZ |
Lat | Epicentre latitude |
Lon | Epicentre longitude |
Dep | Hypocentre depth |
NrStaMLv | Number of MLv station amplitudes/magnitudes observations used |
NrStaMLNZ20 | Number of MLNZ20 station amplitudes/magnitudes observations used |
MLv | Default local network magnitude MLv (vertical) - GeoNetRapid  |
MLNZ20 | Offline processed NZ network magnitude MLNZ20 - Seiscomp Nightly (dev) 
Ratio | Indicative MLnz/MLv Ratio |

## Note
Station corrections terms are issued from the reference paper. MLNZ20 network magnitude is derived from these stations only.
Delta repository reference: https://github.com/GeoNet/delta/blob/main/environment/corrections.csv

### Reference Papers
David A. Rhoades, Annemarie Christophersen, Sandra Bourguignon, John Ristau, Jérôme Salichon; "A Depth‐Dependent Local Magnitude Scale for New Zealand Earthquakes Consistent with Moment Magnitude."; Bulletin of the Seismological Society of America 2020;; 111 (2): 1056–1066. doi: https://doi.org/10.1785/0120200252
