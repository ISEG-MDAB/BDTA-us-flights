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
      - Number of movies produced by year (Genre comparison):
              An interactive scatter plot that allows the user to choose two genres and analyze the evolution of     the number of movies produced by year, for the two corresponding genres.
              <br>
      - Average rating per movie genre, per year:
              An interactive bar chart in which the user selects the year, and visualizes the average rating of the movies per genre, for that particular year.
              <br>
      - Movie rating evolution per actor/actress - Average Rating:
              A combination of a bar chart and a scatter plot to analyze the average rating of the movies in which a particular actor/actress worked on. By choosing an actor/actress, the user will se a bar chart with the overall average rating of the movies for him/her and a scatter plot with the evolution of the movie ratings through the years.
              <br>
      - Versatility indicator:
              The last visualization is an interactive indicator to analyze the versatility of an actor/actress. To do so, an indicator of versatility was developed (further details on the corresponding notebook).
              <br>
  - <b><i>Rating_prediction.ipynb</i></b> : a jupyter notebook to develop prediction of the ratings based on movie features.
  
      To predict the rating of a movie, the following models were tested:
      <br>
      - Linear Regression model;
         <br>
      - Ridge model (alpha = 0.5);
         <br>
      - Lasso Model (alpha = 0.5);
         <br>
      - Bayesian Ridge;
         <br>
      - Neural Network;
         <br>
      - Keras model.
         <br>
  
  All the information and details regarding the development of the models is available on the correspondent notebook.
  
  For further research on the models' properties, all documentation is available at: 
  
 - https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html <i>(Linear Regression models)</i>
      
 - https://www.tensorflow.org/api_docs/python/tf/keras/Sequential <i>(Keras model)</i>
  
  <i>Disclaimer : </i> Due to the big volume of data on these data sets, the rating prediction models were developed using movie data for movies produced in 2020 and 2021.
  
  <br>
  
  - <b><i>Computer_Vision.ipynb</i></b> : on the final notebook of this project, you will find a short approach to computer vision applied to the IMDb data base. 
  
  On this stage of the project, we aimed at developing a process in two phases:
      <br>
      - 1st: reading the front cover of a movie and identifying the title through the image;
      <br>
      - 2nd: automaticlly searching on the IMDb data based by the movie name obtained at stage 1.
      
<br>

 - <b><i>Report.pdf</i></b> : You will also find a report of the project, where results are discussed and analysis made of the overall work.

<br>
<b><i>We hope you find this project as interesting as we did while developing it.</i></b>
