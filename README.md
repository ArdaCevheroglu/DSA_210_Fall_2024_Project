# Analysis of Caffeine's Effects on Money Spending Trends

## Project Overview

This project aims to discover the relationship between caffeine consumption and spending habits. By analyzing my personal data that I collected over a specific time frame, I aim to discover patterns and trends that might indicate whether or not caffeine consumption has a significant impact on my spending behavior. The findings of this project could provide insights towards better financial management.

- Null Hypothesis: Caffeine intake does not influence spending trends

- Alternative Hypothesis: Caffeine intake positively influences spending trends

## Motivation

Caffeine is a part of my daily routine, I often consume it before studying, attending lectures and to kick start my day. However, I suspect that I tend to make more purchases, after drinking more coffee than I normally do on a daily basis. This project is an opportunity to explore whether caffeine genuinely affects my spending behavior or not.

## Dataset Description

The dataset for this project is entirely self collected. I extracted the coffee consumption data from Google Calendar through Google Takeout and downloaded my spending data from Akbank mobile app. My dataset consists of roughly 3 months (Between September 27th and December 18th) of caffeine consumption and money spending data.

## Data Analysis Steps

### Data Collection

#### Caffeine Consumption Data

Caffeine consumption data was extracted from Google Calendar mobile app using Google Takeout in .json format and contains:

* "due" date of tasks (which show the date and time of coffe consumed)

* "title" of tasks (which are represented with coffee emojis (each emoji corresponds to 1 heaping tablespoon of instant coffee))

* "kind", "id", "task_type", "selfLink" and "status" of tasks which won't be used in this project

Data was also logged to a simple spreadsheet for backup

#### Spending Data

Spending data was extracted from Akbank mobile app in .xlsx format and contains:

* Date range for transactions included

* Total amount of money in bank acount after each transaction and the final amount of money left in bank account (redundant for this project)

* Date in which transactions were made

* Amount of transactions

### Data Processing

#### Caffeine Consumption Data

* Redundant informations ("kind", "id", "task_type", "selfLink" and "status") were dropped

* Adjusted UTC time to local timezone (UTC+3 for Istanbul)

* Data was grouped by date and total caffeine consumed per day was calculated

Caffeine intake was calculated through weighing heaping tablespoon of instant coffee (3-4 grams) and multiplying it by USDA's calculation of caffeine in instant coffee (57mgs of caffeine per 1.8 grams of instant coffee) which gives us roughly 120mgs of caffeine per heaping tablespoon of instant coffee.

#### Spending Data

* Thousand separators and commas were replaced and "TL" was dropped from amounts (example: 1.000,99TL -> 1000.99)

* Converted amounts to numeric values

* Filtered out positive amounts (money received)

* Removed the instance of an 18k spending (since it was an outlier and reduced readability of graphs)

* Took absolute values of spending amounts

* Grouped data by date and calculated the total money spent per day

### Visualization

Correlations between caffeine intake and spending habits were visualized using heatmap, scatterplots, lineplots and boxplots.

I used the following graphs to visualize my findings:

* Lineplot to represent total caffeine consumption and money spent by date

* Barchart to show total and average caffeine consumption by time of day

* Scatterplot and Heatmap to visualize correlation between caffeine intake and spending trends

### Machine Learning Models

I built a linear regression model and used Scatterplot graphs to visualize my findings of actual vs predicted values for caffeine intake and spending trends in order to understand how they could look like in the future.

## Techniques and Tools

* Google Calendar, Google Takeout and Akbank mobile apps to obtain dataset

* Jupyter Notebook, Python, Pandas, NumPy and other libraries to parse and process the dataset

* Python, Matplotlib and Seaborn libraries for visualizing the dataset

* Scikit-learn library to create a linear regression model

* GitHub for hosting scripts and the project repository

* Microsoft Powerpoint to create a representation that summarizes my findings

## Findings

As shown in Heatmap, correlation between caffeine intake and money spent was 0.084 which indicates a low level of correlation. Thus, I didnt't have enough evidence to reject my Null Hypothesis and concluded that caffeine intake didn't have any significant effects on spending trends.

I saw that during this time period the amount of money i spent daily was mostly stable (as shown in lineplot and linear regression models) But towards the end of the semester the amount of caffeine i consumed daily went up significantly which might imply that deadlines could be a contributing factor.

I also found out that i generally drank my coffee between 8 a.m and 5 p.m but the amount in grams for a single dose didn't differ significantly regarding the time of day (as it can be seen from barcharts).

## Limitations

* Sample size: The project is limited to my personal data. Generalizing findings and conclusions would require more participants

* Data accuracy: Self-recorded caffeine consumption may have minor inconsistencies

* Confounding Variables: Other factors like mood, holidays, and deadlines could affect spending trends beyond caffeine's influence

## Future Work

The project can be improved to include more participants in the future since not everyone reacts to external stimuli like caffeine in the same way.

Techniques like restriction, matching, statistical control and randomization could be used to adjust the data for confounding variables.

Also a longer period of time to record more data could be useful in order to determine whether or not there is a correlation between caffeine intake and money spent more precisely.
