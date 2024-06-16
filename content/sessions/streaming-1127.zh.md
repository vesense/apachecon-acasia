---
title: "基于字节跳动的Flink SQL性能优化的探索与实践。"
date: "2024-07-27 14:00:00" 
track: "streaming"
presenters: "李精卫"
stype: "中文演讲"
---
随着内部对字节流任务的需求日益增长，Flink SQL的大规模实现已经在多个部门中变得越来越普遍。Flink SQL作为一个经济高效的切入点，已经看到流SQL任务的规模提升到超过30K，而任务资源利用率已经达到数百万核。在公司强调降低成本和提高效率的同时，我们在查询优化和查询执行方面进行了大量的性能增强。字节跳动中的这些广泛实现使CPU使用量减少了大约17%。
在本演示中，我们将详细概述在ByteDance中执行的主要优化和实现的结果。
1. 背景
-当前状态的Flink流SQL在字节跳动
-面临的挑战
2. Flink SQL的深度优化
-查询优化
-查询执行
——其他
3. 实现和收益
4. 未来的计划
——探索更多优化方向
 ### Speakers: 
 <img src="https://sessionize.com/image/3f4c-400o400o1-HTgxt2UDHFRHpeKTQSChv5.jpg" width="200" /><br>李精卫: 字节跳动基础架构工程师，目前主要负责字节跳动Flink SQL相关的工作
 <br><br>