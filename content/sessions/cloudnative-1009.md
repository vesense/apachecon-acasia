---
title: "Seata's Cloud-Native Evolution: A Roadmap from Deployment to Future Possibilities"
date: "2024-07-28 15:00:00" 
track: "cloudnative"
presenters: "Xiangkun Yi"
stype: "Chinese Session"
---
The evolution from monolithic architecture to microservices, and from standalone databases to distributed database systems, has become an undisputed reality in modern service delivery. Applications are now broken down into multiple independently deployable services, necessitating remote collaboration among services to complete transactions. This shift introduces complexity in distributed transaction management, requiring solutions that are not only efficient but also adaptable to the ever-changing cloud-native environment.

The discussion will include how Seata is stepping into Seata 2.0 by adapting to the cloud-native trends. Particularly, the introduction of the Raft consensus mechanism for storing transaction metadata allows for distributed transaction processing without relying on traditional databases and message queues, using file storage and inter-cluster consistency instead. Additionally, the use of Seata's K8s Operator as a means of managing and automating Seata service deployments underscores Seata 2.0's cloud-native adaptability.

Looking ahead, the presentation will explore Seata's further work in the cloud-native domain, including managing cluster configurations through a console and enhancing cluster operations with the expansion of seata-ctl. This represents a key step towards a comprehensive cloud-native distributed transaction management solution. This talk will not only showcase Seata's current achievements but also provide a clear roadmap for its development, illustrating how it adapts to and leads the future trends in microservice architecture.
 ### Speakers: 

 <img src="https://sessionize.com/image/91bb-400o400o1-nKKKZUWXVJ5XYnXihK1tQW.jpg" width="200" /><br>Xiangkun Yi: Tsinghua University,, I'm Xiangkun Yin, and I am currently a Master's student specializing in Software Engineering at Tsinghua University. With a keen interest in open-source projects, I've actively contributed to several communities, and have recently been honored with the Committer role in Apache Seata (Incubating). Within Seata, I have made some major contributions, leading several key projects, such as the Seata operator, the frontend designer, seata-go Saga implementation.
 <br><br>