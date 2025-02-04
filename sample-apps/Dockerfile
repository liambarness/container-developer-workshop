FROM openjdk:11.0-jdk
WORKDIR /app

COPY java/hello-world-maven /app

WORKDIR /app
RUN ./mvnw clean compile assembly:single

CMD ["java", "-jar", "/app/target/sample-app-1.0.0-jar-with-dependencies.jar"]