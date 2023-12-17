# spring-boot
Spring Boot learning
1. install JDK (e.g. version 21)
2. install maven 3.9.6
   a. download apache-maven-3.9.6-bin.tar.gz
   b. extract file (tar -xf apache-maven-3.9.6-bin.tar.gz)
   c. add in PATH (apache-maven-3.9.6/bin)
   d. check successful install (mvn -version) 
3. Download code (src and pom.xml) in your local system's directory (spring-work)
4. cd spring-work
5. run and verify
   a. execute mvn spring-boot:run
   b. server should be run successfully
   c. http://localhost:8080 [GET]
     i. output :- Greetings from Spring Boot!
   d. http://localhost:8080/actuator/health [GET]
     i. output :- {"status": "UP"}
6. Happy Learning
