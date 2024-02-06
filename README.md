## U.S-D.O.T-Air-2015-Flight-Analysis

### Data Source:

Quantum Analytics NG

### Tool Used: 
 
 Power BI 

 
### DATA OVERVIEW
The dataset contains over 5 million rows and 36 columns. The table gave information about various airports, airline, the year (2015), the month and day during which various activities regarding airline operations took place.

### DATA CLEANING

- The data set contained a lot of null values which were replaced with 0. - The airport names were in a 3-letter codes and these were replaced with the full names for easy understanding of the dashboard. - Cancelation reasons are coded as A,B,C & D. These were defined using a conditional column to specify what reason they mean.

  
###  DATA VISUALIZATION KPIs

- Total Flights = Countrows(flight)
  
- Total Delayed Departure = Calculate ([Total Flight]' Flight ' Delay departure > 0)
 
-  %Delayed Departure = Calculate ([Total Delayed Departure]/[Total Flight] x 100)
  
 
- Total Cancelled Flights
  
-  % Cancelled Flights = [Total Cancelled Flights]/ [Total Flights] x 100
  
- Total Ontime Flight = Calculate ([Total Flight], flight [Departure Delay]<=0) Total Airlines = DistinctCount(flight [Airlines])

- Average Delay Time = Average ('flights'[Departure Delay]) 
 
###  Charts

-  Total Flights by Day of the week 

 
- Total Flights by Month Proportions of reasons of cancelation
  
-  % Departure by Months Airline Reliability by Ontime Departure.
  
-  % Delayed Departure by months in Boston.
  
