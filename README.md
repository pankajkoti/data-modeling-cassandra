# Data-modeling-cassandra

## Project Overview
In this project, we apply data modeling with Apache Cassandra and complete an ETL pipeline using 
Python Jupyter Notebook. To complete the project, we modelled our data by creating tables in Apache Cassandra 
to run queries. The ETL pipeline transfers data from a set of CSV files within a directory to create a 
streamlined CSV file to model and insert data into Apache Cassandra tables.


## Datasets
For this project, we work with one dataset: 'event_data' which is a directory of CSV files 
partitioned by date. Here are examples of filepaths to two files in the dataset:

```
    event_data/2018-11-08-events.csv
    event_data/2018-11-09-events.csv
```

## Project Steps

- We create a cleaned smaller single file 'event_datafile_new.csv' by working on files
with 'event_data' directory to create a denormalized dataset
- We mode the the data tables keeping in mind the queries we need to run. Remember,
in NoSQL we model our tables based on the queries we need to run
- We load data from the above csv file in these modeled data tables
- And finally test by running SELECT queries on these tables to see we get inserted data as expected