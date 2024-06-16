---
title: "The Practice of Data&AI Integration of Lake and Warehouse in Xiaomi"
date: "2024-07-27 15:45:00" 
track: "datalake"
presenters: "Peidian Li"
stype: "Chinese Session"
---
This sharing mainly introduces Xiaomi's practice of data lake in Data and AI scenarios. In BI scenarios, we will introduce the business practices and intelligent optimization strategies of using Apache Iceberg. In AI scenarios, we will introduce the management  for unstructured data. In addition, we will introduce our solutions for metadata unification using Gravitino in Data and AI scenarios.

1. Optimization and Practice of Apache Iceberg in Xiaomi
- The practice of Apache Iceberg
  - Apache Iceberg manages tens of thousands of tables and nearly 50 PB of data within Xiaomi. We will introduce the internal business scenarios of Xiaomi using Apache Iceberg, including offline and real-time scenarios, as well as how Apache Iceberg can help users reduce costs and increase efficiency.
- Intelligent Optimization in Apache Iceberg
  - This section will introduce how to intelligently optimize Apache iceberg to improve query efficiency. We will introduce the table portrait and query indicator system, and how to use Zorder to help users complete table optimization automatically.
2. Management and Use of Unstructured Data in AI Scenarios
- Introduce the practice of using Gravitino Fileset to manage unstructured data at Xiaomi
  - We will introduce how to use Gravitino Fileset to manage unstructured data. How to standardize path access to unstructured data, how to manage data lifecycle, how to integrate with Spark engine, and how to integrate with machine learning engines such as TensorFlow or PyTorch
3. Introduction to metadata unification practice in Data and AI scenarios
- Introduction to Iceberg's metadata service
  - We will introduce how to use Gravetino to manage the metadata of the iceberg. Why do we use the Iceberg Rest Catalog instead of the Hive catalog? What advantages can the Iceberg Rest Catalog bring?
- Introduce the practice of using Gravitino to unify metadata
  - Introduce how to use Gravitino to unify metadata for data lakes, what advantages does unified metadata brings to us, and how to achieve unified management of metadata for structured and unstructured data.
 ### Speakers: 
 <img src="https://sessionize.com/image/5727-400o400o1-NcbSszcmadR5rworVwYgoy.jpg" width="200" /><br>Peidian Li: Xiaomi Software R&D Engineer, Xiaomi Software R&D Engineer,  Responsible for the development of Apache Iceberg, Apache Paimon, and Gravitino.
 <br><br>