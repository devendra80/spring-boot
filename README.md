# spring-boot
Spring Boot learning
1. Refer https://github.com/devendra80/spring-boot/blob/first-basic-web-app for JDK and MAVEN requirements
2. You can create Spring Boot project or jump to step#3
   a. go to https://start.spring.io
   b. Add dependencies
     i.  web
     ii. actuator
     iii.jpa
     iv. h2
   c. Generate project
   d. Extract it for use else refer step#3  
3. Download code (src and pom.xml) in your local system's directory (spring-work)
4. cd spring-work
5. Run application
   a. execute mvn spring-boot:run
   b. server should be run successfully
6. Verify application
   a. from windows PC
     i.  curl -X GET http://localhost:8080/clients
     ii.  curl -X GET http://localhost:8080/clients/1
     iii.  curl -X POST http://localhost:8080/clients --header "Content-Type: application/json" -d "{\"name\": \"John Doe\", \"email\": \"john.doe@baeldgung.com\"}"
     iv.  curl -X PUT http://localhost:8080/clients/1 --header "Content-Type: application/json" -d "{\"name\": \"John Doe2\", \"email\": \"john.doe@baeldgung.com\"}"
     v.  curl -X DELETE http://localhost:8080/clients/1
   b. from data file (client.json)
     i.  curl -X POST http://localhost:8080/clients -H "Content-Type: Application/json" -d @"C:\Users\data\client.json"
   c.  from other OS (not tested)
     i.  curl -X POST http://localhost:8080/clients --header "Content-Type: Application/json" -d '{"name": "John Doe", "email": "john.doe@baeldgung.com"}' 
   
7. Happy Learning
