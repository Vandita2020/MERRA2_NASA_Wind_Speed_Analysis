# MERRA2_NASA_Wind_Speed_Analysis

In this study, we aim to explore the vulnerability of power grids in the south-east region of the USA with the help of data analysis tools and machine learning algorithms.

Our work would consist of working with two relevant datasets and then combining them together on the basis of the geolocations for different power grids for a fruitful outcome. 

## Data Downloading: 

### Electric substation data: 

The data is being downloaded from HIFLD (Link: https://hifld-geoplatform.opendata.arcgis.com/datasets/electric-substations/explore)  for 3 particular states Florida, New York, North Carolina. The data is downloaded in csv format and saved in Substation/csv folder.

The data contained several types including Substation, Tap, River, etc. out of which we filtered data for type Substation only. From this filtered data another separate csv file is created that includes only the latitude and longitude of electric substations. This csvs are saved in Substation/geo_locations and were converted using Filtering_Substation_data.py

Metadata: https://www.arcgis.com/sharing/rest/content/items/755e8c8ae15a4c9abfceca7b2e95fb9a/info/metadata/metadata.xml?format=default&output=html
Data Source Info: https://services1.arcgis.com/Hp6G80Pky0om7QvQ/arcgis/rest/services/Electric_Substations_1/FeatureServer/0


### Wind Speed Data:

The data is downloaded from NASA MERRA-2 site (Link: https://disc.gsfc.nasa.gov/datasets/M2TMNXSLV_5.12.4/summary?keywords=Merra%202%20wind%20data ) using API to get data for particular geo-locations. 

Two separate python files were created to get the data for U2M (2M Eastward Wind) and V2M(2M Northward Wind). The files are inside folder merradownload by name U2M_Wind_data_using_geo_location.py and V2M_Wind_data_using_geo_location.py to download U2M and V2M respectively. The files are first being downloaded in .nc4 format and then were converted to csv. The final csv files are saved in the Final_csv folder. 

MetaData: https://goldsmr4.gesdisc.eosdis.nasa.gov/data/MERRA2/M2T1NXSLV.5.12.4/doc/MERRA2.README.pdf

## EDA:
For the EDA and analysis details refer to the report. 
