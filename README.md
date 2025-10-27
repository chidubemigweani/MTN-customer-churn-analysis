# MTN Customer Churn Analysis

### Project Overview

A dataset containing the information of MTN customers, this information includes details like Full Name, MTN Device, Satisfaction Rate, Customer Review, Data Usage, Customer Churn Status

### Data Source

mtn_customer_churn.csv: The primary dataset used for this analysis was the "mtn_customer_churn.csv" csv file gotten from Kaggle, containing detailed information about MTN customers

### Tools

- Python - Data Manipulation
- Python & SQL - Exploratory Data Analysis
- Power Bi - Visualization

### Data Cleaning/Preparation

In the initial data preparation phase, I performed the following tasks:
1. Data loading & Inspection
2. This dataset is gotten from Kaggle is cleaned and formatted before download.
3. Analysis
4. Visualization

### Exploratory Data Analysis (EDA)

EDA involved exploring the data to answer key questions such as:
- How does data plan usage relate to customer reviews?
- Are there any unusual patterns or outliers in the data?
- What is the age distribution of all customers? Are customers with 'Poor' reviews generally younger or older?`
- Which 5 states have the highest number of customers in this dataset?
- Are there any states where one Customer Review category (like 'Poor') is far more common than others?
- Does the type of device a customer uses correlate with their Satisfaction Rate?
- Which plans are most associated with 'Excellent' reviews?
- What is the distribution of Customer Tenure? (Are most customers new, or long-term?)
- Is there a relationship between how much a customer spends (Total Revenue) and their Satisfaction Rate? (Are high-spenders happier?)

### Data Analysis

For the data analysis, Pandas was data manipulation, filtering out data using it's group by and subsetting methods. To find the distribution of certain factors, a histogram was plotted. The following methods are what I implemented while using pandas for data manipulation
1. .read_csv('mtn_customer_churn.csv') was used to import the dataset to Jupyter
2. .head(10) was used to print just the top 10 rows from the dataset
3. .value_counts(normalize=True) * 100 was used to find the states with most poor reviews in percentage
4. .sort_index() as the name implies was used to sort age with the percentage of poor reviews after narmalizing it's value_counts
5. .mean() was used to find the mean(average) of the indicated column
6. .hist(bins = 5) was used to plot a histogram, specifying the number of bins it should contain

The rest of the analysis was carried out in MySQL workbench windows application using SELECT queries in selecting, grouping and aggregating columns to find specific results

### Results/Findings

The analysis results are summarized as follows:
1. There is no clear relationship between customer review and data plan usage.
2. No outliers in age, tenure, unit price. There are outliers in total revenue. There are no unsual patterns in reviews and state.
3. Age is uniformly distributed, there's no clear relationship between customer age and their poor reviews.
4. Osun (43), Abuja (FCT) (42), Borno (38), Bauchi (35), Abia (35).
5. Nasarawa has the most 'Poor' reviews (14) than other states
6. Broadband MiFi are the happiest due to the highest averate rating of 3.0219
7. 60GB Monthly Broadband Plan
8. The distribution is a uniform distribution, though most customers are long-term (3-5 years with 260 out of 494 customers)
9. Customers with 200,000 and above have an average satisfaction rate of 2.9 compare to 2.96 of customers with lower than 200,000 revenue

### Limitations

No limitations

### References

None
