
Description
This project is a Spring Boot application designed to demonstrate the use of JPA (Java Persistence API) with named queries. It focuses on modeling a simple music library where albums, artists, and songs are represented as entities with relationships between them. The project showcases how to perform CRUD operations and manage these relationships using Spring Data JPA.

Technologies Used
Java 11: The programming language used for this project.
Spring Boot: Framework to simplify the creation of Java applications.
Spring Data JPA: Used for data access and ORM (Object-Relational Mapping).
Lombok: Reduces boilerplate code by generating commonly used methods like getters, setters, equals, hashcode, etc., at compile time.
H2 Database: An in-memory database used for testing.
Project Structure
Model: Contains the entity classes Album, Artist, and Song which represent the tables in the database and define relationships between them.
Repository: Contains the repository interfaces AlbumRepository, ArtistRepository, and SongRepository, which extend JpaRepository to provide CRUD operations.
Service: Contains the AlbumService class that handles business logic related to albums and songs.
Application: The App class serves as the entry point to the Spring Boot application.
Installation Instructions
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/SPR-CL-NAMEDQUERIES.git
Navigate to the project directory:
bash
Copy code
cd SPR-CL-NAMEDQUERIES
Build the project using Maven:
bash
Copy code
mvn clean install
Usage
Running the application:

You can run the application using Maven:
bash
Copy code
mvn spring-boot:run
Alternatively, you can build a JAR and run it:
bash
Copy code
mvn package
java -jar target/spr-cl-namedqueries-0.1.jar
Accessing the application:

The application runs on http://localhost:8080 by default.
Interacting with the H2 Database:

You can access the H2 database console at http://localhost:8080/h2-console. The default credentials and JDBC URL can be found in the application.properties file.
Features
CRUD Operations: Perform Create, Read, Update, and Delete operations on Album, Artist, and Song entities.
Relationships: Demonstrates many-to-one and one-to-many relationships between entities.
Service Layer: Provides methods for adding albums, retrieving all albums, and adding songs to an album.
Future Improvements
Add more complex queries and functionality.
Implement more RESTful endpoints for interacting with the application.
Add unit and integration tests for the service and repository layers.
License
This project is licensed under the MIT License. See the LICENSE file for details.
