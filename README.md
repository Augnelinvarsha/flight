# flight
Flight Fare Analysis Project:
This project performs exploratory data analysis (EDA) on a large dataset of Indian domestic flights. It uses Python libraries such as Pandas, Seaborn, and Matplotlib to uncover patterns in flight pricing based on various factors like airline, class, route, stops, and booking days in advance.

📌 Project Motivation
Flight ticket prices vary significantly based on when you book, which airline you choose, your source/destination, number of stops, and class (Economy or Business). This project aims to:

Understand what drives flight ticket prices

Explore trends between booking time and price

Identify airline and route pricing strategies

Create helpful visualizations for business and consumers

Dataset Overview:

File: Clean_Dataset.csv

Features:
Column Name	Description
airline	Airline operating the flight
flight	Flight number
source_city	Departure city
departure_time	Time of departure (e.g., Morning, Evening)
stops	Number of stops (e.g., zero, one)
arrival_time	Time of arrival (e.g., Night, Afternoon)
destination_city	Arrival city
class	Class of travel (Economy or Business)
duration	Duration of the flight in hours
days_left	Number of days left until the flight (from booking date)
price	Ticket price (INR)

Note: The column Unnamed: 0 was dropped as it served no analytical purpose.

🛠️ Requirements
Python 3.7+

pandas

seaborn

matplotlib

jupyter (optional, for notebook-based analysis)

You can install dependencies via:

bash
Copy
Edit
pip install pandas seaborn matplotlib

📊 Key Analyses & Visualizations
Flight Counts by Airline

Price Distributions across Airlines

Top 10 Most Frequent Routes

Flight Duration vs Stops

Price Trends by days_left and Class

📈 Insights You Can Extract
How much does booking earlier reduce flight prices?

Which airline offers the cheapest flights on average?

Do business class prices follow a different trend over time?

What are the busiest city pairs?
📊 Analyses Performed
Here are some of the main insights and visualizations developed in this project:

✈️ Flight-Level Insights
Distribution of flights by airline

Most frequent routes (top source-destination city pairs)

Flight durations vs. number of stops

Comparison of departure and arrival times

💰 Pricing Analysis
Price distribution by airline

Price comparison by travel class

Average prices vs. days_left

Do Business class tickets follow different booking trends?

📈 Trend Visualization
How price changes as the departure date approaches

Price trends for specific airlines or routes

Impact of number of stops on ticket price


models used:

*Linear Regression

*gradient boosting

*knn regressor

*ridge regression

*decision tree regressor

1.  Linear Regression
 Overview:
Linear Regression assumes a linear relationship between the input features and the target variable. It tries to fit a straight line that minimizes the difference (error) between predicted and actual prices.

 Use Case:
Simple, interpretable model—useful when features have a linear correlation with price, such as duration or days_left.

 Pros:
Easy to implement and interpret

Fast training time

Good baseline model

2.  Decision Tree Regressor
 Overview:
A decision tree splits the data into branches using conditions on feature values to predict the target value. It learns decision rules based on data patterns.

 Use Case:
Works well when you have categorical features like airline, stops, or class, and the relationships are not linear.

 Pros:
Captures nonlinear patterns

Easy to visualize

Handles categorical and numerical data

3.  Gradient Boosting Regressor (GBR)
 Overview:
Gradient Boosting builds an ensemble of weak learners (typically trees) in sequence. Each new model learns from the errors of the previous model.

Use Case:
Powerful model for structured/tabular data, especially when you're optimizing for performance.

Pros:
High prediction accuracy

Handles nonlinear relationships

Robust to outliers and noise

4.  K-Nearest Neighbors (KNN) Regressor
 Overview:
KNN predicts a value by averaging the target values of the k closest neighbors in the feature space. It is a non-parametric, instance-based algorithm.

 Use Case:
Best when the dataset is small to medium and the relationships are localized (e.g., similar duration and days_left may have similar prices).

 Pros:
Simple and intuitive

No training phase

Works well when similar observations have similar outcomes

5.  Ridge Regression
 Overview:
Ridge Regression is a regularized version of Linear Regression that adds a penalty term to shrink coefficients and reduce overfitting.

 Use Case:
When your linear model is overfitting or when there is multicollinearity (correlated features).

 Pros:
Handles multicollinearity

Less overfitting than plain Linear Regression

Easy to implement and scale






