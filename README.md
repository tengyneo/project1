<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">

## Impact of Adverse Weather Conditions on Singapore's Tourism Industry
This project is a part of General Assembly's Data Science Immersive (DSI) course requirements at [GA DSI](https://generalassemb.ly/education/data-science-immersive/singapore).  Other DSI projects can be found at the [main GitHub page](https://github.com/tengyneo).

## Project Intro/Objective
According to the latest [National Climate Change Study](https://www.channelnewsasia.com/singapore/sg-tourists-climate-change-heat-sea-level-rise-warmer-weather-ecotourism-green-4050806), Singapore will experience progressively hotter and wetter days. This may diminish the attractiveness of Singapore as a tourist destination. The purpose of this project is to assess the impact of adverse weather conditions on Singapore's tourism industry.

### Methods Used
* Data Processing/Cleaning
* Data Exploration
* Descriptive Statistics
* Data Visualization
  
### Technologies
* Python (packages used include pandas, numpy, seaborn, matplotlib, datetime and calendar)
* Jupyter Notebook

## Data Sources
### Weather Datasets:
- [<span style="background-color: light blue">RainfallMonthlyNumberofRainDays.csv</span>](https://beta.data.gov.sg/collections/1398/view): The number of rain days (day with rainfall amount of 0.2mm or more) in a month recorded at the Changi Climate Station
- [<span style="background-color: light blue">RainfallMonthlyTotal.csv</span>](https://beta.data.gov.sg/collections/1399/view): The total monthly rainfall recorded at the Changi Climate Station
- [<span style="background-color: light blue">RainfallMonthlyHighestDailyTotal.csv</span>](https://beta.data.gov.sg/collections/1397/view): The highest daily total rainfall for the month recorded at the Changi Climate Station
- [<span style="background-color: light blue">SunshineDurationMonthlyMeanDailyDuration.csv</span>](https://beta.data.gov.sg/collections/1417/view): The monthly mean sunshine hours in a day recorded at the Changi Climate Station
- [<span style="background-color: light blue">SurfaceAirTemperatureMonthlyMean.csv</span>](https://beta.data.gov.sg/collections/1419/view): The monthly mean air temperature recorded at the Changi Climate Station
- [<span style="background-color: light blue">WetBulbTemperatureHourly.csv</span>](https://beta.data.gov.sg/collections/1423/view): The hourly wet bulb temperature recorded at the Changi Climate Station
- [<span style="background-color: light blue">RelativeHumidityMonthlyMean.csv</span>](https://beta.data.gov.sg/collections/1404/view): The monthly mean relative humidity recorded at the Changi Climate Station.

### Tourism Datasets:
- [<span style="background-color: light blue">hotelstatistics-table.csv</span>](https://tablebuilder.singstat.gov.sg/table/TS/M550081): Monthly hotel statistics on revenue and occupancy rate
- [<span style="background-color: light blue">visitordays-table.csv</span>](https://tablebuilder.singstat.gov.sg/table/TS/M550281): Number Of Visitor Days, (At End Of Period)
- [<span style="background-color: light blue">outbounddeparturesingaporeresidents-table.csv</span>](https://tablebuilder.singstat.gov.sg/table/TS/M650661): Outbound Departures Of Singapore Residents By Mode Of Transport
- [<span style="background-color: light blue">internationalvisitorarrivals-table.csv</span>](https://tablebuilder.singstat.gov.sg/table/TS/M550001): Total International Visitor Arrivals By Inbound Tourism Markets

## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**month**|*date*|All|Year month| 
|**no_of_rainy_days**|*integer*|RainfallMonthlyNumberofRainDays|Number of rain days (day with rainfall amount of 0.2mm or more) in a month recorded at the Changi Climate Station|
|**rainy_month**|*integer*|Derived|Binary indicator to determine if a specific month is rainy, computed by taking no_of_rainy_days and dividing by the total number of days for that month. Value is 1 if result is >= 0.5, else 0.|
|**total_rainfall**|*float*|RainfallMonthlyTotal|Total monthly rainfall (in mm) recorded at the Changi Climate Station|
|**maximum_rainfall_in_a_day**|*float*|RainfallMonthlyHighestDailyTotal|The highest daily total rainfall (in mm) for the month recorded at the Changi Climate Station)|
|**mean_sunshine_hrs**|*float*|SunshineDurationMonthlyMeanDailyDuration|The monthly mean sunshine hours in a day recorded at the Changi Climate Station|
|**mean_temp**|*float*|SurfaceAirTemperatureMonthlyMean|The monthly mean air temperature (in °C) recorded at the Changi Climate Station|
|**wet_bulb_temperature**|*float*|WetBulbTemperatureHourly|The hourly wet bulb temperature (in °C) recorded at the Changi Climate Station|
|**mean_rh**|*float*|RelativeHumidityMonthlyMean|The monthly mean relative humidity (in %) recorded at the Changi Climate Station|
|**hotel_room_revenue**|*float*|hotelstatistics-table|Total hotel room revenue (in dollars)|
|**standard_average_room_rate**|*float*|hotelstatistics-table|Standard average room rates (in dollars) calculated from total room revenue divided by gross lettings.|
|**standard_average_hotel_occupancy_rate**|*float*|hotelstatistics-table|Standard average hotel occupancy rates (in %) calcualted from gross lettings (room nights) divided by available room-nights.|
|**gross_lettings_room_nights**|*float*|hotelstatistics-table|Gross lettings of room nights|
|**available_room_nights**|*float*|hotelstatistics-table|room-nights available for occupancy. Excludes rooms closed for renovations and staff use as declared by the hotels in the statutory forms.|
|**visitor_days_number**|*float*|visitordays-table|Total number of visitor days|
|**total_departure**|*float*|outbounddeparturesingaporeresidents-table|Total outbound departure of Singapore Residents.|
|**total_air_departure**|*float*|outbounddeparturesingaporeresidents-table|Total outbound departure of Singapore Residents by air.|
|**total_sea_departure**|*float*|outbounddeparturesingaporeresidents-table|Total outbound departure of Singapore Residents by sea.|
|**total_IVA_by_inbound_tourism_markets**|*float*|outbounddeparturesingaporeresidents-table|Total International Visitor Arrivals By Inbound Tourism Markets. Excludes arrivals of Malaysians by land.|
|**total_IVA_by_XXX**|*float*|outbounddeparturesingaporeresidents-table|Total International Visitor Arrivals from specific regions. Excludes arrivals of Malaysians by land.|
  
## Featured Notebooks/Slides/Data
* [Jupyter Notebook Report](https://github.com/tengyneo/project1/tree/main/notebook)
* [Raw Data](https://github.com/tengyneo/project1/tree/main/data)

## Contact

|Name     |  Slack Handle   | 
|---------|-----------------|
|[Neo Teng Yong](https://github.com/tengyneo)| @Teng Yong        |
|[Kathleen](https://github.com/kathleenchang8/GA-DSI)| @kathleen        |
