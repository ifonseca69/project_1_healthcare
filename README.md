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

# Task 2: Data Exploration and Analysis
In this phase, we focus on exploring the cleaned health dataset to gain key insights into mortality rates related to heart disease and stroke across various demographics in the United States. The process is divided into three main steps: data exploration, transformation, and report generation.

1. Data Exploration:
    - We begin with exploratory data analysis to investigate trends, patterns, and potential outliers. This step helps us understand the relationships between variables such as age, gender, race, and cause of death.
    - Line plots and boxplots are used to assess mortality trends over time and compare distributions across different demographic groups.
2. Data Transformation:
    - The dataset is prepared for detailed analysis by creating new variables, aggregating data, and conducting preliminary statistical analysis. This involves grouping data by key factors (e.g., year, cause of death, demographic group) and calculating summary statistics, such as means and variances.
    - Additional transformations include handling skewed data and normalizing variables where necessary.
3. Analysis Report:
    - We drafted a summary of our findings, interpreting the trends and patterns uncovered during the analysis. This report highlights significant insights into mortality disparities across gender, age, race, and geographical location, with a focus on heart disease and stroke.

By systematically exploring trends over time, demographic disparities, and geographical variations, we uncover critical patterns that have important public health implications. Addressing these issues through targeted interventions, a focus on health equity, and ongoing research is essential to reducing the burden of heart disease and stroke and improving health outcomes in the United States.

What we need to add: 
1. Usage and installation instructions
2. Examples of the application
3. The results and a summary of the analysis
