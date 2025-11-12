# Base image (LTS OpenJDK 21, slim variant)
FROM eclipse-temurin:21-jdk

# Set artifact path (from Maven/Gradle target)
ARG artifact=target/app.jar

# Working directory inside container
WORKDIR /opt/app

# Copy built JAR file into image
COPY ${artifact} app.jar

# Default entrypoint to run the app
ENTRYPOINT ["java", "-jar", "app.jar"]
