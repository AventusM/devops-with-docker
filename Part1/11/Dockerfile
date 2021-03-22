# Java 8 required
FROM openjdk:8
EXPOSE 8080

WORKDIR /usr/src/app

# Copy all of the content from the project to the image workdirectory
COPY . /usr/src/app

# Build the project
RUN ./mvnw package

# Run the application
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]