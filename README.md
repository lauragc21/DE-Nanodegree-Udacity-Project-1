# Data Engineering Nanodegree - Project 1: Data Modeliing with Postgres

## Introduction: 

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data. 

The purpose of this project is to create a Postgres database with tables designed to optimize queries on song play analysis. In order to achieve this, a databse schema and the necessary ETL pipeline were build.


## Database schema design and ETL pipeline:



## Explanation of the files:

This project contains six different files:

1. sql_queries.py
This file contains the sql code that will create the necessary tables, define their respective fields and datatypes, and insert the values into them.  

2. create_tables.py
This file contains a python script that reads the queries in the sql_queries.py file, creating the tables and inserting the data for our project. In case the tables already exist in our databse, the script will delete them before creating new ones. 



* How to run the Python scripts:



* Some example queries and results for song play analysis:



* TO DO: Add data quality checks to the test notebook

* TO DO: Put all the notes in the etl file (python script)