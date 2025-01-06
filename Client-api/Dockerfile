# Use a minimal JDK base image
FROM openjdk:17-jdk-slim

# Set environment variables
ENV SPRING_PROFILES_ACTIVE=prod

# Copy the application JAR
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Expose the default port
EXPOSE 8084

# Run the application
ENTRYPOINT ["java", "-jar", "/app.jar"]