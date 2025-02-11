# Enterprise Microservices Application

## Architecture Overview

This is a comprehensive microservices application leveraging:

- Spring Boot
- Spring Cloud
- Java Enterprise Edition (JEE)
- Angular 4
- Web Services
- PL/SQL
- Microservices Architecture

### System Components

1. **Backend Microservices**
   - Config Server
   - Eureka Service Discovery
   - API Gateway
   - Authentication Service
   - Book Service
   - User Service
   - Notification Service

2. **Frontend**
   - Angular 4 Single Page Application (SPA)
   - Responsive Design
   - State Management
   - Reactive Programming

3. **Database**
   - Oracle 19c
   - PL/SQL Stored Procedures
   - Complex Queries and Transactions

4. **DevOps**
   - Docker Containerization
   - Kubernetes Orchestration
   - CI/CD Pipeline

## Technical Architecture

### Backend Technologies

- Spring Boot 2.6.x
- Spring Cloud (Gateway, Config, Eureka)
- Spring Security with JWT
- Hibernate/JPA
- Swagger/OpenAPI Documentation
- Actuator for Monitoring

### Frontend Technologies

- Angular 4
- RxJS
- NgRx State Management
- Angular Material
- Responsive Design
- Lazy Loading

### Database Design

- Normalized Relational Schema
- PL/SQL Stored Procedures
- Oracle 19c Enterprise Features

## Getting Started

### Prerequisites

- Java 11+
- Node.js 14+
- Angular CLI
- Docker
- Oracle Database

### Installation Steps

1. Clone the Repository
2. Build and Run the Backend Services
3. Build and Run the Frontend Application
4. Configure the Database

```bash
git clone https://github.com/yourusername/microservices-app.git
cd microservices-app

# Build Config Server
cd backend/config-server
./mvnw clean install

# Build Eureka Server
cd ../eureka-server
./mvnw clean install

cd frontend/angular-app
npm install
ng serve
-- Connect to Oracle
sqlplus / as sysdba

-- Create Application Schema
CREATE USER microservices IDENTIFIED BY password;
GRANT ALL PRIVILEGES TO microservices;

-- Run initialization scripts
@database/plsql-scripts/init.sql
@database/plsql-scripts/create_tables.sql

docker-compose up --build

Microservices Communication
Service Discovery: Eureka
Configuration Management: Spring Cloud Config
API Gateway: Spring Cloud Gateway
Inter-Service Communication: REST/gRPC
Circuit Breaker: Resilience4j
Security
JWT Authentication
Role-Based Access Control
OAuth2 Support
HTTPS Everywhere
Monitoring & Observability
Prometheus Metrics
Grafana Dashboards
Distributed Tracing with Zipkin
ELK Stack Logging
Deployment
Kubernetes Deployment
Helm Charts
Cloud-Native Ready (AWS/Azure/GCP)
Contributing
Fork the Repository
Create Feature Branch
Commit Changes
Push to Branch
Create Pull Request
License
MIT License

Contact
Yassine Benaich - yassine.benaich05@gmail.com

Project Link: https://github.com/itsRevanor97/microservices-app
