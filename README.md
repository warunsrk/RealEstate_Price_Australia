# RealEstate_Price_Australia
Perform multiple hypothesis testing on real estate prices in the Australian dataset to manipulate real-world data and answer statistical questions.

**Instructions:** \n
These problems will test you on your ability to manipulate real-world data and answer statistical questions. Use the property.csv dataset to arrive at the solutions. The data is on real estate prices in Australia. 

**Explanation of Each Step:**
Importing Libraries: Import pandas for data manipulation.

Loading the Dataset: Read the dataset from a CSV file into a DataFrame.
Checking for Missing Values: Use isnull().sum() to find columns with missing values.
Handling Missing Values: Fill or drop missing values as needed.
Converting Data Types: Ensure all columns have appropriate data types.
Removing Duplicates: Remove any duplicate rows to ensure data integrity.
Standardizing Categorical Data: Ensure consistency in text-based data.
Checking and Correcting Outliers: Optionally remove outliers to clean the data further.
Verifying Data Cleaning: Re-check the dataset to ensure all issues have been addressed and save the cleaned data.

# Use this data to test the following hypothesis:

**Question 1**. For the suburb Altona, it is postulated that a typical property sells for $800,000. Use the data at hand to test this assumption. Is the typical property price really $800,000 or has it increased? Use a significance level of 5%.

# Here are the steps followed:
Loading the Data: The data is loaded into a Pandas DataFrame.
Filtering for Altona: We filter the data to include only rows where the suburb is 'Altona'.
Extracting Prices: We extract the 'Price' column for Altona and drop any missing values.
Calculating Statistics: We calculate the mean and standard deviation of the property prices.
One-Sample T-Test: We perform a one-sample t-test comparing the mean property price to $800,000.
Result Interpretation: We print the results and determine if we reject the null hypothesis based on the p-value.

# Interpretation:
Mean price: The average price of properties in Altona from the sample data.
Standard deviation: The variability of the property prices.
T-statistic and P-value: Values from the t-test used to determine the significance of the result.
Decision: Based on the p-value and the significance level (α = 0.05), we decide whether to reject the null hypothesis.

**Question 2**. For the year 2016, is there any difference in prices of properties sold in the summer months vs winter months? Consider months from October till March as winter months and rest as summer months. Use a significance level of 5%. 

# Here are the steps followed:
Loading the Data: The data is loaded into a Pandas DataFrame.
Date Conversion: The 'Date' column is converted to a datetime format.
Filter for 2016: We filter the data to include only rows where the sale occurred in 2016.
Categorize Months: We create two categories: winter months (October to March) and summer months (April to September).
Extract Prices: We extract the property prices for winter and summer months.
Independent Samples T-Test: We perform an independent samples t-test to compare the mean prices of the two groups.
Result Interpretation: We print the mean prices, t-statistic, and p-value, and determine if we reject the null hypothesis based on the p-value and significance level (α = 0.05).

# Interpretation:
Mean Prices: The average price of properties sold in winter and summer months.
T-statistic and P-value: Values from the t-test used to determine the significance of the result.
Decision: Based on the p-value and the significance level (α = 0.05), we decide whether to reject the null hypothesis.

3. For the suburb of Abbotsford, what is the probability that out of 10 properties sold, 3 will not have car parking? Use the column car in the dataset. Round off your answer to 3 decimal places.
# Probability that out of 10 properties sold, 3 will not have car parking

# Here are the steps followed:
Filtering Data: We filter the dataset to include only properties in Abbotsford.
Calculating Proportion: We calculate the proportion of properties without car parking.
Binomial Distribution: We use the binomial probability mass function (pmf) to find the probability.

4. In the suburb Abbotsford, what are the chances of finding a property with 3 rooms? Round your answer to 3 decimal places. 
# Probability of Finding a Property with 3 Rooms

# Here are the steps followed:
Counting Properties with 3 Rooms: We count the number of properties with 3 rooms.
Calculating Proportion: We calculate the proportion of properties with 3 rooms.

5. In the suburb Abbotsford, what are the chances of finding a property with 2 bathrooms? Round your answer to 3 decimal places.
# Probability of Finding a Property with 2 Bathrooms

# Here are the steps followed:
Counting Properties with 2 Bathrooms: We count the number of properties with 2 bathrooms.
Calculating Proportion: We calculate the proportion of properties with 2 bathrooms.
