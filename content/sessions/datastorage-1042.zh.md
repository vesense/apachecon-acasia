---
title: "通过冰山上的黑斑羚进行行级修改"
date: "2024-07-26 16:15:00" 
track: "datastorage"
presenters: "Péter Rózsa,Zoltán Borók-Nagy"
stype: "英文演讲"
---
Apache Impala是一个分布式、大规模并行的大数据查询引擎。最初，它专注于通过长时间运行的批处理作业获取的大型数据集之上的快速查询执行。表模式和摄取的数据通常保持不变，行级别的修改是不切实际的。今天对现代数据仓库引擎的期望已经显著提高，用户现在希望在他们的数据仓库中拥有类似rdbms的功能，例如:模式和分区演化、时间旅行，以及本次演讲的重点:行级修改。Apache Iceberg是一种先进的表格式，它为大规模数据提供了这些高级写入功能。

在本次演讲中，您将了解Apache Impala如何利用Iceberg的大规模数据编写能力，以及Impala如何实现数据操作操作，如DELETE, UPDATE和MERGE。和我们一起来探索黑斑羚是如何进化以满足这些新需求的。
 ### Speakers: 
 <img src="https://sessionize.com/image/0f03-400o400o1-VjFuA65v8Md5uQxrNPHre2.jpg" width="200" /><br>Péter Rózsa: Cloudera，软件工程师, psamter Rózsa自2020年以来一直是Cloudera的软件工程师，从2022年开始为Apache Impala做出贡献。他一直在为Impala项目的不同部分工作，最近是冰山集成项目
 <br><br><img src="https://sessionize.com/image/982d-400o400o1-KiS1dLEbbFFudUWjA5dcLW.jpg" width="200" /><br>Zoltán Borók-Nagy: Cloudera，首席工程师, Zoltán是Cloudera的一名软件工程师，正在开发Apache Impala。他也是该项目的PMC成员。目前，他正在领导黑斑羚/冰山的整合工作。在Cloudera之前，Zoltán致力于c++静态分析工具。他对分布式、大规模并行系统、数据库和性能工程感兴趣。
 <br><br>