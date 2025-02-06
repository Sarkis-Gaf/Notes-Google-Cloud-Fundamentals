# Module 4

## Objectives:
1. Explore the different storage options
2. Learn to differentiate between structured and unstructured storage in the cloud
3. Examine how you can use Cloud Storage for unstructured data storage
4. Explore the use case for relational vs NoSQL storage options, and identify the options available with Google Cloud

--------------------------------------------------------------------------------------------------------------------------------------------------------------

## Storage options in the Google Cloud
Applications of course, need to store data

There are:
- Relationa Databases: Cloud SQL, Spanner
- Non-relational databases
- Worldwide object storage

For those with Databases Google has two priorities:
1. Migrate existing databases to the cloud, and move them to the right service
2. Innovate, build, or rebuild for the cloud

--------------------------------------------------------------------------------------------------------------------------------------------------------------

## Structured & Unstructured Data Storage

![Unstructured](https://i.imgur.com/5DB076r.png)

Then we have structured data, which is more simply, data that is organized with Tables, Rows, and Coloumns.
This fits more within relational databases, and is seen in stuff like spreadsheets. 

#### There are two types of Structured Data:
![Strcutured](https://i.imgur.com/LZKUJE3.png)

#### What about Unstructured Data?

Cloud Storage's common object storage use case:
- Online content
- Backup and Archiving
- Storage of intermediate results

##### What is Object Storage?

Is a computer data storage architecture that stores data as objects rather than files or folder, or chunks of a disk. 

There are 4 primary Cloud Storage classes:
1. Standard Storage: Hot data, data that is stored for brief periods at a time
2. Nearline Storage: Storing infrequent data, can be accessed once per month
3. Coldine Storage: Also stores infrequent data, can be accessed once every 90 days
4. Archive Storage: this is the lowest cost option, used ideally for data backup and disaster recovery, can be accessed once a year

Cloud Storage files are organized into buckets, with a unique name and geographic location. 
An ideal location for a bucket is where latency is minimized.

Now the thing is, Cloud Storage objects are immutable, you cannot directly edit them, instead you can create a new version of them.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

## SQL Managed Services

What is a database?
A database is an organized collection of information that can be easily accessed and managed. Computer applications run databases to get a fast answer to questions. 

Relational Databases are the most common database management systems

#### What is Cloud SQL

Offers fully manageable relational databases such as mySQL, PostreSQL, and SQL server. It mainly operates mundane, but necessary background tasks like managing backups and configuring replications. 

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Now what is Spanner?

Spanner is a fully managed relational databases that combines aspects of SQL & noSQL

#### Spanner is used for:
![Spanner](https://i.imgur.com/zxhosbg.png)

How does Spanner work?

Data is copied seamlessly throughout zones. It is basically replicated across other regions to ensure data can be available if one area falls short. 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Big Table as a NoSQL option

Bigtable handles massive workloads (ex. Gmail) and it has consistent low latency, and is an overall great choice for operational applications and analytical applications





