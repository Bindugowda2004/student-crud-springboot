# 🎓 Student CRUD Application (Spring Boot)

## 🚀 Overview

This project is a **Spring Boot REST API** that performs CRUD (Create, Read, Update, Delete) operations on Student data.

It follows a **layered architecture** using Controller, Service, and Repository layers and includes Swagger UI for easy API testing.

---

## 🛠️ Tech Stack

* Java 17
* Spring Boot 3
* Spring Data JPA
* MySQL Database
* Maven
* Swagger (OpenAPI)
* SLF4J Logging

---

## 📂 Project Structure

```
src/main/java/com/example/studentcrud
│
├── controller      # REST Controllers
├── service         # Business Logic
├── repository      # DAO Layer (JPA)
├── entity          # Entity Classes
└── StudentCrudApplication.java
```

---

## ⚙️ Features

* ✅ Create Student
* ✅ Get All Students
* ✅ Get Student by ID
* ✅ Update Student
* ✅ Delete Student
* ✅ Swagger UI Integration
* ✅ MySQL Database Integration
* ✅ Logging using SLF4J

---

## ▶️ How to Run

### 🔹 1. Clone Repository

```bash
git clone https://github.com/Bindugowda2004/student-crud-springboot.git
cd student-crud-springboot
```

---

### 🔹 2. Configure MySQL

Create database:

```sql
CREATE DATABASE student_db;
```

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/student_db
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

### 🔹 3. Run Application

```bash
mvn spring-boot:run
```

---

## 🌐 API Endpoints

### ➕ Create Student

POST `/students`

```json
{
  "name": "Bindu",
  "email": "bindu@gmail.com"
}
```

---

### 📥 Get All Students

GET `/students`

---

### 🔍 Get Student by ID

GET `/students/{id}`

---

### ✏️ Update Student

PUT `/students/{id}`

```json
{
  "name": "Updated Name",
  "email": "updated@gmail.com"
}
```

---

### ❌ Delete Student

DELETE `/students/{id}`

---

## 📘 Swagger UI

Test APIs directly in browser:

👉 http://localhost:8080/swagger-ui/index.html

---

## 🗄️ Database

* Database: MySQL
* Schema: `student_db`
* Tables are automatically created using JPA (Hibernate)

---

## 🔐 Notes

* Do not expose your database password in GitHub
* Use environment variables or separate config for production

---

## 📌 Author

**Bindu S Gowda**

---

## ⭐ Future Enhancements

* Input Validation (@Valid)
* Global Exception Handling
* DTO Layer Implementation
* Authentication (JWT)

---
