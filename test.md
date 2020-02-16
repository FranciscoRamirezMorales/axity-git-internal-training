# Cloud Data Warehouse Project

A music streaming startup, Sparkify, has grown their user base and song database and want to move their processes and data onto the cloud. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

As their data engineer, you are tasked with building an ETL pipeline that extracts their data from S3, stages them in Redshift, and transforms data into a set of dimensional tables for their analytics team to continue finding insights in what songs their users are listening to. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.

The purpose is to create a database model to store the data stored in JSON files. This data model is a star schema model that allows to Sparkify query the data in a efficient way.

# Project description

For this project was neccesary to create a data model for Postgres database and build an ETL pipeline using Python. 

### Data model

A star schema was created for song play analysis and queries.
* **Fact Table**: songplays: attributes referencing to the dimension tables.
* **Dimension Tables**: users, songs, artists and time table. 

## ETL pipeline
1. For **songs**, **artist** dimension tables, the source is songs_data.
2. For **users**, **time** dimension tables, the source is log_data.
3. For **songplays** fact table, the source is log_data . 

## Usage
1. **sql_queries.py**: contains all SQL queries, create table statements and insert statements. This file is used in multiple python files.
2. **create_tables.py**: execute this program to create the Postgres database, and star schema tables.
3. **etl.py**: execute this program to process song_data and log_data JSON files and load to star schema.

## Steps to create database and load JSON files data

   1. $ python3 create_tables.py
   2. $ python3 etl.py
   3. To test the results, execute 'test.ipynb'

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcwMjU5MTE3XX0=
-->