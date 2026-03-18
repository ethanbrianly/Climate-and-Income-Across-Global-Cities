# Climate-and-Income-Across-Global-Cities
**Project Overview**
This project records the average temperature and income of cities dispersed across the world from two separate datasets. Using a joined table, I analyzed the relationship between these two factors on a global scale.

Research Question:
Is a city's temperature related to its economic prosperity?

Datasets:
Temperature Dataset:
  - Rows: Day (2015-01-01 to 2019-12-31) 
  - Columns: Country and City (Ex: Afghanistan-Farah)
  - Values: Temperature Recorded (℃)
Income Dataset:
  - Rows: City, Region, Country (separate rows)
  - Columns: Years (2010-2020)
  - Values: Yearly Average Incomes (in USD)

**Tools Used**
  
  - Python	
    - Pandas
  - Excel
  
**Data Cleaning & Preparation**
  -Removed rows with null or redundant values
  -Transposed temperature table to match the format of the income table 
  -Separated country and city into two different columns to join tables efficiently 
  -Found the average temperature each year for every city using daily records
  -Standardized city names
  -Joined tables on the condition of having the same city 
343 cities were matched during the process. 

**Exploratory Analysis**
Visualization: Scatterplot of temperature vs income.
  -X-axis: Average temperature
  -Y-axis: Average income
  -Trendline: y = -40.32x + 1858
The trendline showed a negative relationship, indicating that places with higher temperatures generally experienced more economic struggle.
  -R² = 0.0677
However, the R2 value was quite low, conveying that the data points did not fit the regression model well.

**Conclusion**
Although the data displayed a negative relationship between temperature and income, this relationship is not strong enough to make a definitive statement about the correlation. This suggests that even though temperature could be a factor of economic prosperity, there are likely many other factors that have larger effects. 

**Limitations**
Unfortunately, my final dataset was only able to observe the patterns of 343 cities when it has been estimated that there are over 10,000 cities in the world. Additionally, the income data may not fully reflect economic well-being due to differences in cost of living across the world. In the future, if the data was available, I would’ve implemented other indicators such as unemployment rates. 
