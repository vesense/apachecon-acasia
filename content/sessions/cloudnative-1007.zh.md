---
title: "Apache Pulsar跨kubernetes集群场景的部署实践"
date: "2024-07-28 14:00:00" 
track: "cloudnative"
presenters: "Tian Fang"
stype: "中文演讲"
---
Apache Pulsar集群通常由Apache Pulsar、Apache ZooKeeper、Apache BookKeeper等组成，其中Apache ZooKeeper、Apache BookKeeper通常在Kubernetes中作为statfulset服务。在跨kubernetes集群部署的情况下，这些组件经常面临诸如如何跨多个集群维护统一的顺序索引，以及如何维护最小数量的可用集群副本等问题。本主题探讨如何在跨kubernetes集群场景中部署Apache Pulsar。
 ### Speakers: 
 <img src="https://sessionize.com/image/3fcd-400o400o1-X3L3tRbSJoPYhHdbQYuPXP.jpg" width="200" /><br>Tian Fang: AscentStream, Backend-Engineer, 专注于云原生、无服务器、流、EDA等，CNCF FaaS项目OpenFunction维护者。
 <br><br>