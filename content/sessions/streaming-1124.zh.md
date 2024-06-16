---
title: "Apache Flink中的混合流和批处理"
date: "2024-07-26 15:45:00" 
track: "streaming"
presenters: "Xuannan Su"
stype: "中文演讲"
---
长期以来，流处理和批处理一直是大规模数据处理的两种截然不同的模式。随着统一流和批处理的发展，Apache Flink现在允许在单个引擎中管理这两者。这模糊了流处理和批处理之间的区别，从而产生了一种新的统一数据处理模式，称为混合模式。在这种混合模式下，用户不需要预先确定Flink作业的执行模式。相反，Flink根据数据新鲜度要求自适应地选择和切换执行模式，以有效地平衡延迟和吞吐量。
在这次演讲中，我们将讨论混合模式的概念和优势，并介绍随之而来的技术挑战和设计解决方案。我们将演示混合模式如何在各种用例中将吞吐量提高50%以上。此外，我们还将介绍Flink社区在这一领域的最新发展和未来计划。
 ### Speakers: 
 <img src="https://sessionize.com/image/6797-400o400o1-dbccedf4-ca5c-4ac7-9407-da8d909f00a6.jpg" width="200" /><br>Xuannan Su: 阿里巴巴集团, Xuannan是阿里巴巴的一名软件工程师。他专注于Apache Flink运行时的开发。
 <br><br>