# Data Engineering Nanodegree - Project 1: Data Modeliing with Postgres

## Introduction:

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

The purpose of this project is to extract, transform and load the data from the JSON files mentioned above, creating a Postgres database with tables designed to optimize queries on song play analysis. In order to achieve this, a database schema and the necessary ETL pipeline were build.


## Database schema design and ETL pipeline:



## Explanation of the files:

This project contains six different files:

1. sql_queries.py - 
This file contains the necessary sql code to create the Sparkify tables, define their respective fields, datatypes, characteristics and primary keys, and to insert values into them.  

2. create_tables.py - 
This file contains a python script that reads the queries in the sql_queries.py file, creating the tables and their respective fields with the defined datatypes, characteristics and primary keys. In case the tables already exist in the database, the script will delete them before creating new ones.

3. etl.py - 
This file contains a python script that reads, processes and loads the JSON user logs and songs metadata files into the created tables mentioned in the create_tables.py file. To insert the values, this script reads the sql queries for insertion defined in the sql_queries.py file.

4. etl.ipynb - 
This notebook explains each step of the process used in the etl.py script, using a single file from each (user logs and songs metadata files) as an example.

5. test.ipynb - 
This notebook allows users to displays the first rows of each table in order to check them. It also contains sanity checks for the database that test column data types, primary key constraints and not-null constraints as well look for on-conflict clauses wherever required.


* **How to run the Python scripts:** In order to create the database, the user needs firstly to run the **sql_queries.py** file, which will define the sql queries for table creation and data insertion. Secondly, the user needs to run the **create_tables.py** file, which will read the queries file and create the necessary tables. After running this file, the user can finally run the **etl.py** file, which will populate the newly created tables. 

Attention - if for some reason the user feels the need to delete the tables and run the process again, the **create_tables.py** file will delete the existing tables before creating new ones.
