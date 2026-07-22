Netflix Data Analysis (EDA)
Synent Technologies Data Science Internship — Task 3



README

Problem Statement
Netflix has thousands of movies and TV shows in its catalog, but raw data on its own doesn't say much. This project digs into the Netflix titles dataset to figure out what kind of content dominates the platform, where most of it comes from and how the catalog has grown over the years.

Dataset
Source: Kaggle, Netflix Movies and TV Shows dataset (netflix_titles.csv). Around 8800 rows before cleaning with columns for title, type, country, genre, release year, date added, rating and duration.

Approach
•	Loaded the dataset and checked for missing values, duplicates and wrong data types

•	Filled missing director, cast and country values with "Unknown" instead of dropping them, since dropping would have wiped out a big chunk of the data
•	Dropped a small number of rows where rating or duration were missing, since those were only a handful of rows and didn't cost much
•	Converted date_added to a proper datetime format, which needed stripping extra whitespace first because some entries had a stray leading space before the month
•	Ran value counts and built bar charts to look for patterns in type, genre, country and year added

Results (Summary)
•	Movies make up close to 70% of the catalog (6126 movies vs 2664 TV shows)

•	International Movies, Dramas and Comedies are the three most common genres by a clear margin

•	The US leads content production by far, followed by India and the UK

•	Content additions were almost flat before 2015, took off from 2017, peaked in 2019 at over 2000 titles and dipped slightly in 2020-2021, likely tied to COVID-related production delays

Tools Used
Python, Pandas, Matplotlib, Seaborn built and run in Google Colab.
 

