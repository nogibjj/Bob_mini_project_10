[![CI](https://github.com/BobZhang26/Bob_PythonTemplate1/actions/workflows/cicd.yml/badge.svg)](https://github.com/BobZhang26/Bob_PythonTemplate1/actions/workflows/cicd.yml)
## Mini Project 10: Student Stress Factor Analysis using PySpark 

### Summary
In this project, we are going to anayses student stress factors by using PySpark. PySpark is a powerful framework for distributed data processing and analysis. It provides a high-level API for working with big data, enabling parallel and distributed computing on large datasets. PySpark is built on top of Apache Spark, a fast and general-purpose cluster computing system. 
With PySpark, you can easily perform data transformations, aggregations, machine learning, and more, making it a valuable tool for data engineers
and data scientists working on large-scale data projects. Its ability to scale horizontally across clusters of machines makes it suitable for handling massive datasets and complex data processing tasks. PySpark also integrates seamlessly with popular data storage systems like Hadoop Distributed File System (HDFS) and cloud-based storage solutions.
In summary, PySpark is an essential tool in the big data ecosystem, enabling efficient data processing, analysis, and machine learning at scale.

For more information, please find it [here](https://spark.apache.org/docs/latest/api/python/index.html)

### Code Description
* Install ```PySpark``` in the notebook. Configure the Spark context in your Python script to interact with Spark.
```
!pip install pyspark
```
* Import ```PySpark```
```
import pyspark
```
* Satrt with a spark session. 
```
from pyspark.sql import SparkSession
spark = SparkSession.builder.appName('student').getOrCreate()
```
* EDA analysis
![output](https://github.com/nogibjj/Bob_mini_project_10/assets/141781876/bb05d407-19e1-46ae-b7c6-0bf03e6f1f6d)

* At the end, close the session
```
spark.stop()
```

### CI/CD Automation File


