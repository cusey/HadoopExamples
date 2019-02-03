![CuseyHub](https://github.com/cusey/ImageForWiki/blob/master/Logos/CuseyHub_Banner_Small.jpg)    
# Hadoop Examples 

![HortonWorks](https://github.com/cusey/ImageForWiki/blob/master/Logos/hortonworks.PNG)

## Introduction   
Hadoop is a open software platform for distributed stoarge and ditributed processing of very large data sets on computer clusters build from commodity hardware.

## Why Hadoop?  
* Data's too darn big - terabytes per day
* Vertical scaling does not cut it   
         1. Disk seek times    
         2. Hardware failures    
         3. Processing times    
* Horizontal scaling is linear    
* Hadoop: It is not just for batch processing anymore  

### Core Hadoop Ecosystem
* **Apache Hadoop HDFS**     

Hadoop File System was developed using distributed file system design as core part of Apache Hadoop. It is run on commodity hardware. Unlike other distributed systems, HDFS is highly faulttolerant and designed using low-cost hardware.   

HDFS holds very large amount of data and provides easier access. To store such huge data, the files are stored across multiple machines. These files are stored in redundant fashion to rescue the system from possible data losses in case of failure. HDFS also makes applications available to parallel processing. 

* **Apache Hadoop MapReduce**      

As core part of Apache Hadoop MapReduce is a software framework for easily writing applications which process vast amounts of data (multi-terabyte data-sets) in-parallel on large clusters (thousands of nodes) of commodity hardware in a reliable, fault-tolerant manner.      

A MapReduce job usually splits the input data-set into independent chunks which are processed by the map tasks in a completely parallel manner. The framework sorts the outputs of the maps, which are then input to the reduce tasks. Typically both the input and the output of the job are stored in a file-system. The framework takes care of scheduling tasks, monitoring them and re-executes the failed tasks.


* **Apache Hadoop YARN** (Yet Another Resource Negotiator)  

As core part of Apache Hadoop YARN is to split up the functionalities of resource management and job scheduling/monitoring into separate daemons. The idea is to have a global ResourceManager (RM) and per-application ApplicationMaster (AM). An application is either a single job or a DAG of jobs.   

The ResourceManager and the NodeManager form the data-computation framework. The ResourceManager is the ultimate authority that arbitrates resources among all the applications in the system. The NodeManager is the per-machine framework agent who is responsible for containers, monitoring their resource usage (cpu, memory, disk, network) and reporting the same to the ResourceManager/Scheduler.   

The per-application ApplicationMaster is, in effect, a framework specific library and is tasked with negotiating resources from the ResourceManager and working with the NodeManager(s) to execute and monitor the tasks.     

* **MESOS**

Apache Mesos is an open-source project to manage computer clusters. Alternative to Apache Hadoop YARN.

* **Apache Ambari** 

The Apache Ambari project is aimed at making Hadoop management simpler by developing software for provisioning, managing, and monitoring Apache Hadoop clusters. Ambari provides an intuitive, easy-to-use Hadoop management web UI backed by its RESTful APIs.

* **Pig**

The language for this platform is called Pig Latin. Pig can execute its Hadoop jobs in MapReduce, Apache Tez, or Apache Spark. Pig Latin abstracts the programming from the Java MapReduce idiom into a notation which makes MapReduce programming high level, similar to that of SQL for relational database management systems. Pig Latin can be extended using user-defined functions (UDFs) which the user can write in Java, Python, JavaScript, Ruby or Groovy and then call directly from the language.     

* **Hive**

Apache Hive is a data warehouse software project built on top of Apache Hadoop for providing data query and analysis. Hive gives a SQL-like interface to query data stored in various databases and file systems that integrate with Hadoop. Traditional SQL queries must be implemented in the MapReduce Java API to execute SQL applications and queries over distributed data. Hive provides the necessary SQL abstraction to integrate SQL-like queries (HiveQL) into the underlying Java without the need to implement queries in the low-level Java API. Since most data warehousing applications work with SQL-based querying languages, Hive aids portability of SQL-based applications to Hadoop

* **Tez**
* **Spark**
* **Apache Hbase**
* **Apache Storm**
* **Zookeeper**
* **Oozie**
#### Data Ingestion
* **Oqoop**
* **Flume**
* **Kafka**



## Login
To login into Ambari is (If you have problems login to Ambari check the Windows Services in your Control Panel make sure Oracle database is not running on port 8080. You can stop OracleServiceXE and change the startup type to manual so the next time login in your computer the Oracle Service is not running.) :
* Username : maria_dev
* Password : maria_dev

## Install Instructions
[Getting Started with Horton Works](https://hortonworks.com/tutorial/hadoop-tutorial-getting-started-with-hdp/)
   
## Contact      
* [Linkedin](https://www.linkedin.com/in/john-cusey-06b7184/)    
* Email: jjcusey@gmail.com  
