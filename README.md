# Big Data Tools and Analytics

## Project - US Flights Data Set Analysis - README

### Group:

   - André Viana - l54543 - andreviana@aln.iseg.ulisboa.pt
   - Gonçalo Duarte - l48505 - goncaloduarte@aln.iseg.ulisboa.pt
   - José Cabral - l54997 - l54997@aln.iseg.ulisboa.pt
<br>

Masters Data Analytics for Business - ISEG - University of Lisbon

May 2021

### Summary

Airplanes are the most used transport to move around the world. Through this project, we aim at analyzing the US flights, understanding its evolution over the years and develop a network of the routes.

### Data Description

To develop this project, we worked with <b> Bureau of Transportations Statistics data sets </b>, regarding flights from 2017 to 2020:

Data set containing a row per flight and columns:

<i>FL_DATE</i> = Flight Date (yyyy-mm-dd)  
<i>OP_UNIQUE_CARRIER</i> = Carrier ID 
<i>ORIGIN_AIRPORT_ID</i> = Origin Airport ID. An identification number assigned by US DOT to identify a unique airport.  
<i>ORIGIN</i> = Origin Airport  
<i>ORIGIN_CITY_NAME</i> = Origin Airport city name  
<i>ORIGIN_STATE_ABR</i> = Origin Airport state abreviation  
<i>ORIGIN_STATE_NM</i> = Origin Airport state name  
<i>DEST_AIRPORT_ID</i> = Destination Airport ID. An identification number assigned by US DOT to identify a unique airport.  
<i>DEST</i> = Destination Airport  
<i>DEST_CITY_NAME</i> = Destination Airport city name  
<i>DEST_STATE_ABR</i> = Destination Airport state abreviation  
<i>DEST_STATE_NM</i> = Destination Airport state name  
<i>CRS_DEP_TIME</i> = Programmed departure time (local time: hhmm)  
<i>DEP_TIME</i> = Actual departure time (local time: hhmm)  
<i>DEP_DELAY</i> = Departure delay in minutes, early departures show negative numbers.(DEP_TIME - CRS_DEP_TIME).  
<i>WHEELS_OFF</i> = Wheels Off Time (local time: hhmm)  
<i>WHEELS_ON</i> =  Wheels On Time (local time: hhmm)  
<i>CRS_ARR_TIME</i> = Programmed arrival time (local time: hhmm)  
<i>ARR_TIME</i> = Actual arrival time (local time: hhmm)  
<i>ARR_DELAY</i> = Arrival delay in minutes, early arrivals show negative numbers.(ARR_TIME - CRS_ARR_TIME).  
<i>CANCELLED</i> = Cancelled Flight Indicator (1=Yes)   
<i>CANCELLATION_CODE</i> = Specifies The Reason For Cancellation   
<i>CRS_ELAPSED_TIME</i> = Programmed Elapsed Time of Flight, in Minutes  
<i>ACTUAL_ELAPSED_TIME</i> = Actual Elapsed Time of Flight, in Minutes  
<i>AIR_TIME</i> = Flight Time, in Minutes  
<i>DISTANCE</i> = Distance between airports (miles)  
<i>CARRIER_DELAY</i> = Carrier Delay, in Minutes  
<i>WEATHER_DELAY</i> = Weather Delay, in Minutes  
<i>NAS _DELAY</i> = National Air System Delay, in Minutes  
<i>SECURITY_DELAY</i> = Security Delay, in Minutes  
<i>LATE_AIRCRAFT_DELAY</i> = Late Aircraft Delay, in Minutes  

## Project Description


On the folder, you will find <b>7 documents: </b> 
  

  - <b><i>README.md</i></b> : this document describing all data sets used and what was developed in the project;
  
  
  - <b><i>Complete Dataset to table.ipynb</i></b> : a jupyter notebook to load all csv files and save them on a table to use further on the analysis.


  - <b><i>Data aggregation.ipynb</i></b> : a jupyter notebook to agragate the data and convert it to pandas DataFrame.

   
  - <b><i>Coordinates Script.ipynb</i></b> : a jupyter notebook to get the coordinates of the airports location.


  - <b><i>Data analysis.ipynb</i></b> : a jupyter notebook to visualize and describe the data.
  
      Five different charts are presented:
      <br>
      - Total number of flights per airport:
              A scatter plot with the evolution of the total number of flights per month.
              <br>
      <br>
      - DataFrame with the highest and lowest numbers of flights per month:
              A DataFrame with the 3 aiports with hights number of flighs and 3 the with the lowest number.
              <br>
      <br>
      - Total number of canceled flights, delayed flights and average delay per state:
              A US Heatmap with a button to select the year and the disered metric.
              <br>
      <br>
      - Rate of canceled flights, delayed flights and average delay per state:
              A US Heatmap with a button to select the year and the disered metric.
              <br>
      <br>
      - Network from the routes:
              A network that connects all the airports using the routes on the dataset.
              <br>               
      <br>
      - Map the network for the 350 routes with more flights between 2017-2020:
              A US map with the 350 routes whit more flights on the dataset.
              <br>    
