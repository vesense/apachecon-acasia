---
title: "Stability and Performance Optimization Practices of HBase at Xiaomi"
date: "2024-07-27 16:15:00" 
track: "datastorage"
presenters: "Yuting sun"
stype: "Chinese Session"
---
Background
This section will primarily introduce the current status and scale of HBase applications within Xiaomi, along with encountered challenges. Additionally, it will cover some internal optimization measures implemented and the benefits gained thereafter.
Approaches and Practices
2.1 Stability Practices
- Hotspot Region Handling
- Business hotspot requests leading to queue congestion, impacting read/write operations of other regions; addressing this by isolating hotspot regions onto nodes with lower loads.
- TPS Load Balancing
- Existing balance solutions not effectively handling sudden spikes in request volume, resulting in uneven TPS loads; introducing TPS load balancing to mitigate these issues in line with Xiaomi's internal usage scenarios.
- Accelerating Replay Data During Abnormal Restarts
- The node restarts abnormally, and the large number of WALs causes the playback of data to take a long time; reduce the number of playback WALs, speed up the data playback time, and optimize the time when the region does not provide services from 160s to 16s.
2.2 Performance Optimization Practices
- This section will focus on Xiaomi's internal considerations and implementation of a grouped thread model for HBase request queues, prioritizing requests to better meet internal business requirements.
2.3 Cross-Version Upgrades
- Highlighting Xiaomi's migration from version 0.98 to 2.x, including the background, process, encountered challenges, and corresponding solutions.
Summary and Future Planning
This section will primarily discuss Xiaomi's reflections on the future development of HBase and outline planned strategies to address upcoming challenges and requirements.
Listener benefit:
Through this sharing, you can gain an in-depth understanding of Xiaomi’s internal optimization solutions and methods for business usage scenarios, as well as practices to improve system stability and performance.
 ### Speakers: 
 <img src="https://sessionize.com/image/f58e-400o400o1-94JMLSeRT14HWn8mTYNdUm.png" width="200" /><br>Yuting sun: Storage R&D Engineer, Xiaomi software R&D engineer, mainly responsible for HBase development
 <br><br>