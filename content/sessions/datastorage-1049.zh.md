---
title: "识别，调和，重复:在Apache臭氧统一副本的路径"
date: "2024-07-27 16:45:00" 
track: "datastorage"
presenters: "Ethan Rose,Ritesh Shukla"
stype: "英文演讲"
---
分布式系统中的故障通常是无界的。Apache Ozone需要抵抗故障，并在面对这些故障时保持数据的持久性和一致性。和解是一项正在开发的新功能，它允许Ozone从故障中恢复，而不依赖于故障发生的方式以及故障之间的持续时间。协调允许对等体识别、报告和解决任何类型的差异，并且可以跨数据持久性模型(如复制和擦除编码)工作。系统可以在没有管理员干预的情况下启动并完成此过程。本演讲将涵盖副本协调背后的动机，可应用于任何存储系统的一般策略，以及使其成为可能的实现细节。
 ### Speakers: 
 <img src="https://sessionize.com/image/750e-400o400o1-n6M4nqrtxwshrQHLRedJjt.jpg" width="200" /><br>伊桑玫瑰: 南, Cloudera高级软件工程师，Apache Ozone PMC成员, Ethan是Cloudera存储团队的一名工程师，他的时间主要用于与开源社区一起开发臭氧，以及帮助新用户将臭氧带入生产环境。他拥有伦斯勒理工学院计算机科学学士学位。
 <br><br><img src="https://sessionize.com/image/8296-400o400o1-Njj22QN2B89Sv2EsqnYVby.png" width="200" /><br>:舒克拉: 南, Cloudera，首席工程师, Ritesh是一名Apache Ozone PMC。他在分布式存储解决方案和系统方面拥有超过十年的经验。他热衷于在解决方案中选择这三者:简单、正确和高效。他目前正在研究Ozone，一个满足HDFS和S3工作负载的分布式对象存储。
 <br><br>