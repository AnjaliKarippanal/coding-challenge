## Project Name
**Carpark Ubi Application**

## Project Description:
Carpark Ubi Application is a prototype developed using Spring Boot REST CRUD JPA Project with Thymeleaf User interface with an intension to identify and allocate fast and slow charging port using a web user interface which is managed by RestAPI Controller.

## Features/Highlights of the CarparkUbi Application:
1. An application with web interface which has hosted on http://localhost:8081 (server port can be changed in application.properties)
2. Application developed with a requirement of 10 charging points
3. User can choose either 20 Amperes (fast charging) or 10 Amperes (slow charging) through web UI when a car connects
4.	Total input capacity of CarparkUbiApplication = 100 Amperes, so combination of inputs can be;
    a.5 cars with 20 Amperes or;
    b.10 cars with 10 Amperes or
    c.mix of both fast and slow charging cars but limited total current input to 100 Amperes.
5.	A charge point notifies the application when a car is plugged (status: available) or unplugged (status: occupied)
6.	If total capacity reaches 100 A and if a new user comes (high priority), then any of the fast-charging cars which connected earlier (low priority) will automatically assign to slow charging.
7.	The application also has feature implemented by providing a report with a current state of each charging point returning a list of charging point, status (Available or Occupied) and - if occupied – the consumed current


## Technology
1.	Java 1.8
2.	Spring Boot 2.7.1
3.	Eclipse IDE 2020-09 (4.17.0)
4.	MySQL Work bench 8.0
5.	Sprint Tool 3 Eclipse Addon


## Pre requisite 
1.	Change DB connection in Application.properties according to your Data base credentials
      ![image](https://user-images.githubusercontent.com/47337076/176393127-9cdfc1cf-4220-475a-a8b1-63c1d7809522.png)

2.	SQL file for creating cp_tracker schema and tables such as chargingpoint, customers can be found in project folder. (path: src/main/resources/sql)

Additionally, all other dependencies such as sprint-boot-starter-web, sprint-boot-starter-data-jpa, sprint-boot-starter-thymeleaf, mysql-connected-java etc are defined in pom.xml

## How to Run the project
1.	Download the project from GitHub location
2.	Import as Maven project in Eclipse IDE
3.	Do all the pre-requisite validation
4.	Run as sprint boot application
5.	Start Rest Controller using http://localhost:8081 (url)
6.	Also suggest to refer user manual for user scenario

## Sample output:

![image](https://user-images.githubusercontent.com/47337076/176395019-714a27a8-0393-4507-a76b-2ba94180276e.png)

## Design
<to be updated>
