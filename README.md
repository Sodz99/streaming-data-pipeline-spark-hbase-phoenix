# Streaming Data Pipeline using Spark, HBase and Phoenix

To build an application that monitors oil wells.

## Overview
Sensor networks clearly focus on a wide range of practice-oriented research as individual sensors and related networks for structural monitoring and highly efficient monitoring. The sensor network is designed to respond to emergencies in real-time while observing the radiation field. An intelligent system-based sensor network is presented and used to monitor the condition of remote wells. The network consists of three sensors used to collect oil field data, including temperature, pressure, and gas. Intelligent microprocessor sensors are generally designed for oil well data processing, critical failure alarms or signals, traditional data storage or signals, and data/status connections.

## Approach
- Create an AWS EC2 instance and launch it.
- Create docker images using docker-compose file on EC2 machine via ssh.
- Download the dataset and load it into HDFS storage.
- Read data from HDFS storage and write into HBase table using Spark.
- Create Phoenix view on top of HBase table to analyze data using SQL queries.

## Tech stack
- AWS EC2
- Docker
- Scala
- HBase
- Apache Spark SQL
- Spark Structured Streaming
- HDFS
- Apache Phoenix
- SBT

## How to run
Notebooks: [`presentation.ipynb`](Installation%20and%20Execution/presentation.ipynb)

## Project structure
```
.gitignore
Code/
  airflow_init.sh
  docker-compose.yml
  portforwarding.bat
  src/
    GCOil.scala
    GCOil_Batch.scala
Installation and Execution/
  presentation.ipynb
README.md
```

## Credits
Based on a ProjectPro guided project.
