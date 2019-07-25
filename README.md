# newData_LOW_CARBON_LONDON

This repository collects the data of the UK Power Networks led -- Low Carbon London project [1], which takes places 
from november 2011 to february 2014, the year 2013 is the trial period for dynamic prices. Each data file is explained below:


1) Power-Networks-LCL-June2015.csv_Pieces[2]: data every half hour that include measures of energy consumption in households taken 
by the Smart-meter system and other data associated with each measure, explained below. 

The original database is outsize, so it has been divided into 168 .xlsx files in a compressed .zip folder

Database parameters:

	* LCLid: Unique household identifier.
	* stdorToU: The type of tariff system. Two options: Standard (fixed price) or DTOU (dynamic prices).
	* DateTime: Date and time for half hour intervals.
	* kWh/hh: Consumption reading (½ hour intervals) by the Smart-meter system.
	* ACORN: Classification of households according to geo-demographic group (A-Q). 
	* Acorn_grouped: ACORN groups are grouped into 3 categories: Affluent(A-E), Comfortable(F-J) or Adversity(K-Q).

2) Tariffs.xlsx[2]: data every half hour on tariffs applied to households with dynamic prices during the year of the trial. The dToU system has variations in the price of electricity, it uses three price bands: High, normal, low. The consumer knows the day before the price that will be applied every hour.

	* High price: 67,20 pence/kWh.
	* Normal price: 11,76 pence/kWh.
	* Low price: 3,99 pence/kWh.

The non-TOU group tariff was fixed at 14.28 pence / kWh.


On the other hand, to facilitate the handling and preparation of the data used in our work, we have generated other databases from the originals. 
For example, segmentation and cleansing of data for each ACORN group.

3) Acorn_Data: same data as file 1), but divided for each acorn group and deleted null or empty data.


Additionally, we have used in our analysis a database of temperatures [3]:

4) Temperature.xlsx: Temperature data recorded every half hour at the London City Airport station during 2013.


Resource-Links:
[1]https://innovation.ukpowernetworks.co.uk/ 
[2]https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households
[3]https://rp5.ru/Weather_archive_in_London_City_(airport),_METAR

