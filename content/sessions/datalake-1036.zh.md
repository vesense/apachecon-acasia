---
title: "Apache Paimon数据湖架构的洞察与设计分析"
date: "2024-07-27 16:15:00" 
track: "datalake"
presenters: "陈卓宇"
stype: "中文演讲"
---
在本次演讲中，我将深入研究Apache Paimon数据湖项目的核心实现细节。

1.我将介绍CDC摄取背后的逻辑，这是一种关键的数据同步机制，允许实时捕获和集成数据更改。这确保了数据湖中的信息始终是最新的。
2.我将详细讨论Paimon表的读写过程，以及它的设计理念。这一部分将包括对Paimon体系结构的理解，特别是如何有效地管理和访问存储在数据湖中的数据。我们将探索如何通过“Bucket”和“Tag”这两个核心概念来优化数据的组织和检索，从而提高数据处理的效率。
3.我将解释主键表下的重复数据删除、部分更新和聚合合并引擎的实现逻辑。
通过本次演讲，与会者将深入了解Apache Paimon数据湖项目。
 ### Speakers: 
 <img src="https://sessionize.com/image/02dd-400o400o1-7DUy7qsWmHeqnmXRx1ghWQ.jpg" width="200" /><br>陈卓宇: 小红书-搜索推荐引擎组-apache streaprk PPMC, paimon贡献者, 对开源充满热情。
 <br><br>