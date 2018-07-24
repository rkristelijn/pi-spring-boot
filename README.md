# pi-spring-boot
Tutorial on setting up a simple Spring Boot (Java Web) project on a Rapsberry Pi

# Raspbian
I have downloaded the Raspberry Pi Desktop [2018-06-27-rpd-x86-stretch.iso](http://downloads.raspberrypi.org/rpd_x86/images/) and installed it using VirtualBox on my laptop. Then I used the out of the box cd mount for the guest additions to fully utalize the screen resources. `sudo sh /media/cdrom/VBoxLinuxAdditions.run` and reboot.

# What is what

## Spring Boot

### BUILD ANYTHING

Spring Boot is designed to get you up and running as quickly as possible, with minimal upfront configuration of Spring. Spring Boot takes an opinionated view of building production ready applications.

Spring Boot is the starting point for building all Spring-based applications. Spring Boot is designed to get you up and running as quickly as possible, with minimal upfront configuration of Spring.

- Get started in seconds using Spring Initializr
- Build anything - REST API, WebSocket, Web, Streaming, Tasks, and more
- Simplified Security
- Rich support for SQL and NoSQL
- Embedded runtime support - Tomcat, Jetty, and Undertow
- Developer productivity tools such as live reload and auto restart
- Curated dependencies that just work
- Production-ready features such as tracing, metrics and health status
- Works in your favorite IDE - Spring Tool Suite, IntelliJ IDEA and NetBeans

### Comparing to Node

| _        | Node           | Spring Boot  |
| ------------- |:-------------:| -----:|
| Dependancy Management     | package.json | pom.xml |
| Dependancy Manager      | NPM      |   Maven |
| Web Server      | express, webpack      |   Tomcat (by Spring Boot) |
| Starter templates      | angular/cli, vue/cli, yeoman     |   IDE, start.spring.io |

# What do we Need
- Java (latest)
- Maven (latest)
- Web Server
- IDE such as IntelliJ or Spring STS
- MySQL
