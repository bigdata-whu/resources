# Open Source Big Data Analytics Tools

[ÔÄ¶ÁÖÐÎÄ°æ±¾](tools_cn.md)

<https://www.softwaretestinghelp.com/big-data-tools/>


***********************************

As we all know, data is everything in today¡¯s IT world. Moreover, this data 
keeps proliferating fast each day.

Earlier, we talked about data in kilobytes and megabytes. But nowadays, we are 
talking about terabytes.

Data is meaningless until it turns into useful information and knowledge which 
can aid the management in decision making. To do this, we need the help  
of analytical softwares to handle big data. Such kind of softwares help in 
storing, analyzing, reporting and processing a lot more with big data.

## 1. Apache Hadoop

![hadoop log](pix/hadoop-logo.jpg)

Apache Hadoop is a software framework employed for clustered file system and 
handling of big data. It processes datasets of big data by means of the 
MapReduce programming model.

Apache Hadoop was the original open-source framework for distributed 
processing and analysis of big data sets on clusters. The Hadoop ecosystem 
includes related software and utilities, including Apache Hive, Apache HBase, 
Spark, Kafka, and many others.

Hadoop is written in Java and provides 
cross-platform support. This software is free to use under the Apache License.

No doubt, this is the topmost big data tool. In fact, 
over half of the Fortune 50 companies use Hadoop. 
Some of the Big names include Amazon Web services, Hortonworks, IBM, 
Intel, Microsoft, Facebook, etc.

Pros:

* The core strength of Hadoop is its HDFS (Hadoop Distributed File System) 
which has the ability to hold all type of data ¨C video, images, JSON, XML, 
and plain text over the same file system.
* Highly useful for R&D purposes.
* Provides quick access to data.
* Highly scalable
*Highly-available service resting on a cluster of computers

Cons:

* Sometimes disk space issues can be faced due to its 3x data redundancy.
* I/O operations could have been optimized for better performance.

## 2. What is MapReduce ?
Apache Hadoop MapReduce is a software framework for writing jobs that process 
vast amounts of data. Input data is split into independent chunks. Each chunk 
is processed in parallel across the nodes in your cluster. A MapReduce job 
consists of two functions:

* Mapper: Consumes input data, analyzes it (usually with filter and sorting 
operations), and emits tuples (key-value pairs)

* Reducer: Consumes tuples emitted by the Mapper and performs a summary 
operation that creates a smaller, combined result from the Mapper data

A basic word count MapReduce job example is illustrated in the following diagram:

![MapReduce Job](pix/hdi-word-count-diagram.gif)

The output of this job is a count of how many times each word occurred in the text.

* The mapper takes each line from the input text as an input and breaks it 
into words. It emits a key/value pair each time a word occurs of the word is 
followed by a 1. The output is sorted before sending it to reducer.
* The reducer sums these individual counts for each word and emits a single 
* key/value pair that contains the word followed by the sum of its occurrences.

MapReduce can be implemented in various languages. Java is the most common 
implementation, and is used for demonstration purposes in this course.

