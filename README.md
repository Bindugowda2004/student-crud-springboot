# 🎓 Student CRUD Application (Spring Boot)

## 🚀 Overview

This is a simple **Spring Boot CRUD application** that performs Create, Read, Update, and Delete operations for Student data.

---

## 🛠️ Tech Stack

* Java 17
* Spring Boot
* Spring Data JPA
* H2 Database
* Maven
* REST APIs

---

## 📂 Project Structure

* Controller Layer
* Service Layer
* Repository (DAO) Layer
* Entity (Student)

---

## ⚙️ Features

* Create Student
* Get All Students
* Get Student by ID
* Update Student
* Delete Student
* Logging using SLF4J

---

## ▶️ How to Run

```bash
mvn spring-boot:run
```

---

## 🌐 API Endpoints

### 🔹 Create Student

POST /students

```json
{
  "name": "Bindu",
  "email": "bindu@gmail.com"
}
```

### 🔹 Get All Students

GET /students

### 🔹 Get by ID

GET /students/{id}

### 🔹 Update Student

PUT /students/{id}

```json
{
  "name": "Updated Name",
  "email": "updated@gmail.com"
}
```

### 🔹 Delete Student

DELETE /students/{id}

---

## 🗄️ H2 Database

* URL: http://localhost:8080/h2-console
* JDBC URL: jdbc:h2:mem:testdb
* Username: sa
* Password: (empty)

---

## 📌 Author

Bindu S Gowda
