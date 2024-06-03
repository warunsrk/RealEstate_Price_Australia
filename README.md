# RealEstate_Price_Australia <br>
Perform multiple hypothesis testing on real estate prices in the Australian dataset to manipulate real-world data and answer statistical questions.

**Instructions:** <br>
These problems will test you on your ability to manipulate real-world data and answer statistical questions. Use the property.csv dataset to arrive at the solutions. The data is on real estate prices in Australia. 

**Explanation of Each Step:** <br>
Importing Libraries: Import pandas for data manipulation.<br>
Loading the Dataset: Read the dataset from a CSV file into a DataFrame. <br>
Checking for Missing Values: Use isnull().sum() to find columns with missing values. <br>
Handling Missing Values: Fill or drop missing values as needed. <br>
Converting Data Types: Ensure all columns have appropriate data types. <br>
Removing Duplicates: Remove any duplicate rows to ensure data integrity. <br>
Standardizing Categorical Data: Ensure consistency in text-based data. <br>
Checking and Correcting Outliers: Optionally remove outliers to clean the data further. <br>
Verifying Data Cleaning: Re-check the dataset to ensure all issues have been addressed and save the cleaned data. <br>

**Use this data to test the following hypothesis:** <br>

**Question 1**. For the suburb Altona, it is postulated that a typical property sells for $800,000. Use the data at hand to test this assumption. Is the typical property price really $800,000 or has it increased? Use a significance level of 5%.

**Here are the steps followed:** <br>
Loading the Data: The data is loaded into a Pandas DataFrame. <br>
Filtering for Altona: We filter the data to include only rows where the suburb is 'Altona'. <br>
Extracting Prices: We extract the 'Price' column for Altona and drop any missing values. <br>
Calculating Statistics: We calculate the mean and standard deviation of the property prices. <br>
One-Sample T-Test: We perform a one-sample t-test comparing the mean property price to $800,000. <br>
Result Interpretation: We print the results and determine if we reject the null hypothesis based on the p-value. <br>

**Interpretation:** <br>
Mean price: The average price of properties in Altona from the sample data. <br>
Standard deviation: The variability of the property prices. <br>
T-statistic and P-value: Values from the t-test used to determine the significance of the result. <br>
Decision: Based on the p-value and the significance level (α = 0.05), we decide whether to reject the null hypothesis. <br>

**Question 2**. For the year 2016, is there any difference in prices of properties sold in the summer months vs winter months? Consider months from October till March as winter months and rest as summer months. Use a significance level of 5%. 

**Here are the steps followed:** <br>
Loading the Data: The data is loaded into a Pandas DataFrame. <br>
Date Conversion: The 'Date' column is converted to a datetime format.<br>
Filter for 2016: We filter the data to include only rows where the sale occurred in 2016.<br>
Categorize Months: We create two categories: winter months (October to March) and summer months (April to September).<br>
Extract Prices: We extract the property prices for winter and summer months. <br>
Independent Samples T-Test: We perform an independent samples t-test to compare the mean prices of the two groups.<br>
Result Interpretation: We print the mean prices, t-statistic, and p-value, and determine if we reject the null hypothesis based on the p-value and significance level (α = 0.05). <br>

**Interpretation:** <br>
Mean Prices: The average price of properties sold in winter and summer months. <br>
T-statistic and P-value: Values from the t-test used to determine the significance of the result. <br>
Decision: Based on the p-value and the significance level (α = 0.05), we decide whether to reject the null hypothesis.<br>

**Question 3:** For the suburb of Abbotsford, what is the probability that out of 10 properties sold, 3 will not have car parking? Use the column car in the dataset. Round off your answer to 3 decimal places. <br>
**Probability that out of 10 properties sold, 3 will not have car parking** <br>

**Here are the steps followed:** <br>
Filtering Data: We filter the dataset to include only properties in Abbotsford.<br>
Calculating Proportion: We calculate the proportion of properties without car parking.<br>
Binomial Distribution: We use the binomial probability mass function (pmf) to find the probability.<br>

**Question 4:** In the suburb Abbotsford, what are the chances of finding a property with 3 rooms? Round your answer to 3 decimal places. <br>
**Probability of Finding a Property with 3 Rooms** <br>

**Here are the steps followed:** <br>
Counting Properties with 3 Rooms: We count the number of properties with 3 rooms. <br>
Calculating Proportion: We calculate the proportion of properties with 3 rooms. <br>

**Question 5:** In the suburb Abbotsford, what are the chances of finding a property with 2 bathrooms? Round your answer to 3 decimal places. <br>
**Probability of Finding a Property with 2 Bathrooms** <br>

**Here are the steps followed:** <br>
Counting Properties with 2 Bathrooms: We count the number of properties with 2 bathrooms. <br>
Calculating Proportion: We calculate the proportion of properties with 2 bathrooms. <br>
