---
title: "Apache Pulsar deployment practice in the cross-Kubernetes cluster scenario"
date: "2024-07-28 14:00:00" 
track: "cloudnative"
presenters: "Tian Fang"
stype: "Chinese Session"
---
Apache Pulsar clusters are usually formed by Apache Pulsar, Apache ZooKeeper, Apache BookKeepr, etc., where Apache ZooKeeper, Apache BookKeeper are usually served as a StatefulSet in Kubernetes. In the case of cross-Kubernetes cluster deployments, these components often face issues such as how to maintain a uniform sequential index across multiple clusters, and how to maintain a minimum number of available cluster replicas. This topic explores how the Apache Pulsar can be deployed in the cross-Kubernetes cluster scenario.
 ### Speakers: 
 <img src="https://sessionize.com/image/3fcd-400o400o1-X3L3tRbSJoPYhHdbQYuPXP.jpg" width="200" /><br>Tian Fang: AscentStream, Backend-Engineer, Focus on cloud native, serverless, streaming, EDA, etc., maintainer of the CNCF FaaS project OpenFunction.
 <br><br>