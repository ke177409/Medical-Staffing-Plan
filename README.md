# Medical-Staffing-Plan: Project Overview
Created a plan to help a staffing agency distribute medical staff throughout the United States during influenza seasons.
Performed data cleansing and statistical analyses on U.S. Census and CDC data sets using Excel and Tableau.
Developed visualizations to perform spatial analyses using Tableau.
Built a client dashboard using Tableau.

## YouTube Project Walk-Through
https://youtu.be/vcfuhCl_TEA

## Tools & Skills
Excel
* Data cleansing, transformation, and integration
* Statistical analysis
  
Tableau
* Visualizations
* Spatial Analyis

## Purpose & Context
This project was a part of CareerFoundry’s Data Immersion curriculum. I was tasked to perform an exploratory analysis on multiple data sets using Excel and Tableau. Each part of this project was evaluated with feedback by a tutor and mentor. 
I was responsible for deciding on the project scope and final presentation format.

## Data Cleaning, Integration and Transformation
I began by reviewing and correcting errors within each data set. Certain age groups, years, and states had missing data which I removed or flagged after considering any effects on the results.
The use of separate data sets was getting messy, so I decided to use common variables to integrate them into one large data set. I also created a new variable using a weighted average to calculate mortality rates more 
accurately in each state.

## Visualizations
Spatial analysis was crucial for this project’s goal. With the use of an intuitive color gradient, I was able to create a map of the United States that draws the viewer’s eyes to areas most affected by influenza 
infections.
<p align="center">
  <img src="https://github.com/ke177409/Medical-Staffing-Plan/assets/118031032/a725ebdd-f43c-4ba7-af73-8a44ff0f1b08" width="475" height="323"/>
</p>

Portraying multiple variables in one visualization helped me uncover insights that were not easily identifiable from the raw data. For example, states with more medical staff than influenza patients also 
tend to have lower mortality rates. 
![Staff to Patient ratio (1)](https://github.com/ke177409/Medical-Staffing-Plan/assets/118031032/ba912df1-fc30-4bed-9866-db2145011bde)

## Recommendations and Findings
* The staffing agency should begin allocating medical staff prior to January each year when influenza death counts are highest.
* The weighted average mortality rate and staff-to-patient ratio should be used to determine how many staff members need to be sent to each state.

## The Learning Experience
My biggest challenge was learning to create visualizations in Tableau that speak for themselves. I researched tutorials and troubleshooting strategies to achieve my intended results.
The weighted average mortality rate was one of my key variables in this analysis and was developed with the help of my mentor. I intend to use this calculation in future projects after understanding how it can 
influence results.
Walking through each step of my process helped me to develop a coherent story for my final presentation. During this process I discovered results that were unexpected, which sparked new ideas to explore and more 
details to add to the project.

## Datasets
* “Influenza deaths by geography, time, age, and gender”, Source: CDC (https://wonder.cdc.gov/ucd-icd10.html)
* “Population data by geography”, Source: US Census Bureau (https://coach-courses-us.s3.amazonaws.com/public/courses/data-immersion/A1-A2_Influenza_Project/Census_Population_transformed_202101.csv)
* “Counts of influenza laboratory test results by state”, Source: CDC Fluview (https://images.careerfoundry.com/public/courses/data-immersion/A1-A2_Influenza_Project/CDC_Influenza_Visits.xlsx)
