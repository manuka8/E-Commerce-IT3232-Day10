

# 🏛️ ICT Department Management System (Spring Boot)

This is a Spring Boot-based backend application for managing departments, employees, persons, and projects. It follows a clean, layered architecture using Controllers, Services, Repositories, and Models.

---

## 📂 Project Structure

```

ict/
├── Day10Application.java           # Main application class
├── controller/                    # Handles HTTP requests
│   └── DepartmentController.java
├── service/                       # Business logic
│   └── DepartmentService.java
├── repo/                          # Database access layer
│   └── DepartmentRepo.java
├── model/                         # Entity models
│   ├── Department.java
│   ├── Employee.java
│   ├── Person.java
│   └── Project.java
├── exceptionHandler/             # Global exception handling
│   └── GenericExceptionHandler.java

````

---

## ⚙️ Technologies

- Java 17+
- Spring Boot
- Spring Data JPA
- Maven
- MySQL (or H2 for testing)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <repo-url>
cd ict
````

### 2. Configure Database

Update your `application.properties` file with your DB credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### 3. Run the App

You can run the app using:

```bash
./mvnw spring-boot:run
```

Or run `Day10Application.java` from your IDE.

---

## 📌 API Overview

| Method | Endpoint          | Description             |
| ------ | ----------------- | ----------------------- |
| GET    | /departments      | List all departments    |
| POST   | /departments      | Create a new department |
| PUT    | /departments/{id} | Update a department     |
| DELETE | /departments/{id} | Delete a department     |

---

## 📦 Future Enhancements

* Add CRUD for `Employee`, `Project`, `Person`
* Implement pagination and sorting
* Add Swagger documentation
* Secure endpoints with Spring Security



```

---

Let me know if you'd like me to generate this as an actual file or customize it with your name, university, or database setup details.
```
