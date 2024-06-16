---
title: "Impala discovers Iceberg Metadata Tables"
date: "2024-07-26 15:45:00" 
track: "datalake"
presenters: "Daniel Becker"
stype: "English Session"
---
Storing extensive metadata is one of the key features of the Apache Iceberg table format, helping query engines plan and execute queries efficiently. As Iceberg provides an API to query this metadata, it can be presented in query engines as a set of virtual tables, which can be queried with SQL, including filtering, aggregation and joins with other metadata or even regular tables. This feature provides an invaluable table maintenance tool for database administrators.

During the past year we have been working on making Iceberg metadata tables available in Apache Impala, a high-performance, distributed, massively parallel query engine. Query execution in Impala is implemented in C++, which presented some challenges as the Iceberg API is Java-based. 

In addition, the format in which Iceberg returns data (as Java objects, accessed through JNI) also differs from the format in which Impala normally receives its input data from on-disk files, even for the same SQL data types. The difference is especially pronounced in the case of complex types (structs, arrays and maps), and this necessitated extra steps to incorporate them.

This talk will guide you through all the new Impala features related to Iceberg metadata tables and describe how we overcame the obstacles that arose during their implementation.
 ### Speakers: 
 <img src="https://sessionize.com/image/24b2-400o400o1-L1sybGq4B29dVEAX76VS4t.jpg" width="200" /><br>Daniel Becker: nan, Software Engineer, Cloudera, Daniel Becker started working on Apache Impala in 2019 at Cloudera. His Impala contributions encompass various topics, including LLVM code generation, complex types, Parquet and Iceberg. He is a member of the Apache Impala PMC and has a degree from Pázmány Péter Catholic University.
 <br><br>