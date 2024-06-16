---
title: "在GraalVM静态编译下实现Tomcat应用程序的自动可观察性"
date: "2024-07-28 15:45:00" 
track: "webserver"
presenters: "Zihao Rao"
stype: "中文演讲"
---
GraalVM静态编译在提高Tomcat web应用程序启动速度和运行时内存使用方面有显著的效果。它在云原生生态系统中蓬勃发展是非常有价值的。但是，最初基于Java Agent提供的自动检测将在静态编译后失效。我们的团队在GraalVM中设计了一个静态仪表解决方案来解决上述问题(https://github.com/oracle/graal/pull/8077)。本次讲座将介绍以下两个部分:
1. 解决方案的总体设计思想。
2. 该解决方案的测试结果为Tomcat web应用在Otel Java Agent上。
 ### Speakers: 
 <img src="https://sessionize.com/image/3b4b-400o400o1-nRaiucVbHuuLNGZw1JCsDc.jpg" width="200" /><br>Zihao饶: 南, 热爱开源, 热情的开源贡献者

阿里云智能研发工程师
Spring-Cloud 阿里指导委员会成员(https://github.com/alibaba/spring-cloud-alibaba)
OpenTelemetry Java Instrumentation Triager
https://github.com/steverao

我还作为演讲者参加了一些开源峰会，如ApacheCon Asia 2022 (https://apachecon.com/acasia2022/sessions/webserverandtomcat-1079.html)

社区代码2023 (https://tomcat.apache.org/presentations.html)
 <br><br>