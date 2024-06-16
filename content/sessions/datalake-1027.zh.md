---
title: "在网易使用Apache Gluten和Velox引擎加速Apache Kyuubi的查询"
date: "2024-07-26 14:00:00" 
track: "datalake"
presenters: "尤夕多"
stype: "中文演讲"
---
会议探讨了Kyuubi(一个纯SQL网关)和面筋(一个矢量化执行引擎)的协同使用，以增强SQL查询的性能。Kyuubi通过Thrift JDBC/ODBC接口或RESTful api为最终用户简化了大规模数据操作，减少了对lake - house使用的障碍。它的多租户架构确保了服务器端的资源隔离/共享和数据安全性。会议重点介绍了网易以Apache Gluten和Velox为后端引擎实现的Kyuubi，旨在解决性能瓶颈并分享实际结果。麸质支持各种原生后端，目前的重点是Velox和ClickHouse，未来可能会与Apache Data Fusion等项目集成。
 ### Speakers: 
 <img src="https://sessionize.com/image/0f40-400o400o1-NjV2FCpCH3Lp6YAXXRRtLX.jpg" width="200" /><br>尤夕多: 网易数帆技术专家，Apache Kyuubi PMC成员/ Apache Spark Committer / Apache Gluten PPMC成员, https://github.com/ulysses-you
 <br><br>