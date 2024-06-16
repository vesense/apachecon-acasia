---
title: "Recognize, Reconcile, Repeat: The Path to Uniform Replicas in Apache Ozone"
date: "2024-07-27 16:45:00" 
track: "datastorage"
presenters: "Ethan Rose,Ritesh Shukla"
stype: "English Session"
---
Faults in distributed systems often are unbounded. Apache Ozone needs to be resistant to faults and preserve the durability and consistency of data in the face of these faults. Reconciliation is a new feature being developed that allows Ozone to recover from faults independent of how they occurred as well as the duration between faults. Reconciliation allows peers to identify, report, and resolve discrepancies of any type, and works across data durability models such as replication as well as erasure coding. The system can initiate and complete this process without admin intervention. This talk will cover the motivation behind replica reconciliation, the general strategy that can be applied to any storage system, and the implementation details that make it possible.
 ### Speakers: 
 <img src="https://sessionize.com/image/750e-400o400o1-n6M4nqrtxwshrQHLRedJjt.jpg" width="200" /><br>Ethan Rose: Senior Software Engineer at Cloudera, Apache Ozone PMC Member, Ethan is an engineer on Cloudera's Storage team, where he splits his time between Ozone development with the open source community and helping new users onboard Ozone into production. He has a B.S. in Computer Science from Rensselaer Polytechnic Institute.
 <br><br><img src="https://sessionize.com/image/8296-400o400o1-Njj22QN2B89Sv2EsqnYVby.png" width="200" /><br>Ritesh Shukla: Cloudera, Principal Engineer, Ritesh is an Apache Ozone PMC.  He has over a decade of experience with distributed storage solutions and systems. He is passionate about picking all three in a solution:  simple, right, and efficient. He is currently working on Ozone, a distributed object store that caters to HDFS and S3 workloads.
 <br><br>