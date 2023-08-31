# Hotel-Business-Analysis-Data-Visualization

### Project Environment and Tools
- Tools: JupyterLab
- Programming Language: Python
- Libraries: NumPy, Pandas, Matplotlib, Seaborn
- Dataset: [hotel_bookings_data](hotel_bookings_data)

### Project Introduction
This project is the second mini project created by an expert tutor at Rakamin Academy. In this project, I will take on the role of a data analyst who performs an analysis of hotel booking data and presents it through data visualization.

### Table of Contents
1. [Business Understanding](#business-understanding)
    a. [Problem Statement](#problem-statement)
    b. [Objective](#objective)

2. [Exploratory Data Analysis](#exploratory-data-analysis)
    a. [Dataset Information](#dataset-information)
    b. [Statistical Summary](#statistical-summary)

3. [Data Preprocessing](#data-preprocessing)
   a. [Handling Missing Value](#handling-missing-value)
   b. [Handling Invalid Data](#handling-invalid-data)
   c. [Removing Uneccesarry Value](#removing-uneccesarry-value)
   d. [Feature Engineering](#feature_engineering).

5. [Data Analysis](#data-analysis)
   a. [Monthly Hotel Booking Analysis Based on Hotel Type](#monthly-hotel-booking-analysis-based-on-hotel-type)
   b. [Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates](#impact-analysis-of-stay-duration-on-hotel-bookings-cancellation-rates)
   c. [Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate](#impact-analysis-of-lead-time-on-hotel-bookings-cancellation-rate)


## :pushpin: Business Understanding
### a. Problem Statement
For a company, it is crucial to consistently analyze its business performance. In this endeavor, we will delve into the hospitality industry, specifically focusing on understanding customer behavior in hotel reservations and its correlation with booking cancellation rates. The insights we uncover will be presented through data visualizations to enhance comprehension and persuasive communication.

### b. Objective:
The main objective of this project is to analyze customer behavior patterns in hotel reservations and their association with booking cancellation rates. By examining the dataset, we aim to identify trends, factors, and potential insights that contribute to booking cancellations, ultimately helping businesses make informed decisions.

## :pushpin: Exploratory Data Analysis
### a. Data Information
![Image 1. Data Information](1.png)




The dataset consists of 29 columns and 119,390 rows spanning the period from 2017 to 2019.

### b. Statistical Summary
![Image 2. Statistical Summary of Numerical Data Columns](2.png).




![Image 3. Statistical Summary of Categorical Data Columns](3.png).





## :pushpin: Data Preprocessing
### a. Handling Null Value
![Image 4. Null Value](4.png).




There are 4 columns with null values in the dataset:

- **Children** Column: Contains null values in 4 rows, which is 0.003% of the total data.
- **City** Column: Contains null values in 488 rows, which is 0.408% of the total data.
- **Agent** Column: Contains null values in 16,340 rows, which is 13.686% of the total data.
- **Company** Column: Contains null values in 112,593 rows, which is 94.307% of the total data.
  
To address these missing values, we can fill numerical columns (Children, Agent, Company) with the value 0, and fill the "City" column with the label "unknown".

### b. Handling Invalid Data
Invalid values are present in the "meal" column, specifically the value 'undefined'. This value will be replaced with 'No Meal' because 'undefined' cannot be interpreted as one of the meal types. Replacing it with 'No Meal' will make the data more consistent and avoid misinterpretations.

### c. Removing Uneccessary Value







