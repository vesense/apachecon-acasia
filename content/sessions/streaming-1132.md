---
title: "How we use Reclaimed Low-Cost Computing Resouces for Large-Scale Near-Line Model Inference"
date: "2024-07-27 16:45:00" 
track: "streaming"
presenters: "Yun Tang"
stype: "Chinese Session"
---
Due to the increasing value of GPU resources, we have restructured Xiaohongshu's image search system to create a near-line/offline inference pipeline, ultimately developing a high-quality cost-saving and efficiency-improving solution that utilizes idle computing resources to handle billions of data-scale model inference tasks:

In the transient and easily evictable resource pool with tidal characteristics, we have set up a virtualized k8s cluster to enable the submission of Flink jobs.
Collaborating with the business team, we simplified the complex inference pipeline of the image search system, which previously consisted of over 10 microservices, into a few PyFlink jobs.
Since CPU-based inference is much slower than traditional data processing in the BI domain, the native checkpoint mechanism of Flink is no longer suitable. We combined an adaptive scheduler with customized fault-tolerance mechanisms to ensure stable and continuous operation on transient resources.
In the end, we significantly improved the efficiency and stability of the image search data pipeline while saving hundreds of thousands of core·days of fixed resources. Thanks to Flink's integrated streaming and batch processing features, the entire pipeline also unified the near-line and offline inference paths for business needs, achieving successful implementation in other areas such as transactions and community algorithms. In the future, we also consider integrating the inference ability with Ray to support wider usage scenarios.
 ### Speakers: 
 <img src="https://sessionize.com/image/4849-400o400o1-LRkj3zMXkm7teij1dkn5Bs.jpg" width="200" /><br>Yun Tang: Streaming engine Tech leader at Xiaohongshu, Yun Tang, I have over 10 years of experience in developing and researching big data systems, with a primary focus on real-time computing (from Spark Streaming to Flink). I joined Alibaba Cloud in 2017, working on Flink-related development tasks such as state management, fault tolerance, and ecosystem integration, and became a committer in the Flink community. In 2022, I joined Xiaohongshu as the leader of the real-time computing team, responsible for driving the adoption of integrated streaming and batch processing scenarios, as well as implementing near-line/offline machine learning inference solutions within the company. I am also exploring distributed computing systems like Ray.
 <br><br>