# Spring Boot Microservice HelloWorld

## Project Documentation

This document provides an overview of the setup instructions, Docker usage guide, and deployment steps on Render.com for the Spring Boot Microservice HelloWorld project.

### Setup Instructions
1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/blue-dio/springboot-microservice-helloworld.git
   cd springboot-microservice-helloworld
   ```
2. **Install Dependencies**:  
   Make sure you have [Java](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) and [Maven](https://maven.apache.org/download.cgi) installed. Then run:
   ```bash
   mvn install
   ```
3. **Run the Application**:  
   You can run the application using:
   ```bash
   mvn spring-boot:run
   ```

### Docker Usage Guide
1. **Build the Docker Image**:  
   Make sure you have Docker installed on your machine. From the root of the repository, run:
   ```bash
   docker build -t springboot-microservice-helloworld .
   ```
2. **Run the Docker Container**:  
   ```bash
   docker run -p 8080:8080 springboot-microservice-helloworld
   ```

### Deployment Steps on Render.com
1. **Create a New Web Service**:  
   Go to your Render.com dashboard and create a new web service.
2. **Connect Your Repository**:  
   Connect your GitHub account and select the `springboot-microservice-helloworld` repository.
3. **Select Build Command and Start Command**:  
   Use the following commands:  
   - Build Command: `mvn install`  
   - Start Command: `java -jar target/springboot-microservice-helloworld.jar`
4. **Configure Environment Variables**:  
   Add any required environment variables.
5. **Deploy**:  
   Click on the deploy button and your service will be up and running.

---  

This README will help you to set up and run the Spring Boot Microservice HelloWorld project efficiently.