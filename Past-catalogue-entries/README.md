# Past-catalogue-entries
This dataset is a record of some past entries of the CUSP earthquake catalogue datbase as imported and recorded in a former open AWS event bucket "s3://seiscompml06-bucket-sskhju471z6g/". The bucket is inactive since 2013. 

## Event Dataset description
This dataset is an events listing classified as "other" without any magnitudes associated. The numerous eveanst are located worldwide and poorly informed  and compatible to our current information systems. Hence they are excluded from our present catalogues but listing and archived event seiscomp xml format can be found here instead.

Only Events without magnitude information of type "other are listed here.

The Past "other" events dataset is covering years from 1942 to 2011. It has about 28000  entries which locationis are spread wordlwide.  

Fields | Description |
-------| ----------- |
EventID | CUSP ID
Time | Event origin time format(UTC):yyyy-mm-ddThh:mm:ss.ss
Latitude | Epicentre latitude  
Longitude | Epicentre longitude 
Depth/km | Hypocentre depth 
Author | Author ID 
Catalog |  na
Contributor | na
ContributorID | CUSP ID
MagType | na
Magnitude | na
MagAuthor | na 
EventLocationName | Region informed
EventType | type "other" (mix bag)

## Note
This is a work to make former records archived and accessible to the community as a limited information though in a  machine readable format.

### Reference Papers
No reference clearly identified - CUSP Pre 2012 Database. GNS/GeoNet
Seiscomp format information reference:  https://docs.gempa.de/seiscomp/current/ 
