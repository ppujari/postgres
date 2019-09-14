# Project: Data Modeling with Postgres

## Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.
This project uses Postgres database. Here we create a database schema and ETL pipeline for this analysis. Write an ETL pipeline that transfers data from files in local directories into these tables in Postgres using Python and SQL.

## Summary
create_tables.py, This script successfully connects to the Sparkify database, drops any tables if they exist, and creates these tables again. This script has to be run at the beginning before running any other script. You can run these python script files from the terminal ( command prompt ) as python <file name>

sql_queries.py contains all sql queries for inserting data. This is imported in other scripts. This file should not be run from command line.

etl.py reads and processes files from song_data and log_data directories and loads them into tables. 

etl.ipynb reads and processes a single file from song_data and log_data and loads the data into respective tables. This notebook contains detailed instructions on the ETL process for each of the tables.

test.ipynb displays the first few rows of each table to confirm with the database. Run this file to confirm the creation of your tables with the correct columns. Make sure to click "Restart kernel" to close the connection to the database after running this notebook.You can run any notebook file with the following command:

jupyter notebook <file name>



