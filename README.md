# 📦 Product Inventory System

## 📖 Description
Product Inventory System is a Spring Boot REST API application developed to manage product inventory efficiently. It provides complete CRUD (Create, Read, Update, Delete) operations for products using Spring Boot, Spring Data JPA, and MySQL. The project follows a layered architecture to ensure maintainability and scalability and is designed for cloud-native deployment using Docker, Kubernetes, and Jenkins CI/CD pipelines.

---

## 🚀 Features

- Add a new product
- View all products
- View a product by ID
- Update product details
- Delete a product
- Delete all products
- RESTful API implementation
- MySQL database integration
- Docker containerization
- Kubernetes deployment support
- Jenkins CI/CD pipeline integration

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Maven
- Docker
- Kubernetes
- Jenkins
- Git & GitHub

---

## 📂 Project Structure

```
ProductInventorySystem
│── src
│   ├── main
│   │   ├── java
│   │   │   ├── controller
│   │   │   ├── dao
│   │   │   ├── entity
│   │   │   ├── service
│   │   │   └── ProductInventorySystemApplication.java
│   │   └── resources
│   │       ├── application.properties
│   │       └── static
│── Dockerfile
│── Jenkinsfile
│── kubernetes
│── pom.xml
│── README.md
```

---

## ⚙️ Prerequisites

Before running the project, ensure you have:

- Java 17 or later
- Maven
- MySQL Server
- Docker (optional)
- Kubernetes (optional)
- Jenkins (optional)

---

## 🔧 Installation

### Clone the Repository

```bash
git clone https://github.com/PragatiJayaramRathod/ProductInventorySystem.git
```

Navigate to the project folder.

```bash
cd ProductInventorySystem
```

---

## 🗄️ Database Configuration

Update the `application.properties` file with your MySQL credentials.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/product_inventory
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## ▶️ Run the Application

Using Maven

```bash
mvn spring-boot:run
```

Or

```bash
mvn clean install
java -jar target/ProductInventorySystem.jar
```

---

## 📡 REST API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/api/products` | Get all products |
| GET | `/api/products/{id}` | Get product by ID |
| POST | `/api/products` | Add a product |
| PUT | `/api/products/{id}` | Update product |
| DELETE | `/api/products/{id}` | Delete product |
| DELETE | `/api/products` | Delete all products |

---

## 🐳 Docker

Build Docker Image

```bash
docker build -t productinventorysystem .
```

Run Container

```bash
docker run -p 8080:8080 productinventorysystem
```

---

## ☸️ Kubernetes

Deploy to Kubernetes

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

Check resources

```bash
kubectl get pods
kubectl get svc
```

---

## 🔄 Jenkins CI/CD

The project supports Jenkins pipeline automation for:

- Source code checkout
- Maven build
- Unit testing
- Docker image creation
- Docker Hub push
- Kubernetes deployment

---

## 📸 API Testing

You can test the APIs using:

- Postman
- Swagger (if configured)
- cURL

Example:

```bash
GET http://localhost:8080/api/products
```

---

## 🌟 Future Enhancements

- User Authentication (JWT)
- Product Search & Filtering
- Pagination
- Category Management
- Image Upload
- Swagger Documentation
- Unit & Integration Testing

---

## 👩‍💻 Author

**Pragati Jayaram Rathod**

GitHub: https://github.com/PragatiJayaramRathod

---

## 📄 License

This project is developed for learning and educational purposes.
