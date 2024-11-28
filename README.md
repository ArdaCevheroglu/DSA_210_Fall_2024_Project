Analysis of Caffeine's Effects on Mood and Anxiety

Project Overview

This project aims to explore the relationship between caffeine consumption, mood, and anxiety levels using validated scales like the GAD-7 for anxiety and PANAS for mood. Caffeine is a widely consumed psychoactive substance, but its impact on mental health can vary significantly from person to person. By collecting my own data and performing exploratory data analysis (EDA), visualization, and machine learning, this project seeks to uncover patterns and provide insights into how caffeine affects mood and anxiety.
Motivation
As a university student, caffeine plays a significant role in my daily routine, especially during exam and homework deadlines. While it helps me stay awake and focused, I've often wondered how it actually influenced my mood and anxiety levels. This project offers an opportunity to use data science techniques to investigate these effects and hopefully come to a conclusion.

Dataset Description

The dataset for this project will be entirely self-collected. Over the next four weeks, I will log the following metrics daily:

Caffeine intake: Total amount consumed throughout the day (in the form of milligrams)

Date/Time: When the caffeine was consumed.

Mood Rating: Subjective rating on a scale of 1-10 (using PANAS).

Anxiety Levels: Subjective rating on a scale of 1-10 (using GAD-7).

Other factors: Significant events that might affect results (e.g. exam / homework deadlines and other day to day problems).
Data will be recorded using a combination of a mobile app and a simple spreadsheet for backup.

Project Plan
1. Data Collection

Manually log caffeine intake, mood, and anxiety levels daily.
Ensure data privacy by storing the data locally and sharing only the analysis scripts on GitHub.

2. Exploratory Data Analysis (EDA)

Clean and preprocess the dataset.
Perform EDA to identify trends and correlations (e.g. caffeine intake vs. mood, caffeine intake vs. anxiety).
Visualize data using plots and dashboards (e.g. line charts, scatter plots).

3. Machine Learning Models

Build a regression model to predict mood or anxiety levels based on caffeine intake and other features.
Use clustering to group days with similar caffeine-related behaviors.

4. Reporting Findings and Presentation

Compile findings into a concise report.
Create a project website or video summarizing results.
Prepare materials for peer evaluation and feedback.

Techniques and Tools

Data Collection: Manual tracking using apps and spreadsheets.
Data Analysis: Python with Pandas, NumPy and other libraries.
Visualization: Matplotlib, Seaborn, and other libraries for interactive dashboards.
Collaboration and Version Control: GitHub for hosting scripts and the project repository.

Findings

Although findings will emerge from the analysis, I anticipate discovering:
Patterns in how caffeine affects my mood and anxiety across different times of day.
Relationships between caffeine intake and it’s effects on mood and anxiety.


Github Repository Structure

README.md          # Project overview and details

data/              # Processed datasets (no raw data for privacy)

scripts/           # Python scripts for data processing and
analysis

visualizations/    # Output plots and dashboards

Limitations and Future Work

Limitations

Subjectivity: Mood and anxiety ratings are self-reported and may be influenced by potential biases.

Limited Time: The dataset spans a few weeks, which might not reflect long-term trends.

Confounding Variables: Other factors (e.g., diet, hydration, exercise) that affect mood and anxiety may not be accounted for.

Future Work

Suggest improvements, like using wearable devices for data collection (e.g. using heart rate trackers).

Suggest expanding the study  to include more participants in the future.
