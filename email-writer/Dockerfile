# Java 17 (Render compatible)
FROM eclipse-temurin:17-jdk

# App directory
WORKDIR /app

# Copy all files
COPY . .

# Build Spring Boot jar
RUN ./mvnw clean package -DskipTests || mvn clean package -DskipTests

# Render exposes dynamic port
EXPOSE 8080

# Run application
CMD ["sh", "-c", "java -jar target/*.jar"]
