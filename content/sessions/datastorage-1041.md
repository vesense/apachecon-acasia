---
title: "Thoughts and Practices on Storage and Computing Separation Architecture at Xiaomi"
date: "2024-07-26 15:45:00" 
track: "datastorage"
presenters: "Xing Yong"
stype: "Chinese Session"
---
In order to achieve ultimate cost-effectiveness, Xiaomi has carried out multi-stage exploration and technical practice in the domain of big data storage and computing architecture. 

In terms of storage, we have built HDFS Tiering capabilities of object-based storage, and also implemented the storage of Apache Iceberg on the cloud; In the realm of computing, we have leveraged Yarn federation to achieve hybrid cloud scheduling, enabling us to expand our resources to include ARM-based machines and Spot instances, among other heterogeneous resources. 

This presentation will primarily focus on the practical implementation of the aforementioned architecture in a production environment, while showcasing the business benefits derived from the separation of storage and computing.

Outline：
1) Thoughts on the Separation of Storage and Computing
- Core Elements and Cost Model
- Key Challenges

By examining the system evolutionary history of the separation of storage and computing, we can analyze the core elements of this architecture and abstract a cost model for it. 
From the architectural perspective, we can deduce the key challenges involved in implementing the separation of storage and computing, thereby identifying the key issues to be addressed, such as multi-cloud migration and scheduling, dedicated bandwidth between hybrid clouds, challenges using object storage, and unified metadata management.

2) Practical Implementation on the Separation of Storage and Computing
- HDFS Tiering Architecture
- Iceberg Object-based Storage Architecture
- Yarn Federation Hybrid Cloud Architecture

Xiaomi has experienced a journey in storage architecture, implementing the HDFS Tiering architecture and the Iceberg object-based storage architecture. We will focus on the challenges encountered during the landing process and technical solutions. In terms of computing scheduling, we has built the hybrid cloud scheduling capabilities of Yarn, enabling the scheduling of different heterogeneous resources, including ARM-based machines, Spot instances, and elastic container instances, based on job and resource profiling. 

This presentation will delve into the challenges and solutions throughout this process.


Benefits of the audience：
- Understanding the core elements, cost model, and key challenges on the separation of storage and computing.
- Insights into cloud object-based storage architecture practices based on HDFS and Iceberg.
- Insights into multi-cloud and hybrid cloud scheduling based on Yarn.
 ### Speakers: 
 <img src="https://sessionize.com/image/0d11-400o400o1-aipcfzCvzuZraw1v3xxNAN.jpg" width="200" /><br>Xing Yong: Company: Xiaomi, Title: Head of Cloud Computing Platform, Xiaomi Senior Software R&D Engineer. Responsible for the development of distributed storage and computing system.
 <br><br>