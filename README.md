Analysis of Caffeine's Effects on Money Spending Trends


Project Overview


This project aims to discover the relationship between caffeine consumption and spending habits. By analyzing my personal data that I collected over a specific time frame, I aim to discover patterns and trends that might indicate whether or not caffeine consumption has a significant impact on my spending behavior. The findings of this project could provide insights into behavioral economics and personal finance management.


Motivation


Caffeine is a part of my daily routine, and I often consume it before studying, attending lectures, or for every other possible reason there exists. However, I suspect that I tend to make more purchases, after drinking more coffee than I normally do on a daily basis. This project is an opportunity to explore whether caffeine genuinely affects my spending behavior and how this relationship can be explained.


Dataset Description


The dataset for this project will be entirely self collected. I will extract the necessary data from Google Calendar and Akbank mobile app. My dataset consists of roughly 3 months (Between September 27th and December 18th) of caffeine consumption and money spending data.

1. Caffeine Consumption Data

Caffeine intake: Amount of caffeine consumed throughout the day (in the form of milligrams) and the time of consumption.

Caffeine intake was calculated through weighing heaping tablespoon of instant coffee (3-4 grams) and multiplying it by USDA's calculation of caffeine in instant coffee (57mgs of caffeine per 1.8 grams of instant coffee)  

2. Spending Data

Money spent: Instances in which money was spent (in the format of date, time and amount) extracted from personal financial records


Data Analysis Plan


1. Data Collection

Caffeine consumption data will be extracted from Google Calendar mobile app in the form of tasks and logged to a simple spreadsheet for backup.

Spending data will be extracted from Akbank mobile app and also logged to a simple spreadsheet for backup.

2. Exploratory Data Analysis (EDA)

Clean and parse the dataset (handle missing data, check for outliers, scale variables etc.)

Perform EDA to identify trends and correlations (caffeine intake vs. spending trends).

3. Visualization

Visualize correlations between caffeine intake and spending habits using combined heatmap, scatterplots, lineplots and boxplots.

4. Machine Learning Models

Build a regression model to understand how caffeine intake influences spending trends.

Use clustering to group days with similar caffeine intakes and classify whether high spending days are caffeine influenced.

5. Reporting Findings and Presentation

Compile findings into a concise report.

Create a project slide in order to summarize the results.


Techniques and Tools


Data Collection: Tracking using apps and spreadsheets.

Data Analysis: Python with Pandas, NumPy and other libraries.

Visualization: Matplotlib, Seaborn and other libraries for interactive dashboards.

GitHub for hosting scripts and the project repository.


Findings


Although findings will emerge from the analysis, I look forward to discovering:

Whether caffeine consumption correlates with spending habits.

Possible time based patterns (morning coffee leading to higher amount of money spent during noon time etc.).


Limitations and Future Work


Limitations


Sample size: The project is limited to my personal data. Generalizing findings requires more participants.

Data accuracy: Self reported and app recorded caffeine consumption may have inconsistencies.

Confounding Variables: Other factors like mood, holidays, and deadlines could affect spending beyond caffeine's influence.


Future Work


Suggest improvements, like expanding the study  to include more participants in the future since not everyone reacts to external stimuli like caffeine in the same way.


Github Repository Structure

README.md      ---> Project overview and details

data           ---> Processed datasets (no raw data for privacy reasons)

scripts        --->  Python scripts for data processing and analysis

visualizations --->  Plots and dashboards

slide presentation
