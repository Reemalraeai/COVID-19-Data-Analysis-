
# COVID-19-Data-Analysis-
Description of the Project
- The purpose of this project is to find if there is any relationship between the spread of the virus in a country and how happy people are living in that country. 
- This project is guided by a Coursera course called COVID19 Data Analysis Using Python (instructor: Ahmad Varasteh)
 
Process of the Project 

 1- Data Collection 
 
Datasets:
-	COVID19 dataset, published by John Hopkins University which consists of the cumulative number of confirmed cases around the world from 22-1-2020 to 30-4-2020.
-	Worldwide happiness report datasets which consist of various life factors scored by people living in each country around the world.


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
-	Merge those two datasets into one dataset as Pandas data frame named ‘data’
-	Save it as a csv file named Worldwide Happiness Report


3- Data Analysis & Visualization 
-	Finding the correlation between max infection rate and the next life factors: GDP per capita, Social support, Healthy life expectancy, & Freedom to make life choices, for each country 
-	Visualizing the correlation by plotting the data & fit it to regression line using seaborn.regplot() function 
-	Calculating the Pearson Correlation Coefficient & P-value of the correlation between GDP & max infection rate to confirm any possible correlation
-	Visualizing residual plot to evaluate whether the possible relationship is a linear relationship or not
-	Concluding the result of this analysis
-	This analysis could be biased because the developed countries may have more confirmed cases because they conduct COVID-19 test more than the developing countries.


The Results of the Project

The result of COIVD-19 Confirmed Cases (max infection rate) & Worldwide Happiness Report (life factors):
-	The max infection rate of a country positively correlated the GDP, the Social support, the healthly life expectancy (moderate correlation) and the freedom of a choice of that country.
-	Hence, we can state that happier countries tend to be at higher risk of getting COVID-19 infection.
-	However, this could be biased since happier countries tend to be developed countries and they are more prone to COVID-19 than developing countries 


![](/images/Correlation_between_max_infection_rate_and_GDP.png)

Pearson Correlation Coefficient = 0.5877934046059671, P-value = 1.1839643617609705e-14
Significant moderate positive correlation


![](/images/Correlation_between_max_infection_rate_and_Social_Support.png)

Pearson Correlation Coefficient = 0.410553554663816, P-value = 3.528589753399903e-07
Significant moderate positive correlation


![](/images/Correlation_between_max_infection_rate_and_Healthy_life_expectancy.png)

Pearson Correlation Coefficient = 0.5456787753328285, P-value = 1.8185734429629742e-12
Significant moderate positive correlation



The main result:
-	Happier countries tend to be at higher risk of getting COVID-19 infection.
