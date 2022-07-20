# Airline-Delay-Analysis
## Introduction
The aim of this project is to tell a story about flight delays using a flight delay dataset gotten from [Kaggle](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay) 
## Tools
 - Power Query
 - Power BI
 - Excel
## Tasks
- Data transformation with Power Query Editor
- Data Visualization with Power BI
## Data Sourcing
 The main dataset; flight delay dataset was gotten from [Kaggle](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay). 
 Other complementary datasets was also used in this anaalysis, mainly to make sense of the abbreviations in different columns.
 ## Data Cleaning 
 The flight delay dataset was imported into the power query editor from the excel file.
 All its columns was formatted into the right datatypes
 The time column was formated to the hh:mm:ss format
 The other datasets was also imported and only the columns needed from them were retained.
 ## Data Modelling and DAX
 The different tables were connected for ease of visualization
 ![Screenshot (176)](https://user-images.githubusercontent.com/107176991/180039797-fcc1a994-4119-4a3a-90d1-2d23703636dc.png)
   and several DAX measures were created e.g measures for total flights, total delayed flights, %delayed flights, etc.
   ![Screenshot (221)](https://user-images.githubusercontent.com/107176991/180040401-41b69141-b4d4-4333-a35e-d4ff2927e52f.png)
 ## Brief Overview of the Dataset
 THe dataset contained 8 columns and 539,383. 99% of flights in the data were U.S.A domestic flights while others are flights between U.S.A/Guam, U.S.A/Peurto Rico, U.S.A/Virgin Islands and Virgin Islands/ Puerto Rico. These flights were taken by 18 Airlines between 293 airports.
 ![Screenshot (211)](https://user-images.githubusercontent.com/107176991/180042274-eb22d086-d10c-44a9-b151-8e12d739d0d8.png)
## Insights
- Over 240,000 flights which accounts for 44.5% of the flights were delayed.
- Southern Airlines had the highest %flights delayed while Mesa Airlines had the least %flight delayed.
-Wednesdays had the highest % of delayed flights while saturdays had the least
## Flight Routes
Flights from U.S.A to Guam and vise versa had the highest percentage of delayed flights. 
This can be attributed due to the following reasons:
- Only one airline:Continental Airlines flies this route
- Flights in this route doesn't run on weekends(Saturdays and a Sundays), this further impacts Friday flights for U.S.A/Guam routes as all Friday flights for this routes were delayed.
- ![Screenshot (222)](https://user-images.githubusercontent.com/107176991/180045881-3fdd4bc9-cbaf-40b0-995b-41cc0e374684.png)



      
 
