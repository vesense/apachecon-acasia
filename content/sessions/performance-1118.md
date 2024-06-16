---
title: "Let’s see how fast Impala runs on Iceberg"
date: "2024-07-26 14:00:00" 
track: "performance"
presenters: "Zoltán Borók-Nagy"
stype: "English Session"
---
Apache Impala is a distributed massively parallel query engine designed for high-performance querying of large-scale data. There has been a long list of new features recently around supporting Apache Iceberg tables such as reading, writing, time traveling, and so on. However, in a big data environment it is also a must to be performant. Since Impala has been designed to be fast, it has its own way of reading Iceberg tables. Other engines might simply use the Iceberg library to perform reads, while Impala has a C++ implementation itself optimized for speed.

Nowadays, even big data storage techniques have to offer the possibility not just to store data but also to alter and delete data on a row level. Apache Iceberg solves this by using delete files that live alongside the data files. It is the responsibility of the query engines to then apply the delete files on the data files when querying the data. To efficiently read the data of such tables we implemented new Iceberg-specific operators in Impala.

In this talk we will go into the implementation details and reveal what is the secret behind Impala’s great performance in general and also when reading Iceberg tables with position delete files. We will also show some measurements where we compare Impala’s performance with other open-source query engines.

By the end of this talk, you should have a high-level understanding of Impala’s and Iceberg’s architecture, the performance tricks we implemented in Impala specifically for Iceberg, and you will see how Impala competes with other engines.
 ### Speakers: 
 <img src="https://sessionize.com/image/982d-400o400o1-KiS1dLEbbFFudUWjA5dcLW.jpg" width="200" /><br>Zoltán Borók-Nagy: Cloudera, Principal Engineer, Zoltán is a software engineer at Cloudera, working on Apache Impala. He is also a PMC member on the project. Currently he is leading the Impala/Iceberg integration efforts. Before Cloudera, Zoltán worked on C++ static analysis tools. He is interested in distributed, massively parallel systems, databases, and performance engineering.
 <br><br>