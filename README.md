# Project 1: Data modeling with Postgres

This **Udacity Data Engineering nanodegree** project creates a postgres database `sparkifydb` for a music app, *Sparkify*. The purpose of the database is to model song and log datasets (originaly stored in JSON format) with a star schema optimised for queries on song play analysis.

## Schema design and ETL pipeline

The star schema has 1 *fact* table (songplays), and 4 *dimension* tables (users, songs, artists, time)..

![schema] (untitled Workspace.png)

## the creation process is as follows : 

**sql_queries.py**: 
used to create and drop  the fact and dimension tables 
**etl.ipynb**:
firstly sql_queries.py file is imported
secondly a connection to database is established 
thirdly we get the raw files that will be processes as raw entries for the database 
then we peocess the log and data files and insert them in the corresponding tables of the database 
**create_tables.py**:
establish the connection with the database 
execute the queries in te sql_queries.py 
**etl.py** :
auto create data pipelines.
