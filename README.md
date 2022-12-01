<h1 align="center">
:oncoming_taxi: 
# Taxi-Service
:oncoming_taxi:
</h1>

:pushpin: 
## <u>Description</u> 
> A simple web application that is designed according to SOLID principles 
> and supports authentication and other CRUD operations.
___

### <u>Content</u>

<p>
* <a href="#-features">Features</a></br>
* <a href="#-project-structure">Project structure</a></br>
* <a href="#-technologies">Technologies</a></br>
* <a href="#-instructions">Instructions</a></br>
</p>

___

:star:
### <u>Features</u>
* authentication like a driver
* displaying cars list for the authenticated driver
* creating a driver/car/manufacturer
* updating a driver/car/manufacturer
* adding new drivers to the car
* displaying list of all drivers/cars/manufacturers
* soft deletion a driver/car/manufacturer
___

:derelict_house:
### <u>Project structure</u>
Application is divided into logical layers in accordance with N-tier architecture to separate responsibilities 
and manage dependencies in project.

| Tier         | Responsibility                                                              |
|--------------|:----------------------------------------------------------------------------|
| Presentation | Uses Apache Tomcat as the web server and Controllers to interact with users |
| Logic        | Uses Services to perform data processing of an application                  |
| Data         | Uses DAOs to perform CRUD operations                                        |

<b><i>UML Diagram</i></b>

<img src="img/umlDiagram.png" alt="umlDiagram" width="500">

<b><i>DB Diagram</i></b>

<img src="img/dbDiagram.png" alt="dbDiagram" width="500">

___

:computer:
### <u>Technologies</u>
* JDK 11
* Maven 4.0.0
* MySql 8.0.30
* JDBC
* Dependency Injection
* Java Servlet 4.0.1
* Tomcat 9.0.50
* JSP
* JSTL 1.2
* HTML, CSS
___

:hammer_and_wrench:
### <u>Instructions</u>
1. Install [MySQL](https://dev.mysql.com/downloads/installer/) 
and [Apache Tomcat](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/) if it's needed.
2. Clone this project from GitHub.
3. Create a schema using `ini_db.sql` file in `src\main\resources`.
4. Change URL, username, password and JDBC driver in `\src\main\java\taxi\util\ConnectionUtil.java`.
5. Configure Tomcat server :
   * Press *Edit configuration*;
   * Choose *Tomcat Server (Local)*;
   * Go to *Deployment* 
     * *Add -> Artifact -> taxi-service:war exploded*
     * *Application context -> /*
   * Press *Ok*.
6. Run the application.


GOOD LUCK ! :rocket:
