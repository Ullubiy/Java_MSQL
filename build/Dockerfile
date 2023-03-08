
FROM maven:3-jdk-7-alpine as build
COPY . ./
WORKDIR app
RUN mvn package

FROM tomcat:9.0-jre7-alpine
COPY --from=build /app/target/*.war /usr/local/tomcat/webapps/
EXPOSE 8080