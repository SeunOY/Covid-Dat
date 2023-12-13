Covid Analysis


The COVID-19 Data Analysis was done to gain insights into the COVID-19 pandemic, leveraging extensive datasets that include total infection, vaccination coverage, hospitalisation records, demographic information, and socioeconomic indicators, the analysis seeks to uncover patterns and correlations that can inform targeted interventions and policy adjustments.

I assumed the position of a data analyst to generate insights on metrics such as the death rate, vaccination rate, and peak cases across countries in different continents. This data provides the backdrop to make informed decisions about vaccine supply, rate of infection and the possibility of dying from COVID-19.

The data was cleaned to ensure there were no duplicates and null values.

Objectives/Ask

What was the highest record for new COVID cases in each country?
The Infection Rate Per Country
The Death Rate Per Country
Vaccination Efficacy Per Country 
Number of people vaccinated/vaccinated percentage in each continent 
Number of people vaccinated/vaccinated percentage in each continent 


What was the highest record for new COVID-19 cases in each country? The highest daily record for each country was determined with the query below. As each daily record was entered with the same population for each country, grouping on location was done to ensure that the result populated data for each country.




The Infection rate per country was determined by running the query below


The death rate for each country was determined with the query below:




The vaccinated population in each country was determined by running queries on joined CovidDeaths & CovidVaccinattions table



The percentage infected in each continent was determined by joining 2 Common Table Expressions (CTE) to determine the total cases in each continent and the total population in each continent. A join was created to query the 2 CTEs and determine the max running total for COVID cases and population of each continent and calculations were performed on them to determine the percentage population infected in each continent.  The query can be seen below.





	2.



A similar query was done to populate the total vaccinated population of each continent but by querying the running total of the new vaccination field in the Covid Vaccine Table and the new_cases field in the Covid Deaths Table.

 





Key insights from the data are provided below. A more interactive visualisation of these insights can be found here.


America had the highest vaccination rate with 44% of its population vaccinated till present

The highest number of infections compared to the total population is observed in Andorra with a population of 77,265%  and an infection rate of 17.1255%.

Israel, UAE & Chile had the highest vaccination rates at 121.278%, 95.799%, 77.248% respectively while countries like Algeria, Cameroon, and Myanmar had vaccination rates that were close to zero and almost negligible 

Hungary, Czechia, and San Marino had the highest death rate with records of 0.28%, 0.27%, 0.27% compared to countries with larger populations like China, India & United States with death rates of 0.000335%, 0.015352%, 0.174087%.
 



Recommendations:


Countries like Algeria, Cameroon, Myanmar should implement a strategy to increase the total vaccinated population to reduce incidents of infections.

