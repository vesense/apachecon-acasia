---
title: "Implement automatic observability of Tomcat applications under GraalVM static compilation"
date: "2024-07-28 15:45:00" 
track: "webserver"
presenters: "Zihao Rao"
stype: "Chinese Session"
---
GraalVM static compilation has a significant effect on improving Tomcat web application startup speed and runtime memory usage. It is very valuable for it to flourish in Cloud Native ecosystem. However, the automatic instrumentation originally provided based on Java Agent will become invalid after static compilation. Our team designed a static instrumentation solution in GraalVM to solve above problem (https://github.com/oracle/graal/pull/8077). This talk will introduce following two parts:
1. The overall design idea of the solution.
2. The test results of this solution for Tomcat web application in Otel Java Agent.
 ### Speakers: 
 <img src="https://sessionize.com/image/3b4b-400o400o1-nRaiucVbHuuLNGZw1JCsDc.jpg" width="200" /><br>Zihao Rao:  Passionate about Opensource, Passionate open source contributor=

Alibaba Cloud intelligent R&D engineer
Steering Committee Member of Spring Cloud Alibaba (https://github.com/alibaba/spring-cloud-alibaba)
OpenTelemetry Java Instrumentation Triager
https://github.com/steverao

I also as a speaker to participate in some Open Source summits, such as ApacheCon Asia 2022 (https://apachecon.com/acasia2022/sessions/webserverandtomcat-1079.html)
Community Over Code 2023 (https://tomcat.apache.org/presentations.html)
 <br><br>