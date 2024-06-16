---
title: "Xiaomi's Practice in Flink Stability Optimization and Business Efficiency Improvement with Paimon"
date: "2024-07-27 16:15:00" 
track: "streaming"
presenters: "Shengjie Wang"
stype: "Chinese Session"
---
This sharing mainly introduces some optimizations of Xiaomi in terms of stability and case sharing of Flink+Paimon in helping Xiaomi improve business production efficiency.
1. Flink Stability Optimization
  1.1Flink High Availability (HA) Capability Construction
    Fault tolerance is very important in production. This segment primarily discusses Xiaomi's efforts in establishing robust high-availability (HA) capabilities within its job processing architecture, specifically delving into mechanisms such as Checkpoint High Availability and MQ High Availability.
  1.2 Enhancing Problem Diagnosis Efficiency with Flink Job Debugging
    Troubleshooting real-time jobs is very complex, for example, aggregation results do not meet expectations, data is suspected to be lost, etc.
    In this section, we will introduce the implementation process of operator-level debugging capabilities for Xiaomi Flink Jobs.
  1.3 Flink Fault Automatic Recovery Capability Building
    The production environment is very complex. We hope to automatically handle failures in some common scenarios, such as the recovery of hotspot machines and long-term checkpoint trigger failures, etc., to reduce users' energy investment and operation and maintenance pressure.
1. How Flink + Paimon Helps Improve Business Efficiency
This section will introduce the practical scenarios of Xiaomi Flink+Paimon and how Paimon helps improve business efficiency.
 ### Speakers: 
 <img src="https://sessionize.com/image/110c-400o400o1-wtyHF2drG5sPmRkdsfAkgH.jpg" width="200" /><br>Shengjie Wang: Xiaomi Computing Engine R&D Engineer , Xiaomi Computing Engine R&D Engineer. Responsible for the development of computing engine
 <br><br>