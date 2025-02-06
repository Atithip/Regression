# Regression
A real world regression problem predicting health insurance charges.

## Dataset Summary
This dataset contains information on health insurance customers and is a key to unlocking patterns in healthcare costs.

|Column| 	Data Type	| Description|
|------|------------| ---------------|
|age	  |     int	    |Age of the primary beneficiary.|
|sex	  |     object	|Gender of the insurance contractor (male or female).|
|bmi	  |    float	  |Body mass index, a key indicator of body fat based on height and weight.|
|children|	int	      |Number of dependents covered by the insurance plan.|
|smoker|	object	    |Indicates whether the beneficiary smokes (yes or no).|
|region| object	    |The beneficiary's residential area in the US, divided into four regions.|
|charges| float	    |Individual medical costs billed by health insurance.|

## STEP1: Data Profiling and Preparation
In this project, I followed a structured approach for data profiling and preparation before performing any analysis. Below are the key steps I took:

### 1. Initial Data Profiling
1. Checked Unique Values: I started by reviewing the unique values for each column to understand the range of data in each feature.
2. Missing Values: Identified columns with missing values to ensure proper handling during the cleaning phase.
3. Summary Statistics: I reviewed summary statistics (mean, median, standard deviation) to detect potential outliers and anomalies in the dataset.
4. Frequency Distribution: Analyzed the frequency distribution of categorical features to assess class balance and any potential skew.
5. Duplicate Rows: Checked for duplicate rows to ensure data integrity and remove redundancy.
6. Data Issues: I presented a list of issues found in the dataset (e.g., improperly formatted data, missing values, outliers, and duplicates).
### 2. Data Cleaning
1. Corrected Improper Formats:
- Converted negative values for age and number of children to positive.
- Standardized categorical values for sex and region to ensure consistency.
- Removed the dollar sign from the charges column to convert it to a numerical format.
2. Data Type Adjustments:
- Changed data types for age, children, and charges columns from float and object to int and float where appropriate for easier analysis.
3. Handling Missing Values:
- For age, I replaced missing values with the mean of the column.
- For charges, I calculated the mean of charges where smoker == 'yes' and used that mean to replace missing values in the charges column.
- For children, I replaced missing values with the mode (most frequent value).
- For categorical variables like sex, smoker, and region, I replaced missing values with 'unknown' to maintain consistency in the data.
4. Removed Duplicate Rows: I removed any duplicate rows to ensure the dataset was free from redundancy.
### 3. Final Dataset
After applying the above cleaning steps, I now have a cleaned dataset, ready for further analysis.

## STEP 2: Exploratory Data Analysis (EDA)




