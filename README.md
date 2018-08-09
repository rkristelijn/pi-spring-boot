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
| Starter templates and scaffolding     | angular/cli, vue/cli, yeoman     |   IDE, start.spring.io |
| Testing framework | Moocha | junit? |

# What do we Need
- Java (latest) - JRE 1.8.0 is already installed
- Maven (latest)
  - `sudo apt-get install maven`
- Web Server
- IDE such as IntelliJ or Spring STS
  - `sudo apt-get install eclipse` -> eclipse will appear in start menu
  - Eclipse Marketplace
    - Menu:help Install New Software, 
    - Work With: --All Available Sites--
    - type filet text: `marketplace`
    - Flag: `Marketplace Client`
    - click Next, Next, Accept, Finish, Trush Certificate, Ok, restart now (eclipse)
  - STS
    - Menu:help Eclipse market place
    - find: `sts`, go
      - Sprint Tools (aka Spring IDE ans Spring Tools Suite)
- MySQL
  - `sudo apt-get install mysql-server mysql-client`
  - after that you can connect using `sudo mysql -u root`
  - not sure why [this](https://stackoverflow.com/questions/10895163/how-to-find-out-the-mysql-root-password) doesn't work and `mysql -u root -p` doesn't work as well.
