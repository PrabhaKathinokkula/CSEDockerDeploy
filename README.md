# Automated CI/CD Pipeline for Spring Boot Application

## Overview

This project demonstrates an automated CI/CD pipeline for a Spring Boot application using Jenkins, Maven, SonarQube, Docker, Docker Hub, and AWS EC2.

The pipeline automates the application build, unit testing, code-quality analysis, Docker image creation, Docker Hub publishing, and deployment to an AWS EC2 instance.

## Technologies Used

- Java / Spring Boot
- Maven
- Jenkins
- SonarQube
- Docker
- Docker Hub
- AWS EC2
- Git
- GitHub

## CI/CD Pipeline

The Jenkins pipeline performs the following stages:

1. **Clone Code** - Clones the Spring Boot application from GitHub.
2. **Install Dependencies** - Installs project dependencies using Maven.
3. **Unit Testing** - Executes automated unit tests and publishes test results.
4. **SonarQube Analysis** - Performs automated code-quality analysis using SonarQube.
5. **Build JAR** - Packages the Spring Boot application as a JAR file.
6. **Build Docker Image** - Creates a Docker image for the application.
7. **Push Image to Docker Hub** - Publishes the Docker image to Docker Hub.
8. **Deploy to AWS EC2** - Pulls the Docker image and deploys the container on an AWS EC2 instance.

## Pipeline Workflow

GitHub
   ↓
Jenkins
   ↓
Maven Dependencies
   ↓
Unit Testing
   ↓
SonarQube Analysis
   ↓
Build JAR
   ↓
Build Docker Image
   ↓
Push Image to Docker Hub
   ↓
Deploy to AWS EC2
