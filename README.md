# Airline-Delay-Analysis

## Introduction
A flight is delayed when it lands or takes off 15min(or more) later than its scheduled time.
Flight delay negatively impacts both the passengers and airline companies.
The aim of this project is to tell a story about flight delays using a flight delay dataset gotten from [Kaggle](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay) 

 ## Brief Overview of the Dataset
 THe dataset contained 8 columns and 539,383. 99% of flights in the data were U.S.A domestic flights while others are flights between U.S.A/Guam, U.S.A/Peurto Rico, U.S.A/Virgin Islands and Virgin Islands/ Puerto Rico. These flights were taken by 18 Airlines between 293 airports.
 ![Screenshot (211)](https://user-images.githubusercontent.com/107176991/180042274-eb22d086-d10c-44a9-b151-8e12d739d0d8.png)
 
## Tools
 - Power Query
 - Power BI
 - Excel

## Outline
- Data Sourcing
- Data transformation with Power Query Editor
- Data Visualization with Power BI
- Giving of Insights
- Reasons for the Insights
- Recommendations

## Data Sourcing
 The main dataset; flight delay dataset was gotten from [Kaggle](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay). 
 Other complementary datasets was also used in this analysis, mainly to make sense of the abbreviations in different columns of the flight delay datasets.
 For example,
 - Airports Data set from [Kaggle](https://www.kaggle.com/datasets/zinovadr/iata-airport-code) to extract the full names of and locations(Country,State,and Municipacity) of the airports in the flight delay dataset.
 - Airlines Dataset from [Kaggle](https://www.kaggle.com/datasets/open-flights/airline-database?resource=download) to extract the full names of the Airlines in the flight delay dataset.
 - U.S.A state/region dataset from [Kaggle](https://www.kaggle.com/datasets/omer2040/usa-states-to-region) to get further information on location of airports in U.S.A
 
 ## Data Cleaning 
 The datasetS were imported into the power query editor from their respective excel files.
 All columns were formatted to the right datatypes.
 The time column in the flight delay dataset was transformed to the hh:mm:ss format
 
 ## Data Modelling and DAX
 The different tables were connected.
 ![Screenshot (176)](https://user-images.githubusercontent.com/107176991/180039797-fcc1a994-4119-4a3a-90d1-2d23703636dc.png)
 Several DAX measures and calculated columns were created e.g measures for total flights, total delayed flights, %delayed flights, etc.
 Dax functions(Related,switch, and concatenate operator(&) ) were used in creating columns that returned the Flight route/Journey between the Origin Airport and Destination Airport at the level of country,state and    municipality. 
   ![Screenshot (221)](https://user-images.githubusercontent.com/107176991/180040401-41b69141-b4d4-4333-a35e-d4ff2927e52f.png)
   
  > Several factors can cause/be associated with flight delay. E.g 
  > - Airline
  > - Airport
  > - Flight Route/Journey
  > - Day of the Week
  > - Time of the day
  > Data Analysis: Different factors that can influence flight delay were compared based on their %delayed flights i.e the proportion of delayed flight as opposed to using the number of delayed flights.

 ## Data Visualizations
  The report is a 4 pages report. Though only one report is visible, others can be accessed through drill through functionality applied to the % delay by Airlines and % Delay by Flight Route Visuals
## Insights
- Over 240,000 flights which accounts for 44.5% of the flights were delayed.
### Airlines
- Southern Airlines had the highest %flights delayed while Mesa Airlines had the least %flight delayed.
- ![Screenshot (225))](https://user-images.githubusercontent.com/107176991/180051035-43870482-ac59-4025-aa94-376a696c1382.png)

### Weekdays
- Wednesdays had the highest % of delayed flights while saturdays had the least
![Screenshot (224)))](https://user-images.githubusercontent.com/107176991/180051572-00def8be-971b-4e6e-993c-ae28926c889f.png)

### Flight Routes
- Flights from U.S.A to Guam and vise versa had the highest percentage of delayed flights. This can be because only one airline(Continental Airlines) flies this route
- Flights from Virgin Islands to Puerto Rico and vice versa had the least % delayed flights with flights being delayed on sundays only
![Screenshot (224))](https://user-images.githubusercontent.com/107176991/180070071-6b7af9c2-dff4-4c19-a6e0-a45c80088851.png)

### Time
- Total  flights is directly proportional to the delayed flights for most routes.
- For U.S.A Domestic Flights: 6:00am  had the highest total flights and delayed flights while 11:00-11:30pm had the least total flights and delayed flights

![Screenshot (226)))](https://user-images.githubusercontent.com/107176991/180051972-0c52ad5d-a868-4a7b-8b55-dd57250bcabe.png)

### Airports
  Chicago Midway International airport had the highest % of delayed Flights while Texakana Regional Webb Field had the least.
  ![Screenshot (228)](https://user-images.githubusercontent.com/107176991/180073230-2560b9dd-7bd8-47e1-b0b7-8b97d2264ac6.png)

  

Interact with the report [here](https://app.powerbi.com/view?r=eyJrIjoiMDMxMzNhN2EtNjhiMC00NTZkLWE4NGMtNGM4NGNlODcwOGExIiwidCI6IjNjOWJiNWVjLTU3NmItNDY2NS05N2Y0LTlmNDBmYzQ1YTRjMiJ9&pageName=ReportSectiona99a6715b29aa7ff6508)



      
 
