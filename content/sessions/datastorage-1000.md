---
title: "Optimization for Reducing Compute Cost of SparkSQL in ByteDance"
date: "2024-07-27 14:30:00" 
track: "datastorage"
presenters: "Hongnan Gan"
stype: "Chinese Session"
---
ByteDance employs SparkSQL as one of the primary tools for ETL. Through analysis of online tasks, it was discovered that three major factors contribute to the degradation of Spark job performance: shuffling large volumes of data, scanning numerous small files, and inefficient speculative execution. Shuffling large volumes of data may lead to issues such as network congestion, IO bottlenecks, and affecting the stability of the Shuffle Service. Reading numerous small files increases data transmission overhead and memory usage. Inefficient speculative execution frequently initiates and kills backup tasks, wasting cluster resources and impacting the scheduling of other tasks. These factors significantly increase computational costs. 

We optimized Shuffle using two main techniques: Bucketing and ZSTD Shuffle. Firstly, we significantly enhanced Bucket optimization based on the open-source SparkSQL. This includes covering more Exchange elimination scenarios, improving usability, and becoming more adaptive. We also constructed a Bucket recommendation system to automatically identify which tables could reduce Shuffle data when converted to Bucket. In ODS scenarios, the recommended Bucket optimization can reduce Shuffle data by up to 99.9% and save up to 58% of computational resources. Secondly, we changed the compression algorithm of Shuffle data from LZ4 to ZSTD, resulting in a noticeable increase in compression ratio, reducing Shuffle data by over 40%.

We designed and implemented a Shuffle-based small file consolidation feature to prevent the generation of small files, thereby eliminating the need for downstream tasks to scan numerous small files. This functionality achieves file consolidation by introducing a Shuffle before writing to the table and controlling Shuffle parallelism, thereby avoiding secondary HDFS read-write operations. Additionally, we utilized the AQE (Adaptive Query Execution) framework to optimize Shuffle Read, preventing data skew.

To mitigate the issues caused by inefficient speculative execution, we first analyzed the profiles of all online tasks and found that a significant number of tasks initiated for speculative execution were ultimately terminated, resulting in considerable waste of cluster resources. Subsequently, we introduced Efficient Speculation optimization, which determines whether to initiate speculative execution based on the speed of data processing, thereby avoiding speculative execution initiation due to data skew (as speculative execution cannot address such cases). Finally, we appropriately increased the threshold for initiating speculative execution, further reducing the waste of computational resources caused by speculative execution. After optimization, the number of speculative execution tasks decreased by 15%, and computational resource consumption decreased by 9%.
 ### Speakers: 
 <img src="https://sessionize.com/image/c52a-400o400o1-fqHUaN3MbFjUnx1NxULM9c.jpg" width="200" /><br>Hongnan Gan:  ByteDance Senior R&D Engineer,
* BS and MEng Degree of Fudan University
* SparkSQL kernel developer in ByteDance
* Interested in SQL optimizing
 <br><br>