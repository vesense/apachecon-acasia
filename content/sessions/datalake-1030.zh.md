---
title: "Impala发现了Iceberg元数据表"
date: "2024-07-26 15:45:00" 
track: "datalake"
presenters: "Daniel Becker"
stype: "英文演讲"
---
存储大量元数据是Apache Iceberg表格式的关键特性之一，它可以帮助查询引擎高效地计划和执行查询。由于Iceberg提供了一个API来查询这些元数据，它可以在查询引擎中以一组虚拟表的形式呈现，这些虚拟表可以用SQL进行查询，包括过滤、聚合和与其他元数据甚至常规表的连接。这个特性为数据库管理员提供了一个非常有用的表维护工具。

在过去的一年里，我们一直致力于在Apache Impala(一个高性能、分布式、大规模并行的查询引擎)中提供Iceberg元数据表。Impala中的查询执行是用c++实现的，由于Iceberg的API是基于java的，这给它带来了一些挑战。

此外，Iceberg返回数据(作为Java对象，通过JNI访问)的格式也不同于Impala通常从磁盘文件接收输入数据的格式，即使是相同的SQL数据类型也是如此。在复杂类型(结构体、数组和映射)的情况下，这种差异尤其明显，这就需要额外的步骤来合并它们。

本演讲将引导您了解所有与Iceberg元数据表相关的Impala新功能，并描述我们如何克服在实现过程中出现的障碍。
 ### Speakers: 
 <img src="https://sessionize.com/image/24b2-400o400o1-L1sybGq4B29dVEAX76VS4t.jpg" width="200" /><br>Daniel Becker: Cloudera软件工程师, Daniel Becker于2019年开始在Cloudera开发Apache Impala。他对Impala的贡献涵盖了各种主题，包括LLVM代码生成、复杂类型、Parquet和Iceberg。他是Apache Impala PMC的成员，拥有Pázmány psamter Catholic University的学位。
 <br><br>