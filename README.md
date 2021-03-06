# Big_Data

## Big Data vs Data Science
|     |                                      |                        |
| --- | ------------------------------------ | ---------------------- |
| 1.  | Collection, processing and analyzing | Extracting Information |
| 2.  | Hadoop Spark Flunk                   | Python,R,SAS           |

How big is **Big Data**?
> 1 Zettabytes = 10^10 bytes and
> In 2016 we reached 1 zettabyte.
> Speed is measured in term of FLOPS Floating Point operations per second, it is basically number of multilication and divsion we can do per sec.
> Max 122.3 FLOPS by IBM in 2018.

#### Types of Big Data

1. Structured Data
   eg. PostgreSQL
2. Semi Structured Data
   eg. JSON
3. Unstructured Data
 eg. Email,Image,Audio,Video

#### Ways in which Unstructured data can be handled

1. Data mining
2. Text mining
3. NLP
4. Noisy text analytics

### Challenges of Big Data

1. Storing exponentially growing huge datasets
2. Processing Data having complex structure
3. Processing Data Faster
   
### Solving Challenges

1. Storing : Horizontal vs Verticl Scaling
2. Pre-processing : Hive, Pig
3. Faster Comparision

| Horizontal                                         | Vertical                                                      |
| -------------------------------------------------- | ------------------------------------------------------------- |
| scale out                                          | scale in                                                      |
| multiple OS instance                               | single OS instance                                            |
| scale out as much as needed                        |                                                               |
| Less financial investment                          |                                                               |
| has to handle distribution and parellel processing |                                                               |
|                                                    | It is not possible to scale up vertically after certain limit |

### V's of Data Science

1. .
2. .
3. Volume, Velocity and Variety
4. " and Veracity
5. " and Value
6. " and Visiblity

> Veracity : Uncertainty and inconsistemcies in data (Min, Max, Mean, SD)

> Value : mechanisim to bring correct meaning out of the data

> Visiblity : 

## Comparision 

| charecteristics        | High                | Low         |
| ---------------------- | ------------------- | ----------- |
| Scaliblity             | P2P                 | FPGA        |
| Spark is               | more scalable       | than Hadoop |
| I/O                    | FPGA                | P2P         |
| HPC has                | greater I/O than    | Spark       |
| Fault tolerant         | FPGA (HPC == Spark) | P2P         |
| Real Time Processing   | FPGA (HPC < Spark)  | P2P         |
| Data Size              | P2P (equal)         | FPGA        |
| Iterative task support | P2P (HPC>Spark)     | FPGA, GPU   |

## YARN
Yet Another Resource Negotiater
1. Client
2. Resource Manager
3. Node Manager
4. Application Master 
5. Container

### Resource Manager

1. Scheduler : It is a pure scheduler, means it does not perform other
tasks such as monitoring or tracking and does not guarantee a restart if a
task fails.
2. Application manager : It is responsible for accepting the application and
negotiating the first container from the resource manager. It also restarts the
Application Manager container if a task fails.

>Capacity Scheduler :-  Here a separate dedicated queue allows the small job to start as soon
as it is submitted, although this is at the cost of overall cluster
utilization since the queue capacity is reserved for jobs in that queue.
This means that the large job finishes later than when using the FIFO
Scheduler

> Fair  Scheduler :- Here there is no need to reserve a set amount of capacity, since it will
dynamically balance resources between all running jobs. Just after the
first (large) job starts, it is the only job running, so it gets all the
resources in the cluster

## Hadoop

### HDFS
1. [Architecture](https://www.youtube.com/watch?v=m9v9lky3zcE&t=2310s)
2. [HDFS Commands](https://www.geeksforgeeks.org/hdfs-commands/)
3. [How to change replication factor and data size of block?](https://princetonits.com/blog/technology/how-to-configure-replication-factor-and-block-size-for-hdfs/)
4. [Impact of change replication factor and default size of block](https://www.datacenterknowledge.com/archives/2016/05/04/impact-block-sizes-data-center)
5. [Data locality](https://data-flair.training/blogs/data-locality-in-hadoop-mapreduce/)
6. [Job Tracker and Task tracker](https://www.hadoopinrealworld.com/jobtracker-and-tasktracker/)
7. [Serialization](https://www.wisdomjobs.com/e-university/hadoop-tutorial-484/serialization-14784.html)
> In Hadoop, interprocess communication between nodes in the system is implemented using remote procedure calls (RPCs). The RPC protocol uses serialization to render the message into a binary stream to be sent to the remote node, which then deserializes the binary stream into the original message
### MapReduce

1. [Concept](https://www.youtube.com/watch?v=SqvAaB3vK8U)
2. [Write a psuedocode for "Grop By" aggregation in a datbase]()
3. [Matrix Multiplication using Mapreduce]()
4. [PsuedoCode for KMeans Algo in MapReduce]()

## Hive
> Hive is data warehouse infrastructure tool to process structured data in hadoop, intially was developed by Facebook and later Open Sourced was used by Amazon in Elastic MapReduce.

**Hive is not** a relational database, or OLTP tool, real time queries or low-level queries.
**OLAP** tool provides SQL typed language called HiveQL or HQL.

1. [Hive and Architecture and it's component](https://www.youtube.com/watch?v=5IAsnI4lwZI)
2. [When executing Hive Queries in different directories, why is metastore_db created in all places from where hive is luanched?](https://www.projectpro.io/article/hive-interview-questions-and-answers-for-2018/246#:~:text=10)
## Spark

Fast expensive cluster computing system.<br>
>Spark contains Resilient Distributed Datasets (RDDs) that save the
time taken in reading and writing operations, and hence it runs
almost 10???100 times faster than Hadoop.

>DAG is the scheduling layer of the Apache Spark architecture that
implements stage-oriented scheduling. Compared to MapReduce
that creates a graph in two stages, Map and Reduce, Apache Spark
can create DAGs that contain many stages.

Key features :  FIRFCB

Iterative operations on MR vs spark.<br>
Interactive " <br>
API Support in Scala, Python

1. [The way we have spark shell and PySpark shell it is possible to have such shell in Map Reduce? if not specify the reason. How is Mlibb library different than ML Library different in Spark?]()
2. [What are various data sources available ib Spark SQL? Why is there need for broadcast variables when working with Apache Spark?]()
3. [What are transformation in RDD? How is narrow transformation different than wide transformation]()
4. [What do you underrstand by SchemaRDD and Apache Spark RDD? How spark is different from HQl and SQL?]()
## Casandra

Column Oriented database, based on Amazon's DynamoDB and model on Google's BigData, created at Facebook.<br>
Fault tolerant due to replication factor.<br>
CQL treats the database as KeySpaces as container of table.<br>
>Write operations :- it is captured by the commit logs, later data will be captured in memtable. Whenever memtable is full, data will be written into the SStable file.

> Read Operations :- gets value from mem-table and check bloom filter to find appropriate SStable.

> Column is basic data structure of cassandra with three values name,value & timestamp.

> Super column is name , ```map<timestamp,column>```



## Zokeeper
Co-ordinator
## HBase

>NoSQL database which can be used for REST, Avro or Thrift, It's modeled after Goggle's Big Table.

## Pig 
1 line of pig = 100 lines of MapReduce

## Oozie
Job Scheduler

## Flume
Data injestion in HDFS

## SQoop
SQL -> HDFS

## Solar and Lucene
Search and indexing

## Ambari
Used to maintain Hadoop Cluster