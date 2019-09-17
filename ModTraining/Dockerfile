FROM openjdk:latest

# Add Maintainer Info
MAINTAINER Kajal Korde <kajal.korde@cognizant.com>

# Add a volume pointing to /tmp
VOLUME /tmp

ADD target/ModTraining.jar ModTraining.jar

# Make port 8083 available to the world outside this container
EXPOSE 8084

# The application's jar file
ARG JAR_FILE=target/ModTraining.jar-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
ADD ${JAR_FILE} ModTraining.jar.jar

# Run the jar file 
ENTRYPOINT ["java","-jar","ModTraining.jar"]