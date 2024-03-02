# Continuous Assessment-Spotify Clone Web


Prerequisites:
•	Intellij IDEA
•	MySQL DataBase Community Edition
•	Java Development Kit (JDK), version 1.8.
•	Apache Maven, version 3.0 or later.
•	Java Spring Boot 3.1.0
•	Docker Desktop

# Spotify-Clone Web Page 

•	Design Pattern
•	User Interface
•	Authentication and Security
•	Database
•	Services
•	Deployment of Docker & Kubernetes


# 2.1 Design Pattern:
In this project, I used Architectural Pattern there are some design pattern for example; Model-View-Controller (MVC),Service-Oriented Architecture (SOA),Dependency Injection (DI),Event-Driven Architecture (EDA) but I decided best one is Model-View-Controller (MVC) separates the application into three components: Model, View, and Controller. The Model represents the data and business logic, the View displays the user interface, and the Controller handles user input and coordinates interactions between the Model and View. This pattern promotes separation of concerns, modularity, and ease of maintenance.

# 2.2 User Interface
JSP (JavaServer Pages) is a technology used for creating dynamic web pages in Java. It allows embedding Java code within HTML pages to generate dynamic content that can be sent to the client browser. JSP is often used for building the user interface (UI) layer of Java web applications. Here's how JSP is used for UI development:

Combining Java and HTML: With JSP, you can write Java code directly within HTML pages. JSP files have a .jsp extension and contain both static HTML content and dynamic Java code enclosed within special tags. These tags allow you to embed Java expressions, declarations, scriptlets, and use control structures like loops and conditionals.
Dynamic Content Generation: JSP enables the dynamic generation of content based on server-side logic. You can use Java code to retrieve data from a database, perform calculations, or apply business logic. The results are then embedded within HTML tags or used to populate form fields, tables, or other UI components.

![image](https://github.com/emrah-uzdilli/spotifyCloneCCT/assets/62702253/d43f74aa-78dc-4da8-9052-7ea1b9966db1)

# 2.3 Authentication and Security
I prefer to write this project using java Spring boot because which provide us several mechanisms to enhance security when using JPA (Java Persistence API) for database interactions. Here are some ways to improve security in a Spring Boot application with JPA.Spring Security is a powerful framework 

# 2.4 Database
In this project I used MySQL Database system because MySQL is an open-source database, which means it is freely available for use. 
![image](https://github.com/emrah-uzdilli/spotifyCloneCCT/assets/62702253/1132389c-f713-4b44-ab3f-f010a3743f0d)

# 2.5 Services
There are 5 services;UserService,UserDetailsImpService,SongService,PlaylistService and Playlist_SongService.
 All of them have separate duties and the Services are able to communicate with each other.
 # 2.6 Deployment of Docker
End of this assignment, I will evaluate deeply Docker and Kubernetes which provides portability, scalability, efficiency, and automation. Also, we can make pods and we can run more than one services run at the same time. 
1.	Write Dockerfile Codes:
FROM openjdk:17-alpine
ARG JAR_FILE=target/*.jar
COPY ./target/Spotify-0.0.1-SNAPSHOT.jar app.jar
CMD ["java", "-jar", "/app.jar"]

2.	After Install Maven dependences created automatically under target folder these jar files.
   
