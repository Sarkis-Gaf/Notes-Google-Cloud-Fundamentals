# Computing Foundations in Data Mining, Machine Learning, & Big Data w/ Google Cloud

## Introduction to big data managed services in the cloud

#### Here is how big data is stored/managed
- Dataproc: processes big data with Hadoop/Spark
- Dataflow: Analyze streaming data in real-time
- BigQuery: Modernize a data warehouse foundation

---------------------------------------------------------------------------------------------------------------

## Leveraging big data operations with Dataproc
Dataproc is a managed service for Spark and Hadoop, which are open-source data processing software.
Dataproc allows you to create clusters easily, it is cost-effective, fast, and scalable, and it has an open-source ecosystem

Lets see its use case in ML:
Let's say that someone is using Spark machine learning libraries (Mlib) and are using it to run classification algorithms on large datasets

You can install Spark & MLib on any dataproc cluster and you can use cloud monitoring to monitor workflows

----------------------------------------------------------------------------------------------------------------

## Build extract, transform, and load pipelines using dataflow

![Pipeline](https://i.imgur.com/0ZiBDM7.png)

Here you can see how Dataflow works

Here are some questions to ask yourself during pipeline design:
1. Will the pipeline code be compatible with both batch and streaming data, or will it need to be refactored?
2. Will the pipeline code SDK have all the necessary transformations and windowing?
3. Will the SDK be able to handle late data?

