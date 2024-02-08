# Medical Staffing Plan: Project Overview
Hospitals and clinics face a substantial influx of patients during influenza seasons, placing significant demands on healthcare staff and patients seeking treatment. To address this challenge, I developed a strategic plan to assist a staffing agency in efficiently deploying medical personnel across the United States during influenza seasons.

### [YouTube Project Walk-Through](https://youtu.be/UtJXxrL7UzY)
### [Tableau Dashboard](https://public.tableau.com/views/U_S_InfluenzaData2010-2017/Story1?:language=en-US&:display_count=n&:origin=viz_share_link)

## Data 
Influenza death counts were obtained from the Centers for Disease Control’s National Center for Health Statistics (NCHS). Influenza deaths are identified by each state's statistics office using diagnostic codes to record cause of death. Individuals are grouped by age range, and month and year of death from 2009 to 2017. Counts were not available for the District of Columbia.

U.S. Census Bureau population data was recorded annually for each state and its counties from 2009 to 2017. Data includes total population, male total population, female total population, and population by age group.

Records of patients with influenza-like illnesses (ILI) and provider data was provided by the U.S. Outpatient Influenza-like Illness Surveillance Network (ILINet). The data set includes the average percentage of ILI and number of healthcare providers available by state from 2010 to 2019. ILI visits only capture respiratory-related illnesses with symptoms of fever plus cough or sore throat, which may over represent the number of influenza visits. Data was not available for the state of Florida in this data set.

## Tools & Skills
**Excel**
* Data cleansing and transformation using Pivot tables and CONCATENATE function to ensure data quality and consistency.
* Integration of data sets using combined keys and XLOOKUP function.
* Statistical hypothesis testing to define outliers and correlations using VAR, STDEV, AVERAGE, and CORREL functions.
  
**Tableau**
* Data manipulation and transformation.
* Spatial analysis techniques.
* Forecasting using statistical methods to facilitate proactive planning and resource allocation.
* Data storytelling using visualizations.

## Purpose & Context
This project was a part of CareerFoundry's Data Immersion curriculum and was evaluated by my tutor and mentor. I defined the project's scope and selected the optimal format for the final presentation.

## Data Cleaning, Integration, & Transformation
* Duplicate records in the U.S. Census dataset were eliminated, ensuring the retention of unique combinations of County, Year, and Population.
* Missing values in the "Influenza Death" dataset belong to D.C. Imputed missing values as "District of Columbia".
* Columns and rows containing irrelevant or missing data were removed.
* Integer values, such as population counts, were converted from decimals into whole numbers. State abbreviations were transformed into their full names.
* Year "20133" in the "Influenza Death" dataset was corrected to "2013".
* Age groups were restructured into a consistent format, allowing for seamless integration of datasets.
* Created a new variable that normalizes the mortality rates for each age group.

## Visualizations
This line graph shows that there is an upward trend in influenza patients, which suggests that influenza rates are getting worse over time. I needed to find out which states had confirmed influenza deaths in order to locate affected areas.

<img src="images/Line%20Influenza%20Patients.png"/>

Spatial analysis played a pivotal role in this project. An intuitive color gradient was used on a density map of the U.S., directing the viewer's attention to regions most significantly impacted by influenza infections.

States exhibiting a darker red shading indicate higher counts of influenza-related deaths across all age groups. Additionally, large and darker-shaded dots within each state correspond to areas with larger total population sizes.

California and Texas stand out with the most significant population sizes, while New York and California are the states reporting the highest counts of influenza-related deaths. 

<img src="images/Map%20U.S.%20Deaths%20%26%20Pop..png" />

I explored the proportions of age groups within each state's population, guided by the assumption that specific age groups may exhibit a higher susceptibility to influenza infections than others. The resulting line chart illustrates the sum of influenza-related deaths across all age groups, shedding light on the seasonality of these infections. January has the highest number of influenza-related deaths, while August has the lowest. This seasonality provides valuable information for healthcare planning and resource allocation.

Aage groups 45 years and older exhibit the highest rates of influenza-related deaths and are identified as vulnerable populations in this analysis.

<img src="images/Line%20Deaths%20by%20Month.png"/>

This stacked bar chart conveys the proportion of vulnerable age group populations within each state. Maine has the largest proportion of vulnerable age groups and Utah has the lowest.

<img src="images/%25%20All%20Ages.png"/>

The following two images provide insights into influenza-related deaths for age groups 45 and older. The first image presents a map displaying shades of red as the count of deaths, and large, shaded dots as population size. California and New York continue to stand out as states most significantly affected.

<img src="images/Map%20Deaths%2045-85%20%26%20Pop..png"/>

The second map introduces a more precise measure known as the weighted average mortality rate. This measure was calculated by considering the proportion of each vulnerable age group's population and the total mortality rate for that specific age group. The map uses a mortality rate scale that assigns darker red shading to indicate high mortality and lighter pink for low mortality. Gradations within the scale are labeled as follows: low, low-moderate, moderate, moderate-high, and high.

This refined measure provides a deeper understanding of the impact of influenza, revealing more states that are significantly affected by the virus. Notably, California is no longer one of the top states, emphasizing the importance of using precise metrics for decision-making.

When determining staffing allocation, it's essential to consider this measure to ensure that states with high mortality rates receive sufficient staff to maintain a minimum 90% staff-to-patient ratio, with allowances up to 110% to avoid overstaffing. Additionally, the incorporation of historical seasonality data enables the prediction of when additional staff will be needed, contributing to effective and proactive resource management during influenza seasons.

<img src="images/Map%20WA%20Mort.%20Rate%2045-85%2B%20(2)%20(1).png"/>

The presented bar chart illustrates the number staff-to-influenza patient ratios for each state. Several key observations emerge from this analysis:

* Montana and New Hampshire are notably overstaffed, with a low to low-moderate mortality rate, respectively. This suggests that these states have a surplus of medical staff in proportion to their influenza patient populations.
* The District of Columbia (D.C.) stands out as the most understaffed, indicating a significant shortage of medical personnel in this region. However, it's worth noting that influenza death counts were not available in the dataset used for this analysis.
* Louisiana and Georgia exhibit low percentages of medical staff in relation to their influenza patient populations. These states also have moderate-high and high mortality rates, respectively.

The analysis reveals a potential correlation between staffing levels and mortality rates, suggesting that states with more medical staff than influenza patients tend to have lower mortality rates. The project's goal is to bolster the number of medical staff in states with low staffing levels to achieve a noticeable decline in influenza-related mortalities. 

<img src="images/Staff%20to%20Patient%20ratio%20(1).png"/>

## Recommendations & Findings
* The staffing agency should initiate the allocation of medical staff prior to January each year when influenza death counts are at their peak. This proactive approach ensures that states are adequately prepared to address the surge in cases during peak influenza seasons.
* Utilize the weighted average mortality rate and staff-to-patient ratio to determine the number of staff members required for each state. This data-driven approach aligns staffing levels with the specific needs of each region.
* Incorporate real-time updates into the dashboard to address staffing needs more precisely. Real-time data ensures that the allocation of medical staff remains responsive to evolving conditions.
* The state of Florida should provide the necessary number of providers and influenza patient data to determine accurate staff-to-patient ratios.
* Extend the analysis to measure other factors that may affect influenza rates, such as access to vaccinations and education on influenza prevention. A more comprehensive understanding of these factors can inform targeted interventions to reduce influenza-related morbidity and mortality.

## The Learning Experience
My most significant challenge was creating self-explanatory visualizations in Tableau. I researched tutorials and troubleshooting strategies to align my outcomes with my initial objectives. One of the pivotal variables in this analysis was the weighted average mortality rate, a metric whose development was facilitated by the guidance of my mentor. I envisage leveraging this calculation in upcoming projects, having gained an understanding of its potential impact on outcomes. The walkthrough of each procedural step enabled me to weave a coherent narrative for my final presentation. During this process I unearthed unexpected findings that catalyzed novel explorations to incorporate into my project.

## Datasets
* *Underlying Cause of Death, 1999-2020* [Data set]. Centers for Disease Control and Prevention. https://wonder.cdc.gov/ucd-icd10.html
  
* *Population data by geography* [Data set]. U.S. Census Bureau, CSV file. https://coach-courses-us.s3.amazonaws.com/public/courses/data-immersion/A1-A2_Influenza_Project/Census_Population_transformed_202101.csv
  
* *Outpatient Illness Surveillance* [Data set]. U.S. Outpatient Influenza-like Illness Surveillance Network (ILINet), Excel file. https://images.careerfoundry.com/public/courses/data-immersion/A1-A2_Influenza_Project/CDC_Influenza_Visits.xlsx
