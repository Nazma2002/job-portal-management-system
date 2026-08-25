# Job Portal Management System

A full-stack job portal web application built with **Java, Spring Boot, MySQL, and Thymeleaf**. It allows job seekers and recruiters to register, and supports creating, viewing, updating, and deleting job postings through both a REST API and a browser-based UI.

## Features

- Role-based user model (Job Seeker / Recruiter)
- Full CRUD REST API for job postings
- Server-side rendered UI (Thymeleaf) to view and add jobs
- Input validation with clean, structured error responses
- MySQL persistence via Spring Data JPA / Hibernate

## Tech Stack

- **Backend:** Java 17, Spring Boot, Spring Data JPA, Hibernate
- **Database:** MySQL
- **Frontend:** Thymeleaf, HTML, CSS
- **Build Tool:** Maven
- **Other:** Lombok, Jakarta Bean Validation

## Project Structure

## Getting Started

### Prerequisites

- Java 17+
- Maven (or use the included `mvnw` wrapper)
- MySQL Server running locally

### Setup

1. Clone the repository:

```bash
   git clone https://github.com/Nazma2002/job-portal-management-system.git
   cd job-portal-management-system
```

2. Create a MySQL database:

```sql
   CREATE DATABASE jobportal_db;
```

3. Update `src/main/resources/application.properties` with your MySQL credentials:

```properties
   spring.datasource.url=jdbc:mysql://127.0.0.1:3306/jobportal_db
   spring.datasource.username=root
   spring.datasource.password=YOUR_PASSWORD
```

4. Run the application:

```bash
   ./mvnw spring-boot:run
```

5. Open your browser:
   - UI: `http://localhost:8080/jobs`
   - API: `http://localhost:8080/api/jobs`

## API Endpoints

| Method | Endpoint              | Description          |
| ------ | --------------------- | -------------------- |
| GET    | `/api/jobs`           | Get all job postings |
| GET    | `/api/jobs/{id}`      | Get a job by ID      |
| POST   | `/api/jobs`           | Create a new job     |
| PUT    | `/api/jobs/{id}`      | Update a job         |
| DELETE | `/api/jobs/{id}`      | Delete a job         |
| GET    | `/api/users`          | Get all users        |
| POST   | `/api/users/register` | Register a new user  |

## Screenshots

_Add screenshots of the job listing page and add-job form here._

## Author

**Nazma Shaik**
[LinkedIn](https://linkedin.com/in/nazma-shaik22) | [GitHub](https://github.com/Nazma2002)
