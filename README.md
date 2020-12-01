# COVID-19-Data-Analysis-
Description of the Project
- The purpose of this project is to find if there is any relationship between the spread of the virus in a country and how happy people are, living in that country. 
- This project is guided by a Coursera course called COVID19 Data Analysis Using Python (instructor: Ahmad Varasteh)
 
Process of the Project

 1- Data Collection 
 
Datasets:
-	COVID19 dataset, published by John Hopkins University which consists of the cumulative number of confirmed cases around the world from 22-1-2020 to 30-4-2020.
-	Worldwide happiness report datasets which consists of various life factors scored by people living in each country around the world.
-	Another COVID19 dataset published by John Hopkins University consists of the cumulative number of deaths caused by COVID-19 around the world from 22-1-2020 to 30-4-2020.

2- Data Cleaning 
-	Import COVID-19 confirmed cases dataset csv file to Jupyter Notebook 
-	Explore the dataset 
-	Drop the unnecessary columns 
-	Aggregate the rows to displays the cases for each country in one row
-	Find a good measure which is in this case is ‘Max Infection Rate’
-	Calculate max infection rate for each country and then dropping the unnecessary columns  
-	Save it as a csv file named COVID19 Confirmed Cases (22-1-2020 to 30-4-2020)
-	Import Worldwide happiness report datasets csv file to Jupyter Notebook
-	Explore the dataset 
-	Drop the unnecessary columns 
-	Index the dataset by country
-	Merge those two datasets into one dataset as pandas data frame named ‘data’
-	Save it as a csv file named Worldwide Happiness Report
-	Import COVID-19 deaths dataset csv file to Jupyter Notebook 
-	Explore the dataset 
-	Drop the unnecessary columns 
-	Aggregate the rows to displays the cases for each country in one row
-	Find a good measure which is in this case is ‘Max Death Rate’
-	Calculate max death rate for each country and then dropping the unnecessary columns  
-	Save it as a csv file named COVID19 Death Rate (22-1-2020 to 30-4-2020)
-	Merge this dataset with the merged data frame (data) 
-	Drop the unnecessary columns  

3- Data Analysis & Visualization 
-	Finding the correlation between max infection rate and the next life factors: GDP per capita, Social support, Healthy life expectancy, & Freedom to make life choices, for each country 
-	Visualizing the correlation by plotting the data & fit it to regression line using seaborn.regplot() function 
-	Calculating the Pearson Correlation Coefficient & P-value of the correlation between GDP & max infection rate because the visualization was showing a possible correlation
-	Concluding the result of this analysis
-	Since this analysis could be biased because the developed countries may have more confirmed cases because they conduct COVID-19 test more than the developing countries, so another analysis should be done to see test the significance of the result
-	 Finding the correlation between max death rate and GDP per capita for each country 
-	Visualizing the correlation by plotting the data & fit it to regression line using seaborn.regplot() function 
-	Calculating the Pearson Correlation Coefficient & P-value of the correlation between GDP & max death rate
-	Concluding the result of this analysis

The Results of the Project

The result of COIVD-19 Confirmed Cases (max infection rate) & Worldwide Happiness Report (life factors):

-	There was a significant positive correlation between the max infection rate (dependent variable) & the GDP of a country (independent variable) (r = 0.2598925070926983 with a P-value of P = 0.0017207018252792102)


![](/images/Correlation_between_max_infection_rate_and_GDP.png)

The result of COIVD-19 Deaths (max death rate) & GPD per Capita:

-	There was significant positive correlation between the death rate and GDP per capita

The main result:

-	These results states that the developed countries are at higher risk of getting COVID-19 infection than developing countries
