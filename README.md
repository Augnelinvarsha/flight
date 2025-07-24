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






