# First REST API with Spring Boot

This project is a beginner-friendly RESTful API built with **Java** and **Spring Boot**. It demonstrates the fundamental principles of REST architecture and provides basic CRUD operations on a product catalog. The goal of this project is to help newcomers understand how to create and manage REST APIs in a clean, structured manner using Spring Boot.

## 📦 Features

- ✅ Create new products
- 🔍 Retrieve single or multiple products
- ✏️ Update existing products
- ❌ Delete products
- 💾 Uses H2 in-memory database
- 🧪 Easy to test with tools like Postman or curl

## 🛠 Technologies Used

- Java 17+
- Spring Boot
- Maven
- H2 Database
- Spring Web

## 📁 Project Structure

```
src/
└── main/
    └── java/com/springstarter/first_rest_api/
        ├── FirstRestApiApplication.java
        └── product/
            ├── api/
            │   ├── ProductController.java
            │   ├── request/
            │   │   ├── ProductRequest.java
            │   │   └── UpdateProductRequest.java
            │   └── response/
            │       └── ProductResponse.java
            ├── domain/
            │   └── Product.java
            └── repository/
                └── ProductRespository.java
```

## 🚀 Getting Started

### Prerequisites

Ensure the following tools are installed:

- Java 17 or higher
- Maven

### Run the Application

```bash
git clone <repository-url>
cd first-rest-api-java-master
./mvnw spring-boot:run
```

The server will start at `http://localhost:8080`.

## 🔗 API Endpoints

| Method | Endpoint           | Description             |
|--------|--------------------|-------------------------|
| GET    | /products          | Get all products        |
| GET    | /products/{id}     | Get product by ID       |
| POST   | /products          | Create a new product    |
| PUT    | /products/{id}     | Update existing product |
| DELETE | /products/{id}     | Delete a product        |

## 🗃 Database Access (H2 Console)

The application uses an H2 in-memory database. You can access the H2 console at:

```
http://localhost:8080/h2-console
```

**JDBC URL:** `jdbc:h2:mem:testdb`  
**Username:** `sa`  
**Password:** *(leave blank)*

## 📸 Screenshots

- ![GET All Products](screenshots/get-all.png)
- ![POST Product](screenshots/post.png)
- ![GET Product](screenshots/get.png)
- ![PUT Product](screenshots/put.png)
- ![DELETE Product](screenshots/delete.png)
- ![Database View](screenshots/database.png)

## 📄 License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code as needed.

---

Happy Coding! 🎉
