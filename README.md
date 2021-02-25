# Covid_project
STA 207 project 3

Variables in WHO_new_response.csv

Original variables from WHO dataset:
"Date_reported"     
"Country_code"      
"Country"           
"WHO_region"       
"New_cases"         
"Cumulative_cases"  
"New_deaths"        
"Cumulative_deaths"

New variables:
"New_infectious": Infectious population is defined as people who are infected and have the potential to infect others. New_infectious is the daily increase in infectious populationon day t. 
"lag_infectious": total ifectious population on day t-1.  
"New_infec_07ma": 7-day moving average of daily increase of infectious population  
"lag_infec_07ma": 7-day moving average of day t-1 infectiou population
"New_infec_05ma": 5-day moving average    
"lag_infec_05ma": 5-day moving averag
"New_infec_03ma": 3-day moving averag  
"lag_infec_03ma": 3-day moving averag

Reponse variable: percent change in infectious population on day t, choose one of the following as response variable. They are the same, just based on different moving average values
"delta_infectious"  
"delta_infec_07ma"  
"delta_infec_05ma"  
"delta_infec_03ma" 
