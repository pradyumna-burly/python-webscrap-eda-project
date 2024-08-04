# Web Scraping + EDA using Python

## Project Overview

This project involves web scraping the NHL hockey database from 1990-2011 using BeautifulSoup, followed by an exploratory data analysis (EDA) to uncover patterns and trends in the dataset. The goal is to provide insights into the performance metrics of various teams over the years.

## Introduction

The objective of this project is to scrape NHL hockey data spanning from 1990 to 2011 and perform an exploratory data analysis to identify key trends and patterns. This analysis is particularly focused on the changes in team performance metrics such as wins, losses, goals scored, and goals conceded over time.

## Data Collection

### Web Scraping

Data was scraped from the NHL database using the BeautifulSoup library. The following information was collected for each team:
- **Team Name**
- **Year**
- **Wins**
- **Losses**
- **Overtime Losses (OT Losses)**
- **Goals For**
- **Goals Against**
- **Goal Difference**

### Handling Missing Data

The 'OT Losses' column contains null values for years when this metric was not recorded. Imputation or exclusion was applied as necessary during the analysis.

## Exploratory Data Analysis (EDA)

The EDA process involved several steps:
1. **Data Cleaning and Preprocessing**: Correcting data types, handling missing values, and preparing the data for analysis.
2. **Descriptive Statistics**: Generating summary statistics for the dataset.
3. **Data Visualization**: Using matplotlib to create visualizations that reveal trends and distributions in the data.

### Key Insights

- **Trends in Wins and Losses**: Analysis showed fluctuations in team performance, with notable increases or stagnation in wins.
- **Goals Analysis**: Evaluation of goals scored and conceded, with insights into offensive and defensive strengths of teams.

## Feature Engineering

New features were derived to enhance the analysis:
- **Win Ratio**: Calculated as Wins / (Wins + Losses + OT Losses).
- **Goals Per Game**: Calculated as Goals For / Total Games.
- **Goals Against Per Game**: Calculated as Goals Against / Total Games.

## Hypothesis Testing

Hypothesis tests were conducted to compare the average number of wins across different time periods. For example, a t-test was used to assess whether there was a significant difference in wins before and after a key rule change year.

## Technologies Used

- **Python**: Primary language for the project.
- **BeautifulSoup**: For web scraping.
- **pandas**: For data manipulation and analysis.
- **matplotlib**: For data visualization.
- **scipy**: For statistical analysis and hypothesis testing.

## Installation

To set up the environment and install the necessary packages, run:

```bash
pip install -r requirements.txt

