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
* Apache Hadoop HDFS     

Hadoop File System was developed using distributed file system design as core part of Apache Hadoop. It is run on commodity hardware. Unlike other distributed systems, HDFS is highly faulttolerant and designed using low-cost hardware.   

HDFS holds very large amount of data and provides easier access. To store such huge data, the files are stored across multiple machines. These files are stored in redundant fashion to rescue the system from possible data losses in case of failure. HDFS also makes applications available to parallel processing.   

* Apache Hadoop YARN (Yet Another Resource Negotiator)  

As core part of Apache Hadoop YARN is to split up the functionalities of resource management and job scheduling/monitoring into separate daemons. The idea is to have a global ResourceManager (RM) and per-application ApplicationMaster (AM). An application is either a single job or a DAG of jobs.   

The ResourceManager and the NodeManager form the data-computation framework. The ResourceManager is the ultimate authority that arbitrates resources among all the applications in the system. The NodeManager is the per-machine framework agent who is responsible for containers, monitoring their resource usage (cpu, memory, disk, network) and reporting the same to the ResourceManager/Scheduler.   

The per-application ApplicationMaster is, in effect, a framework specific library and is tasked with negotiating resources from the ResourceManager and working with the NodeManager(s) to execute and monitor the tasks.     

* Apache Hadoop MapReducd      

As core part of Apache Hadoop MapReduce is a software framework for easily writing applications which process vast amounts of data (multi-terabyte data-sets) in-parallel on large clusters (thousands of nodes) of commodity hardware in a reliable, fault-tolerant manner.      

A MapReduce job usually splits the input data-set into independent chunks which are processed by the map tasks in a completely parallel manner. The framework sorts the outputs of the maps, which are then input to the reduce tasks. Typically both the input and the output of the job are stored in a file-system. The framework takes care of scheduling tasks, monitoring them and re-executes the failed tasks.  
* Apache Ambari
* Pig 
* Hive
* Tez
* Spark
* MESOS
* Apache Hbase
* Apache Storm
* Zookeeper
* Oozie
#### Data Ingestion
* oqoop
* Flu
* Kafka



## Login
To login into Ambari is (If you have problems login to Ambari check the Windows Services in your Control Panel make sure Oracle database is not running on port 8080. You can stop OracleServiceXE and change the startup type to manual so the next time login in your computer the Oracle Service is not running.) :
* Username : maria_dev
* Password : maria_dev

## Install Instructions
[Getting Started with Horton Works](https://hortonworks.com/tutorial/hadoop-tutorial-getting-started-with-hdp/)
   
## Contact      
* [Linkedin](https://www.linkedin.com/in/john-cusey-06b7184/)    
* Email: jjcusey@gmail.com  
