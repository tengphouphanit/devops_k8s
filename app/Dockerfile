# Base image 
FROM openjdk

# setting artifact path
ARG artifact=target/app.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Entrypoint for running app
ENTRYPOINT ["java","-jar","app.jar"]