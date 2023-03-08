
FROM tomcat:9.0-alpine
FROM maven:3.3-jdk-8
WORKDIR /app
ADD pom.xml /app
RUN mvn clean install
ADD app/target/App42PaaS-Java-MySQL-Sample-0.0.1-SNAPSHOT.war webapps/
s