---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Apache Kafka and Redis"
tags: ['Oracle', 'Kafaka', 'Redis']
image: "2022-01-25/kafkaRedis-1.jpeg"
identifier: 3
---
Today, the most popular tools for message streaming like log aggregation are Kafka and Redis. Both tools provide the functionality of data streaming and aggregation in their own respective ways. Here, we are going to compare the two in regards to their various capabilities and performance tests.

Author and collect by: Cell

<!--more-->

<blockquote class="tip">

<strong>Redis</strong> is an open source (BSD licensed), in-memory data structure store, used as a database, cache, and message broker. Redis provides data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes, and streams. Redis has built-in replication, Lua scripting, LRU eviction, transactions, and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster.

<strong>Apache Kafka</strong> is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Redis:</h4>

Redis is an in-memory, key-value data store which is also open source. It is extremely fast one can use it for caching session management, high-performance database and a message broker. In terms of storage and multiple functionalities, Redis is a bit different from Kafka.


<br>
Redis is an acronym for the Remote Dictionary Server. It is a key-value store, this key-value store can be used as a repository for reading and writing data. Redis is a No-SQL database, which means that unlike MySQL, or Oracle database, it does not have structures such as table/row/column/functions/ procedures, etc. and also it does not support commands like SELECT, INSERT, DELETE and UPDATE. Strings, hashes, lists, sets and sorted sets are the different data structures provided by Redis.
<br>


![db]({{ site.baseurl }}/assets/img/2022-01-25/db-1.png){: .small70-image}
<em class="figure">Fig. Database</em>
<br>

![Redis]({{ site.baseurl }}/assets/img/2022-01-25/r1.png){: .small70-image}
<em class="figure">Fig. Redis</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Why is redis so fast</h4>

<br>
Redis is basically a memory operation, so it is very fast

<br>
Redis communication uses non blocking IO, and its internal implementation adopts epoll + simple event framework. Epoll’s read, write, close, connection are converted into events, and then use epoll’s multiplexing feature, never waste a bit of time on IO.

epoll’s high performance makes redis.


<br>
Single redis adopts single process, single thread and single instance to avoid unnecessary context switching and competition conditions.


<br>
<strong>Epoll</strong> (this technology is mostly used in Linux)Instead of copying file descriptors (FD) between user mode and kernel mode, the shared space is opened up by MMAP technology. All FDS are stored in the red black tree, and the FD with returned results is placed in the linked list. The user process reads the returned results through the linked list. Pseudo asynchronous I / o has high performance. Epoll can be divided into two modes: horizontal triggering and edge starting. Et is edge triggering, and lt is horizontal triggering. One means that only the marginal trigger is changed, and the other means that it will be triggered at a certain stage

![Redis]({{ site.baseurl }}/assets/img/2022-01-25/r2.jpeg){: .small70-image}
<em class="figure">Fig. Redis</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Apache Kafka</h4>

<br>
Apache Kafka is a messaging system that allows you to publish and subscribe to streams of messages that are based on topics and partition. In this way, it is similar to products such as ActiveMQ, RabbitMQ. But even with these similarities, Kafka has a range of fundamental differences from traditional messaging systems that make it different complete
<br>

![kafka1]({{ site.baseurl }}/assets/img/2022-01-25/k1.png){: .small70-image}
<em class="figure">Fig . kafka.</em>
<br>



<hr class="with-margin">
<h4 class="header" id="quantization">Why Apache Kafka is so Fast </h4>

Low-Latency I/O: There are two possible places which can be used for storing and caching the data: Random Access Memory (RAM) and Disk.
<br>

Kafka Avoids the Seek Time.
<br>


Zero Copy Principle.
<br>


Optimal Data Structure: Tree vs. Queue.
<br>


Horizontal Scaling
<br>


Compression & Batching of Data.
<br>

![kafkaRedis]({{ site.baseurl }}/assets/img/2022-01-25/k3.png){: .small70-image}
<em class="figure">Fig . One design.</em>
<br>


![kafkaRedis]({{ site.baseurl }}/assets/img/2022-01-25/Kafka-Operation-1.png){: .small70-image}
<em class="figure">Fig . One design.</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Why Apache Kafka is so Fast </h4>


![kafkaRedis]({{ site.baseurl }}/assets/img/2022-01-25/diff.png){: .small70-image}
<em class="figure">Fig . Summary.</em>
<br>

![kafkaRedis]({{ site.baseurl }}/assets/img/2022-01-25/one.png){: .small70-image}
<em class="figure">Fig . Cases.</em>
<br>

<hr class="with-margin">
### References

<ol>
  <li><a href="https://redis.io/">Redis</a></li>
</ol>

<ol>
  <li><a href="https://kafka.apache.org/">APACHE KAFKA</a></li>
</ol>

<ol>
  <li><a href="https://hub.docker.com/_/redis">Docker Image Redis</a></li>
</ol>

<ol>
  <li><a href="https://www.geeksforgeeks.org/why-apache-kafka-is-so-fast/#:~:text=Horizontal%20Scaling%3A%20Kafka%20has%20the,throughput%20and%20provide%20low%20latency.">Why Apache Kafka is so Fast</a></li>
</ol>

<hr class="with-margin">

![go]({{ site.baseurl }}/assets/img/2022-01-25/download.png){: .autofit-image}
<br>