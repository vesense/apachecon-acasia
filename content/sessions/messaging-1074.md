---
title: "Apache Pulsar cluster scale control and stability practice"
date: "2024-07-26 14:00:00" 
track: "messaging"
presenters: "Lin Lin"
stype: "Chinese Session"
---
Whether it is service cloud nativeization or AI model training, the stability of the message queue as a basic component is increasingly important.
The magnitude of upper-layer business is getting larger and larger, and the requirements for message queue performance and throughput are getting higher and higher.
The continuous expansion of clusters will continue to expand the scale of the cluster. Large clusters are prone to problems such as hot spots and excessive explosion radius, which have always affected the stability of upper-layer services.
A cluster that is too small cannot carry the rising business traffic, and naturally has problems such as insufficient resource utilization.
Huawei's terminal cloud middleware team has summarized a set of cluster scale control practices in front-line production environments for many years. The cluster size and business isolation are controlled within a reasonable range, and the message queue is serverless for high-traffic business, and the server schedules resources across clusters.
On the premise of ensuring cluster resource utilization, the stability of the message queue is continuously improved.
 ### Speakers: 
 <img src="https://sessionize.com/image/ec9e-400o400o1-KuHvwPtuLnXMT8uZBbVMQi.jpg" width="200" /><br>lin lin: Technical Director of Huawei Terminal Cloud Message Queue, Huawei SDE expert, middleware technical director, formerly worked for Tencent and Ant Financial.
Focus on middleware and infrastructure, with more than 10 years of relevant experience, committed to building high-quality infrastructure.
Apache Pulsar Committer & PMC member.
Author of《深入理解Apache Dubbo与实战》《深入解析Apache Pulsar》
 <br><br>