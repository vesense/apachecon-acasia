---
title: "Mixing Stream and Batch Processing in Apache Flink"
date: "2024-07-26 15:45:00" 
track: "streaming"
presenters: "Xuannan Su"
stype: "Chinese Session"
---
For a long time, stream processing and batch processing have been the two distinct modes of large-scale data processing. With the development of unified stream and batch processing, Apache Flink now allows both to be managed within a single engine. This blurs the distinction between stream and batch processing, giving rise to a new unified data processing mode, known as mixed mode. In this mixed mode, users are not burdened with the need to pre-determine the execution mode for their Flink jobs. Instead, Flink adaptively chooses and switches between execution modes based on data freshness requirements to effectively balance latency and throughput.
During this talk, we will discuss the concepts and advantages of mixed mode and introduce the attendant technical challenges and design solutions. We will demonstrate how the mixed mode enhances throughput by more than 50% in various use cases. Additionally, we will cover the latest developments and outline the future plans of the Flink community in this domain.
 ### Speakers: 
 <img src="https://sessionize.com/image/6797-400o400o1-dbccedf4-ca5c-4ac7-9407-da8d909f00a6.jpg" width="200" /><br>Xuannan Su:  Alibaba Group, Xuannan is a software engineer at Alibaba. He is focusing on the development of Apache Flink runtime.
 <br><br>