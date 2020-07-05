# Movies-ETL

### In this module, we used the Extract, Transform, Load (ETL) process to create data pipelines. A data pipeline moves data from a source to a destination, and the ETL process creates data pipelines that also transform the data along the way.

### We gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database. Since these JSON and CSV files are rather large, they won't be checked into github directory. 

#### "wikipedia.movies.json" https://courses.bootcampspot.com/courses/151/files/78740/download?wrap=1
#### "ratings.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download
#### "movies_metada.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download

### After extracting the data, an used an iterative process to merge, inspect and clean the source data. A few examples include:
#### List comprehensions to filter the data 
#### Functions to remove columns like "alternate langauage titles", and merge many redundant columns
#### Removed duplicate data
#### Parsed and converting the data and data types
#### Regular Expressions for converting "Box Office", "Budget", 'Release Date", "Running Time"
#### Merged data from two data frames using scatter plots to select the best source

### We then moved the data from Pandas into a PostgreSQL database "movies_data" and created "movies" Table and "ratings" Table.   
### URL Link: The Jupyter Notebook Python code for this ETL process is located in
https://github.com/daneshtavana/Movies-ETL/blob/master/Wikipedia-ETL.ipynb

# Challenge Problem

## Create a new automated ETL pipeline that operates on three data sources:
#### "wikipedia.movies.json" https://courses.bootcampspot.com/courses/151/files/78740/download?wrap=1
#### "ratings.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download
#### "movies_metada.csv" https://www.kaggle.com/rounakbanik/the-movies-dataset/download


## Use the same "def" function from "Wikipedia-ETL.ipyn" that performed all of the transformation steps, but removed any exploratory data analysis and redundant code.
### URL Link: The Jupyter Notebook Python code for the challenge ETL process is located in
https://github.com/daneshtavana/Movies-ETL/blob/master/challenge.ipynb
