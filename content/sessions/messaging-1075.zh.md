---
title: "AMQP在火箭mq实践"
date: "2024-07-26 14:30:00" 
track: "messaging"
presenters: "Le Zhang"
stype: "中文演讲"
---
AMQP协议是消息中间件领域的标准应用层协议。凭借其悠久的历史、活跃的社区、丰富的生态、全覆盖的多语言SDK等优势，它已经成为使用最广泛的标准消息协议之一，直到今天，Kafka、RocketMQ等。目前，分布式消息队列产品非常流行，但在消息传递领域仍然占有一席之地，被用户广泛采用。

但是由于历史原因，目前RabbitMQ的开源实现存在架构上的局限性，导致在性能、可扩展性、可维护性、可扩展性等方面存在一定的不足。作为一个经过验证的分布式消息中间件，Apache RocketMQ基于Apache RocketMQ，兼容AMQP 0.9.1协议，为已经使用AMQP协议和旧系统升级的用户提供更可靠、易于操作和高性能的消息中间件解决方案。

本演讲主要讲述了基于Apache RocketMQ实现兼容AMQP协议的技术体系结构和关键技术，包括以下几个部分:
1. AMQP开源产品RabbitMQ的架构
2. AMQP对RocketMQ的总体架构设计
3. RocketMQ上AMQP的关键技术要点
4. AMQP在RocketMQ上的功能和性能比较
5. RocketMQ上的AMQP开源
 ### Speakers: 
 <img src="https://sessionize.com/image/5c07-400o400o1-3zbmvi3e9RxK9W3Cwd56qJ.jpg" width="200" /><br>Le Zhang: 腾讯技术专家, 我目前就职于腾讯云，负责消息队列和微服务相关的系统研发。我在中间件领域工作了10年。我也是一个开源社区的爱好者，也是Apollo & Spring Cloud腾讯的创始人。
 <br><br>