## Overview of Apache Spark
- Objective of this overview is to introduce and make you familiar about Apache Spark, as quick as possible
- It is meant to help those, who are in deciding process, to decide if Spark is for your purpose and should you invest more time in knowing about it.
- It can also help you, if you are impatient in knowing about Spark

### What is Apache Spark
A general-purpose cluster computing system, i.e., distributed computing environment, over a fault tolerant cluster of computing nodes.

Spark comes with an DAG execution engine with bunch of tools to support the cluster computing (execution) and monitoring same

### Framework services
Below are the primary services offered by spark, which you should know about

- Cluster computing
	- Job Scheduling
	- Directed acyclic graph execution (DAG Execution)
- Resilient Distributed Dataset (RDD)
- Spark Streaming
- Spark SQL, DataFrames and Datasets Guide
- Structured data processing
- GraphX
- MLib

### Version & Support details
| Current version | Languages supported                        | Operating systems supported |
|:----------------|:-------------------------------------------|:----------------------------|
| 2.4             | JAVA (8+)                                  |                             |
|                 | Scala (2.11) - Python (2.7+/3.4) - R (3.1) | Linux                       |
|                 | Python (2.7+/3.4) - R (3.1)                | Mac OS                      |
|                 | R (3.1)                                    | Windows                     |
|                 |                                            |                             |


### Cluster computing
- Cluster computing is what you use to run your applications as Spark applications
- Spark comes with high level APIs, you **submit** your your applications as jobs, which Spark schedules on its cluster before running. 
- Spark applications run as independent sets of processes on a cluster, coordinated by the SparkContext object in your main program (called the driver program).
- The components of Spark is as below
	![Apache Spark Components](https://spark.apache.org/docs/latest/img/cluster-overview.png "Spark components")
- From the image shown the **Task** is where your application runs, spark sends your applications to the executors, which run on cluster nodes, these nodes can be provided by any cluster provider (MESOS, Kubernetes, Hadoop, Standalone)
- Each driver program has a web UI, typically on port 4040, that displays information about running tasks, executors, and storage usage
- Spark gives control over resource allocation both across applications (at the level of the cluster manager) and within applications (if multiple computations are happening on the same SparkContext)
- Please refer [here](https://spark.apache.org/docs/latest/cluster-overview.html) to read more about the cluster mode of Spark

### Resilient Distributed Dataset (RDD)
- One of the core abstraction provided by Spark is RDD, the **R**esilient **D**istributed **D**ataset (RDD), which is a fault-tolerant collection of data elements that can be operated on in parallel.

- Other abstraction by Spark is **variables**, which are shared or broadcast, depending on you want to share data across tasks or between tasks. broadcast variables are cached on all nodes. Spark automatically broadcasts variables which are needed in computations across nodes. 

- We can taken any collection object from the program and parallelize it over the cluster, you can decide how many slices of the data you want to cut in parallelizing the data set, Spark does this automatically, however the API provides options for you to decide the number of partitions. 

- Choose RDD if you want to operate on the data in parallel and you are not concerned about the order of the data and/or processing

- RDD can be in memory of the program or in external data store (HDFS, Filesystem, Cassandra, S3...)

- Using RDD will make your spark application stateful

- We can run `transformations` and `accumulation` type of operations on RDD, transformations are lazy and only computed when action required to return the computed data

- RDDs can be re-distributed over partitions using expensive operations known as **shuffle**

- Please refer [here](https://spark.apache.org/docs/latest/rdd-programming-guide.html#overview) to know more about RDD

### Spark Streaming
### Spark SQL, DataFrames and Datasets Guide
### Structured data processing
### GraphX
