# project_1_healthcare

**Anticipating Heart Disease Trends: A Predictive Analysis of US Mortality Rates**

This project seeks to conduct a comprehensive exploratory data analysis (EDA) of heart disease and stroke mortality rates among U.S. adults aged 35 and older from 2000 to 2019. The project will not only analyze historical trends but also develop predictive models to forecast future mortality rates. By examining demographic factors such as age, race/ethnicity, and sex, as well as geographic variations across counties, the project aims to uncover significant patterns and project potential future outcomes.

# Task 1: Data Cleaning
The first step in our data analysis is to ensure the dataset is clean and structured. This process focuses on loading the CSV file, handling missing data, filtering irrelevant information, and ensuring that the data is prepared for analysis.

1. Handling Missing Data:
    - Missing values are a significant challenge, especially when they occur in critical columns such as Data_Value, Confidence_limit_Low, and Confidence_limit_High. Rows with missing values in these columns are dropped, as they are essential for accurate statistical analysis.
    - Two columns, Data_Value_Footnote_Symbol and Data_Value_Footnote, are dropped entirely as they contain no useful information.
2. Column Reduction:
    - Irrelevant columns, like DataSource, are removed from the dataset as they are not needed for the analysis. 
3. Processing the Year Column:
    - Data in the Year column is converted to numeric, with invalid or problematic entries removed. This ensures that the subsequent analysis focuses only on valid data points. We further filter the dataset to include only entries from 2010 to 2019, ensuring that the analysis remains relevant to recent trends.
4. Unique Value Columns:
    - Some columns, like GeographicLevel and Class, contain the same value across all rows. These are dropped since they provide no additional information.
5. Outlier Detection:
    - We identify and remove outliers in the Data_Value column by excluding values beyond the 1st and 99th percentiles. This helps to reduce the impact of extreme data points that could skew the analysis.
6. Renaming for Clarity:
    - To improve clarity and readability, several columns are renamed. 

# Task 2: Data Exploration and Analysis: 
The analysis of the cleaned health dataset reveals significant insights into mortality rates associated with heart disease and stroke across various demographics in the United States. It encompasses three key tasks like data exploration, data transformation and analysis report. In data transformation, we performed exploratory data analysis (EDA) to identify trends, patterns, and outliers. Data transformation involves preparing the data for detailed analysis by creating new variables, aggregating data, and performing preliminary statistical analysis. And the last part is analysis write-up, where we drafted a summary of our major findings and discuss their implications. This structured approach aims to provide valuable insights into mortality trends based on certain attributes like gender, age, race, cause of death. By examining trends over time, demographic disparities, and geographical variations, we can draw meaningful conclusions that may inform public health strategies and policies. The analysis of mortality rates related to heart disease and stroke across various demographics in the United States has uncovered critical trends and disparities that have significant public health implications. Addressing these issues through targeted interventions, a focus on health equity, and continued research will be essential in reducing the burden of these diseases and improving health outcomes for all Americans.
