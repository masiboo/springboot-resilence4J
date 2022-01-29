# springboot-resilence4J

To use resilience4j circuit breaker steps:-

1. We need dependency :-

       <dependency>
           <groupId>org.springframework.boot</groupId>
           <artifactId>spring-boot-starter-actuator</artifactId>
           <version>2.2.1.RELEASE</version>
       </dependency>
       <dependency>
           <groupId>io.github.resilience4j</groupId>
           <artifactId>resilience4j-spring-boot2</artifactId>
           <version>1.4.0</version>
       </dependency>
       <dependency>
           <groupId>org.springframework.boot</groupId>
           <artifactId>spring-boot-starter-aop</artifactId>
           <version>2.2.6.RELEASE</version>
       </dependency>

2. Configuration file application.yml

Then add annotation o the required external web service call.

For testing, we can check    

http://localhost:8080/actuator/health

Then we can stop and start service and monitor  
