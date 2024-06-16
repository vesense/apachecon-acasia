---
title: "Row-level modifications at petabyte-scale via Impala on Iceberg"
date: "2024-07-26 16:15:00" 
track: "datastorage"
presenters: "Péter Rózsa,Zoltán Borók-Nagy"
stype: "English Session"
---
Apache Impala is a distributed, massively parallel query engine for big data. Initially, it focused on fast query execution on top of large datasets that were ingested via long-running batch jobs. The table schema and the ingested data typically remained unchanged, and row-level modifications were impractical. Today's expectations for modern data warehouse engines have risen significantly, users now want to have RDBMS-like capabilities in their data warehouses, e.g.: schema and partition evolution, time-travel, and the focus of this talk: row-level modification. Apache Iceberg is a cutting-edge table format that delivers these advanced write capabilities for large-scale data.

In this talk, you will learn about how Apache Impala leverages Iceberg’s writing capabilities for large-scale data, and how Impala implements data manipulation operations like DELETE, UPDATE, and MERGE. Join us for this session to discover how Impala evolved to meet these emerging requirements.
 ### Speakers: 
 <img src="https://sessionize.com/image/0f03-400o400o1-VjFuA65v8Md5uQxrNPHre2.jpg" width="200" /><br>Péter Rózsa: Cloudera, Software Engineer, Péter Rózsa, a Software Engineer at Cloudera since 2020, started contributing to Apache Impala in 2022. He's been working on different parts of the Impala project, recently on Iceberg integrations
 <br><br><img src="https://sessionize.com/image/982d-400o400o1-KiS1dLEbbFFudUWjA5dcLW.jpg" width="200" /><br>Zoltán Borók-Nagy: Cloudera, Principal Engineer, Zoltán is a software engineer at Cloudera, working on Apache Impala. He is also a PMC member on the project. Currently he is leading the Impala/Iceberg integration efforts. Before Cloudera, Zoltán worked on C++ static analysis tools. He is interested in distributed, massively parallel systems, databases, and performance engineering.
 <br><br>