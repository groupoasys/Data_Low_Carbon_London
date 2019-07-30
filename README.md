# Data_LOW_CARBON_LONDON

This repository collects the data of the UK Power Networks led -- Low Carbon London project [1], which takes places 
from november 2011 to february 2014, the year 2013 is the trial period for dynamic prices. 

The analysis and interpretation of this data are done to understand the response of consumers to dynamic prices in the supply of electricity, which can help us measure the level of households flexibility and the prediction of user demand according to their characteristics.

Each data file is explained below:


1) Power_Networks_LCL[2]: data every half hour that include measures of energy consumption in households taken 
by the Smart-meter system and other data associated with each measure. 

The original database is outsize, so it has been divided into 168 .csv files in a compressed .zip folder

Database parameters:

	* LCLid: Unique household identifier.
	* stdorToU: The type of tariff system. Two options: Standard (fixed price) or DTOU (dynamic prices).
	* DateTime: Date and time for half hour intervals.
	* kWh/hh: Consumption reading (½ hour intervals) by the Smart-meter system.
	* ACORN: Classification of households according to geo-demographic group (A-Q). 
	* Acorn_grouped: ACORN groups are grouped into 3 categories: Affluent(A-E), Comfortable(F-J) or Adversity(K-Q).

2) Data_features.xlsx: this file includes input variables used in our analysis and other data generated for aggregate groups of households (year 2013).

--> Price[2]: Data every half hour on tariffs (£) applied to households with dynamic prices during the year of the trial. The dToU system has variations in the price of electricity, it uses three price bands: High, normal, low. The consumer knows the day before the price that will be applied every hour.

	* High price: 67,20 pence/kWh.
	* Normal price: 11,76 pence/kWh.
	* Low price: 3,99 pence/kWh.

The non-TOU group tariff was fixed at 14.28 pence / kWh.

--> Temperature[3]: Temperature (ªC) data recorded half hourly at the London City Airport station during 2013.

--> Demand: The aggregate demand (kWh/hh) of consumer groups in the experimental group (dtou) during the year 2013. Groups:
* 'flex': Average & total aggregate consumption of the most flexible cluster.
* 'noflex': Average & total aggregate consumption of other clusters.
* 'all': Average & total aggregate consumption of all clusters.

On the other hand, to facilitate the handling and preparation of the data used in our work, we have generated other databases from the originals. For instance, segmentation and cleansing of data for each ACORN group or data including prices half hourly. If you are interested, let me know and I will be pleased to provide you.


Resource-Links:
[1]https://innovation.ukpowernetworks.co.uk/ 
[2]https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households
[3]https://rp5.ru/Weather_archive_in_London_City_(airport),_METAR
