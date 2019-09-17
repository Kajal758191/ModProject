FROM openjdk:latest

# Add Maintainer Info
MAINTAINER Kajal Korde <kajal.korde@cognizant.com>

# Add a volume pointing to /tmp
VOLUME /tmp

ADD target/ModMentor.jar ModMentor.jar

# Make port 8083 available to the world outside this container
EXPOSE 8082

# The application's jar file
ARG JAR_FILE=target/ModMentor.jar-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
ADD ${JAR_FILE} ModMentor.jar.jar

# Run the jar file 
ENTRYPOINT ["java","-jar","ModMentor.jar"]