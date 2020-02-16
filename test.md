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

All dimension are configurated as `DISTSTYLE ALL`. This allows to replicate the dimensions on all slices to speed up the joins with fact table.

## Fact table
1.  **songplays** - records in event data associated with song plays i.e. records with page `NextSong`
    -   _songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent_

This fact table is configured as `DISTKEY` over `user_id`. This is because this fact table is designed to support queries based on the user behavior or user preferences.

## ETL pipeline
1. For **songs**, **artist** dimension tables, the source is songs_data.
2. For **users**, **time** dimension tables, the source is log_data.
3. For **songplays** fact table, the sources are log_data and song_data.

The programs used for ETL pipeline are:
 - **sql_queries.py**: contains all SQL queries, create table statements and insert statements. This file is used in the next two programs.
 - **create_tables.py**: This program creates the data model tables.
 - **etl.py**: This program  processes song_data and log_data JSON files and load to data modelo tables.
 
## How to run
Follow the next steps:

1. Configure the  following connection parameters in the file dwh.cfg file:
   - HOST
   - DB_NAME
   - DB_USER
   - DB_PASSWORD
   - DB_PORT
   - DB_REGION='<*region*>'
   - ARN='aws_iam_role=<*arn*>'

1. Execute this command to create the database model:

       $ python create_tables.py

1. Execute this command to load the data:

       $ python etl.py

## Validation query

Execute the following query to validate:

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2Nzg5Nzk0ODQsNTM0NTk3Mjc5LC0yMD
YzMzAxMTU3LC04OTcyODU1MzYsMjA1NDczNzExOV19
-->