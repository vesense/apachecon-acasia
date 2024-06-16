---
title: "小米湖仓数据与人工智能集成的实践"
date: "2024-07-27 15:45:00" 
track: "datalake"
presenters: "Peidian Li"
stype: "中文演讲"
---
本次分享主要介绍小米在data和AI场景下的数据湖实践。在BI场景中，我们将介绍使用Apache Iceberg的业务实践和智能优化策略。在AI场景中，我们将介绍对非结构化数据的管理。此外，我们将介绍我们在数据和人工智能场景下使用重力子实现元数据统一的解决方案。

1. Apache Iceberg在小米的优化与实践
- Apache Iceberg的实践
- Apache Iceberg在小米内部管理数万个表和近50 PB的数据。我们将介绍小米使用Apache冰山的内部业务场景，包括离线和实时场景，以及Apache Iceberg如何帮助用户降低成本，提高效率。
-智能优化Apache Iceberg
-本节将介绍如何智能优化Apache Iceberg以提高查询效率。我们将介绍表画像和查询指标系统，以及如何使用Zorder帮助用户自动完成表优化。
2. 人工智能场景中非结构化数据的管理和使用
-介绍小米使用Gravitino Fileset管理非结构化数据的做法
-我们将介绍如何使用重力文件集来管理非结构化数据。如何标准化非结构化数据的路径访问，如何管理数据生命周期，如何与Spark引擎集成，以及如何与TensorFlow或PyTorch等机器学习引擎集成
3. 介绍Data和AI场景下元数据统一实践
-冰山元数据服务简介
-我们将介绍如何使用Gravetino来管理冰山的元数据。为什么我们使用冰山休息目录而不是Hive目录?冰山休息目录能带来什么优势?
-介绍使用Gravitino统一元数据的实践
-介绍如何使用Gravitino统一数据湖元数据，统一元数据给我们带来哪些优势，如何实现结构化和非结构化数据元数据的统一管理。
 ### Speakers: 
 <img src="https://sessionize.com/image/5727-400o400o1-NcbSszcmadR5rworVwYgoy.jpg" width="200" /><br>Peidian Li: 小米软件研发工程师, 小米软件研发工程师，负责Apache Iceberg、Apache Paimon、Gravitino的开发。
 <br><br>