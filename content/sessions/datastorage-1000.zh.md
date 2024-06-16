---
title: "降低ByteDance中SparkSQL计算成本的优化"
date: "2024-07-27 14:30:00" 
track: "datastorage"
presenters: "甘红楠"
stype: "中文演讲"
---
字节跳动使用SparkSQL作为ETL的主要工具之一。通过对在线任务的分析，我们发现导致Spark作业性能下降的主要因素有三个:对大量数据进行变换、扫描大量小文件和低效的推测执行。对大量数据进行Shuffle处理可能会导致网络拥塞、IO瓶颈等问题，影响Shuffle服务的稳定性。读取大量小文件会增加数据传输开销和内存使用。低效的推测执行经常启动和终止备份任务，浪费集群资源并影响其他任务的调度。这些因素显著增加了计算成本。

我们使用两种主要技术优化Shuffle: bucket和ZSTD Shuffle。首先，我们基于开源的SparkSQL显著增强了Bucket优化。这包括覆盖更多的Exchange消除场景、改进可用性和提高适应性。我们还构建了一个Bucket推荐系统来自动识别哪些表可以在转换为Bucket时减少Shuffle数据。在ODS场景下，推荐的Bucket优化可以减少多达99.9%的Shuffle数据，节省高达58%的计算资源。其次，我们将Shuffle数据的压缩算法从LZ4改为ZSTD，压缩比明显提高，减少了40%以上的Shuffle数据。

我们设计并实现了一个基于shuffle的小文件整合功能，以防止小文件的生成，从而消除了下游任务扫描大量小文件的需要。该功能通过在写入表之前引入Shuffle并控制Shuffle并行性来实现文件整合，从而避免了二次HDFS读写操作。此外，我们利用AQE (Adaptive Query Execution)框架来优化Shuffle Read，防止数据倾斜。

为了缓解投机执行效率低下造成的问题，我们首先分析了所有在线任务的配置文件，发现为投机执行而启动的大量任务最终被终止，导致相当大的集群资源浪费。随后，我们引入了Efficient Speculation optimization，根据数据处理的速度来决定是否发起投机执行，从而避免了由于数据倾斜而发起投机执行(因为投机执行无法解决这种情况)。最后，我们适当提高了投机执行的启动阈值，进一步减少了投机执行造成的计算资源浪费。优化后，推测执行任务数量减少了15%，计算资源消耗减少了9%。
 ### Speakers: 
 <img src="https://sessionize.com/image/c52a-400o400o1-fqHUaN3MbFjUnx1NxULM9c.jpg" width="200" /><br>甘红楠: 字节跳动高级研发工程师，字节跳动高级研发工程师, 
 * 复旦大学学士、硕士学位 
 * SparkSQL内核开发者ByteDance
 * 对SQL优化感兴趣
 <br><br>