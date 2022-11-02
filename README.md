# Apache Cassandra Data Modeling
## Objectives

In this project, the main objective is to create a simple non relational data model using Python and Apache Cassandra (NoSQL database) to simulate a real project at Sparkify, some music streaming startup. Sparkify team wants to analyze the data they've been collecting on songs and user activity on their new music streaming application, but since they don't have a database and all data are available only in csv files generated by the app, we are going to use CQL (Cassandra Query Language) to optmize this process.
## How to run ETL

First of all, you must have [Python](https://www.python.org/downloads/) and [Apache Cassandra](https://cassandra.apache.org/_/index.html) installed in your machine. You can find instructions [here](https://cassandra.apache.org/_/download.html). 
The others Python packages can be installed running the command below:

``` pip install -r requirements.txt ```

After that, you can run ```ELT.ipynb``` to extract data from csv files, create keyspace and tables and insert data to our model.
## CSV files

In event_data folder we have the application logs in CSV files, registering events sent by users regarding the listened musics and other information about themselves.

## Modeling

In order to pull especific data from CSV files respecting Cassandra's arquitechture and functionalities, we've created three different tables. Below you can check the model with Chebotko diagram.
![Entity Relationship Diagram (4)](https://user-images.githubusercontent.com/49285727/199594184-c23db27c-8c5c-484b-aede-003cbc8dd1f0.jpg)
