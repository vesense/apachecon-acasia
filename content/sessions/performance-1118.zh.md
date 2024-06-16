---
title: "让我们看看Apache Impala在 Apache Iceberg 上跑得有多快"
date: "2024-07-26 14:00:00" 
track: "performance"
presenters: "Zoltán Borók-Nagy"
stype: "英文文演讲"
---
Apache Impala是一个分布式大规模并行查询引擎，专为大规模数据的高性能查询而设计。最近出现了一长串支持Apache Iceberg表的新特性，比如读、写、时间旅行等等。然而，在大数据环境中，性能也是必须的。由于黑斑羚被设计得很快，它有自己的方式来读取冰山表。其他引擎可能只是简单地使用Iceberg库来执行读取，而Impala本身有一个c++实现来优化速度。

如今，即使是大数据存储技术，也必须不仅提供存储数据的可能性，还必须提供在行级别上更改和删除数据的可能性。Apache Iceberg通过使用数据文件旁边的删除文件解决了这个问题。查询引擎负责在查询数据时对数据文件应用删除文件。为了有效地读取这些表的数据，我们在Impala中实现了新的针对冰山的操作符。

在这个演讲中，我们将深入到实现的细节，并揭示Impala出色的性能背后的秘密，以及在读取带有位置删除文件的冰山表时的秘密。我们还将展示一些测量结果，将Impala的性能与其他开源查询引擎进行比较。

在演讲结束时，你应该对Impala和Iceberg的架构有一个高层次的了解，我们在Impala中特别为Iceberg实现的性能技巧，你将看到Impala是如何与其他引擎竞争的。
 ### Speakers: 
 <img src="https://sessionize.com/image/982d-400o400o1-KiS1dLEbbFFudUWjA5dcLW.jpg" width="200" /><br>Zoltan Borok-Nagy: Cloudera，首席工程师, Zoltán是Cloudera的一名软件工程师，正在开发Apache Impala。他也是该项目的PMC成员。目前，他正在领导黑斑羚/冰山的整合工作。在Cloudera之前，Zoltán致力于c++静态分析工具。他对分布式、大规模并行系统、数据库和性能工程感兴趣。
 <br><br>