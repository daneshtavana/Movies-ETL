# Movies-ETL

### In this module, we used the Extract, Transform, Load (ETL) process to create data pipelines. A data pipeline moves data from a source to a destination, and the ETL process creates data pipelines that also transform the data along the way.

## We gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database. Since these JSON and CSV files are rather large, they won't be checked into github directory. 

### "wikipedia.movies.json" https://courses.bootcampspot.com/courses/151/files/78740/download?wrap=1
### "ratings.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download
### "movies_metada.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download

### After extracting the data, an used an iterative process to merge, inspect and clean the source data. A few examples include:
#### List comprehensions to filter the data 
#### Functions to remove columns like "alternate langauage titles", and merge many redundant columns
#### Removed duplicate data
#### Parsed and converting the data and data types
#### Regular Expressions for converting "Box Office", "Budget", 'Release Date", "Running Time"
#### Merged data from two data frames using scatter plots to select the best source

### We then moved the data from Pandas into a PostgreSQL database "movies_data" and created "movies" Table and "ratings" Table.   
### URL Link: The Jupyter Notebook Python code for this ETL process is located in
https://github.com/daneshtavana/Pewlett-Hackard-Analysis/blob/master/Data/final_retiring_emp_list.csv

# Challenge Problem

## Create two Technical Reports

### 1) The Number of Retiring Employees by Title -- A table showing number of tiles retiring, one showing number of employees with each title, and one showing a list of current employees born between Jan. 1, 1952 and Dec. 31, 1955.
Two intermediate TABLES were created FROM "current_emp"; 
the first TABLE "retiring_emp_titles" was the JOINED "current_emp" with "titles" and 
the second TABLE "retiring_emp_titles_salaries" was the JOINED "retiring_emp_titles" with "salaries" 
Finally, duplicates where removed after searching Google for a novel code to achive this. 
 
### URL Link: The SQL code and CSV file for obtaining the final list is located in 
https://github.com/daneshtavana/Pewlett-Hackard-Analysis/blob/master/Queries/queries_challenge.sql
https://github.com/daneshtavana/Pewlett-Hackard-Analysis/blob/master/Data/final_retiring_emp_list.csv

### 2) And employees who are eligible for the mentorship program 
