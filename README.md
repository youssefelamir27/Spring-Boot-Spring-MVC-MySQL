# 🚗 Car List Management Application

A full-stack web application for managing car inventory built with **Spring Boot**, **Spring MVC**, **MySQL**, and **Bootstrap 5**.

## 📋 Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation & Setup](#installation--setup)
- [Database Configuration](#database-configuration)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

- **View All Cars** - Browse through the complete car inventory
- **Add New Car** - Create new car entries with details
- **Edit Car Information** - Update existing car records
- **Delete Cars** - Remove cars from the inventory
- **Responsive Design** - Mobile-friendly interface with Bootstrap 5
- **Beautiful Landing Page** - Eye-catching home page with background image

## 🛠️ Technologies Used

### Backend
- **Spring Boot** - Framework for building the application
- **Spring MVC** - Web framework for handling HTTP requests
- **Spring Data JPA** - Data persistence layer
- **MySQL** - Relational database
- **Maven** - Dependency management

### Frontend
- **HTML5 & CSS3** - Markup and styling
- **Bootstrap 5** - Responsive UI framework
- **Thymeleaf** - Server-side template engine

## 📦 Prerequisites

Before running this application, make sure you have:

- **Java 17** or higher installed
- **MySQL 8.0** or higher installed and running
- **Maven 3.6+** (or use the included Maven wrapper)
- An IDE like **IntelliJ IDEA** or **Eclipse** (optional)

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/youssefelamir27/Spring-Boot-Spring-MVC-MySQL.git
cd Spring-Boot-Spring-MVC-MySQL
```

### 2. Create MySQL Database

Open MySQL Workbench or command line and run:

```sql
CREATE DATABASE carlist_db;
```

### 3. Configure Database Connection

Open `src/main/resources/application.properties` and update with your MySQL credentials:

```properties
spring.application.name=beststore
spring.datasource.url=jdbc:mysql://localhost:3306/carlist_db
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 4. Build the Project

Using Maven wrapper:
```bash
./mvnw clean install
```

Or if you have Maven installed:
```bash
mvn clean install
```

## ▶️ Running the Application

### Option 1: Using Maven
```bash
./mvnw spring-boot:run
```

### Option 2: Using JAR file
```bash
java -jar target/beststore-0.0.1-SNAPSHOT.jar
```

### Option 3: From IDE
Run the main application class (usually named `BeststoreApplication.java`)

The application will start on **http://localhost:8080**

## 📁 Project Structure

```
Spring-Boot-Spring-MVC-MySQL/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/yourpackage/
│   │   │       ├── controller/      # MVC Controllers
│   │   │       ├── model/           # Entity classes
│   │   │       ├── repository/      # JPA Repositories
│   │   │       └── service/         # Business logic
│   │   └── resources/
│   │       ├── static/              # CSS, JS, images
│   │       │   ├── index.html       # Landing page
│   │       │   └── bg2.avif         # Background image
│   │       ├── templates/           # Thymeleaf templates
│   │       │   └── products/        # Car CRUD pages
│   │       └── application.properties
│   └── test/                        # Unit tests
├── pom.xml                          # Maven configuration
└── README.md
```

## 📸 Screenshots

### Landing Page
<img width="1919" height="864" alt="image" src="https://github.com/user-attachments/assets/bddd1d06-6f56-42d4-9a3e-bf295a1210ff" />


### Car List View
<img width="1200" height="861" alt="image" src="https://github.com/user-attachments/assets/953fb990-5442-448a-8d5d-11d27ea90b31" />


### Add/Edit Car Form
<img width="1220" height="707" alt="image" src="https://github.com/user-attachments/assets/2cb4bab4-eee8-46f8-96dc-7b256e92522e" />
<img width="1188" height="664" alt="image" src="https://github.com/user-attachments/assets/6a4db921-2864-4617-97ba-f4dff583690f" />
<img width="1068" height="231" alt="image" src="https://github.com/user-attachments/assets/569747f7-69d7-48d1-82ba-a154fe0b3e07" />

<img width="1178" height="587" alt="image" src="https://github.com/user-attachments/assets/c0b1b1df-581a-4758-90f8-0b493e595a41" />




> **Note:** Add screenshots to a `screenshots/` folder in your repository

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Landing page |
| GET | `/products` | View all cars |
| GET | `/products/create` | Show create car form |
| POST | `/products/create` | Save new car |
| GET | `/products/edit/{id}` | Show edit car form |
| POST | `/products/edit/{id}` | Update car |
| GET | `/products/delete/{id}` | Delete car |

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Youssef Elamir**
- GitHub: [@youssefelamir27](https://github.com/youssefelamir27)

## 🙏 Acknowledgments

- Spring Boot Documentation
- Bootstrap Team
- MySQL Community

---

⭐ If you found this project helpful, please give it a star!

## 📞 Contact

For any questions or feedback, feel free to reach out or open an issue in the repository.
