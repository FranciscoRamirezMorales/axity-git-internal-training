# Cloud Data Warehouse Project

A music streaming startup, Sparkify, has grown their user base and song database and want to move their processes and data onto the cloud. Their data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

The purpose for this project is:

 - Create a database model to store the data stored in JSON files.
 - Built the ETL pipeline for:
   -  extract data form S3 and load to stage tables
   - load to dimensional model from stage tables

## Data sources
The data resides in JSON  files on Amazon S3:
-   Song data: `s3://udacity-dend/song_data`
-   Log data: `s3://udacity-dend/log_data`

For log data structucture the definition resides here:
 - Log data json path: `s3://udacity-dend/log_json_path.json`

## Data model
### Stage tables
1.  **staging_songs** - stores the data from `song_data` JSON files
2.  **staging_events** -  stores the data from `log_data` JSON files

### Dimension Tables

1.  **users** - users in the app
    -   _user_id, first_name, last_name, gender, level_
1.  **songs** - songs in music database
    -   _song_id, title, artist_id, year, duration_
1.  **artists** - artists in music database
    -   _artist_id, name, location, lattitude, longitude_
1.  **time** - timestamps of records in **songplays** broken down into specific units
    -   _start_time, hour, day, week, month, year, weekday

## Fact table
1.  **songplays** - records in event data associated with song plays i.e. records with page `NextSong`
    -   _songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent_

## ETL pipeline
1. For **songs**, **artist** dimension tables, the source is songs_data.
2. For **users**, **time** dimension tables, the source is log_data.
3. For **songplays** fact table, the sources are log_data and song_data. 



Log data json path: `s3://udacity-dend/log_json_path.json`
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

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
eyJoaXN0b3J5IjpbMTAzNTg4ODMwN119
-->