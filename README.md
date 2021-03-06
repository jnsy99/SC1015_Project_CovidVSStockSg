
# Finding correlation between Singapore Covid-19 cases and Stock market prices in Singapore and predicting future stock prices 

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on stock prices and covid-19 data in Singapore by Team 3 from SC9. Please read the README.txt file first!


## Contributors
- Jaren Ng Shing Yu - Problem formulation, Data Analysis, Data Visualisation, Linear Regression
- Lee Zheng Xuan - Data Extraction, LSTM, Linear Regression, Data Cleaning
- Joel Tham Yew Hng - LSTM, Dataset Research, Model Evaluation

 ## Contents of Codebase
1. Presentation Video (SC9_Team03.mp4) *Please note video is not on github
2. Project code (SC9_Team03.ipynb)
3. Presentation PowerPoint slides (Presentation Slides ───> SC9_Team03.pdf)
4. Datasets (Datasets ───> PublicHols2020-2022.xlsx)
		    │    
                    └────> covid19_sg.csv )


Thank you and hope you enjoy our project as much as we do!


## Problem Statement
We aim to find out the correlation between various stock prices and the Covid-19 situation in Singapore, allowing us to predict future stock prices of selected industries. We hope to use machine learning models and selecting the most suitable model to predict future industries’ stock prices more accurately using Covid-19 as a variable.

## Machine Learning Models Used
1. Linear Regression
2. Long Short-Term Memory Network Model

## Conclusion
- None of the stocks selected worked with Covid-19 for the linear regression model since the explained variance is close to zero or negative. The MSE is also too large for test datasets
- Linear Regression Model might not be optimal for time-series dataset 
- Thus, to predict these stocks, we need to consider other facts and think of it as a multivariate problem
- We can look for other stocks to find a relation between them with Covid-19 cases
- Lastly, we can also look for other Machine Learning models like LSTM to predict stock prices as seen previously as it is suitable for time series datasets. 

## What did we learn from this project?
- An API allows the user to collect real time data that is updated regularly, depending on the data provider
- How to extract data using API to retrieve real time data
- How using pd.to_datetime().date() allows appropriate date format to be used
- Understanding the data we are extracting from e.g. Stock Market closes on weekends and public holidays. Thus, removal of corresponding data for proper alignment is     necessary
- Plotting of 2 times series data with different units on the same graph
- Learning new machine learning model like LSTM which uses RNN

## Possible Improvements
- Include covid cases for weekends and holidays
  - These cases may increase and affect stock prices
- Explore other factors that can cause stocks prices to change
  - For example, political unrest, improvement of technology, speculation, brand reputation, etc.
