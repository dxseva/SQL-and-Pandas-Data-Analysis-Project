# SQL-and-Pandas-Data-Analysis-Project
A data analysis project that uses SQL and Pandas to analyze user behavior on an educational platform. The goal is to find out if adding a newsfeed feature makes students start their assignments earlier.

What This Project Does
I analyzed real data from an educational platform to test whether showing students their peers' activity would change their behavior. The platform added a newsfeed page where students could see when others submitted assignments. My job was to figure out if this actually made students start working sooner.
The data comes from SQLite database tables that track when students check assignments and when they visit different pages on the platform.

Files Description
src/ex00/ex00_first_select.ipynb
Basic SQL queries and data filtering. Connects to the database, looks at table structure, and pulls specific data based on user types and time periods.
src/ex01/ex01_subquery.ipynb
Uses nested SQL queries to count records across multiple tables. Filters data based on assignment status, attempt numbers, and specific lab names.
src/ex02/ex02_joins.ipynb
Combines data from different tables using JOIN operations. Creates test and control groups for A/B testing and handles missing data.
src/ex03/ex03_aggs.ipynb
Calculates statistics like minimum, maximum, and average time differences between assignment submissions and deadlines. Tests correlations between page visits and work timing.
src/ex04/ex04_ab-test.ipynb
Runs the A/B test analysis. Compares user behavior before and after the newsfeed launch to see if it actually changed when students start their work.

Technical Features

SQL Techniques

Subqueries: Queries inside other queries for complex filtering
JOIN Operations: Combining data from multiple tables
Date/Time Calculations: Finding time differences in hours between events
Aggregation Functions: GROUP BY operations for statistical summaries

Python Integration

SQLite3: Direct database connections using Python's sqlite3 module
Pandas SQL: pandas.io.sql.read_sql for converting database results to DataFrames
Statistical Analysis: pandas.DataFrame.corr() for correlation calculations

Analysis Methods

A/B Testing: Split users into test and control groups
Missing Data Handling: Replace missing values with group averages
Outlier Filtering: Remove data points that skew results

Libraries Used
Core Tools

Pandas: Data manipulation and analysis
SQLite3: Database management
Jupyter Notebook: Interactive coding environment

Analysis Tools

Correlation Analysis: Measure relationships between variables
DateTime Processing: Handle dates and times in both SQL and Python
Statistical Functions: Calculate means, mins, maxes across groups

Project Structure 
```
├── src/
│   ├── ex00/
│   ├── ex01/
│   ├── ex02/
│   ├── ex03/
│   ├── ex04/
│   └── data/
└── README.md
```
What's in Each Directory

src/: All the code and analysis notebooks.
src/data/: The SQLite database file and any data files created during analysis.
src/ex##/: Each exercise folder contains one Jupyter notebook that builds on the previous one.

Results

The project shows how to use SQL and Python together for real data analysis. It covers everything from basic database queries to running statistical tests on user behavior. The A/B test format mimics what you'd do in a real company to measure if a new feature actually works.
