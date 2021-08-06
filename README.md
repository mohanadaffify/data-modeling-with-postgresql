# Project 1: Data modeling with Postgres

This **Udacity Data Engineering nanodegree** project creates a postgres database `sparkifydb` for a music app, *Sparkify*. The purpose of the database is to model song and log datasets (originaly stored in JSON format) with a star schema optimised for queries on song play analysis.

## Schema design and ETL pipeline

The star schema has 1 *fact* table (songplays), and 4 *dimension* tables (users, songs, artists, time)..

![](Untitled_Workspace.png?raw=true)

## the creation process is as follows : 

### sql_queries.py: 
<br /> 
used to create and drop  the fact and dimension tables 
<br /> 
#### etl.ipynb:
firstly sql_queries.py file is imported
<br /> 
secondly a connection to database is established 
<br /> 
thirdly we get the raw files that will be processes as raw entries for the database 
<br /> 
then we peocess the log and data files and insert them in the corresponding tables of the database 
<br /> 
### create_tables.py:
<br /> 
establish the connection with the database 
<br /> 
execute the queries in te sql_queries.py 
<br /> 
### etl.py :
<br /> 
auto create data pipelines.
