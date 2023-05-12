# Project-Data-Pipeline-for-Recruitment-Start-Up

## Introduction
This project is to build a near real-time ETL pipeline for a recruitment company to calculate the total number of clicks, candidates applying, and the qualified and unqualified people for jobs on the recruitment website by combining programming language and frameworks like Python, Apache Spark (PySpark, SparkSQL), Docker.
<br>
![test (1)](https://github.com/DuyDoan233/Project-Data-Pipeline-for-Recruitment-Start-Up-/assets/101572443/d9656f3f-5c8e-44b7-973c-972b5e8d6771)

## Dataset
Since it mainly focuses on building the ETL pipeline so the dataset used for processing is faked from the customer's schema.
- [CassandraDB (DataLake)]()
- [MySQLDB (Data Warehouse)]()

## Process description
- Fake Data process
  - Since this project only received schema and a limited amount of data from the customer, in order to increase the size of the data to test ETL scripts as well as simulate the process of a near real-time ETL pipeline, I built a Python script ([Fake_data_process.py](##)) to fake randomly generate from 1 to 10 records after 'Time = Script running time + 5s sleep'.
- ETL process
  - 

## Requirements
- Since it simulates an actual project, so we use some programming\tools\framework such as:
  - Python: Use to build the Fake_data_process.py script to combine with ETL pipeline to simulate the near real-time process.
  - Apache Spark: Framework to build the ETL script (Including PySpark & SparkSQL)
  - Docker: Install Cassandra(as DataLake), MySQL(as Data Warehouse).
    - Cassandra: raw data would store in a keyspace named 'datalake'.
    - MySQL: processed data would store in the database named 'DW', the shorten of Data Warehouse. 
&#8594; All the above requirements are packaged inside Dockerfile and Docker-compose.yaml.

  ### Dockerfile & Docker-compose detail
