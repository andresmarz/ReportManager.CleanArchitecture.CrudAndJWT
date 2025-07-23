# ReportManager.CleanArchitecture.CrudAndJWT

This project builds upon the basic CRUD structure and adds secure authentication using JWT (JSON Web Tokens). It's built with ASP.NET Core and follows the Clean Architecture pattern.

## 🔧 Technologies Used

- ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- Clean Architecture
- JWT Authentication
- AutoMapper

## 📂 Project Structure

- **Domain** – Business entities and interfaces
- **Application** – Application logic and DTOs
- **Infrastructure** – EF Core repositories and services
- **WebAPI** – Controllers and JWT setup

## 🔐 Authentication

- The API uses JWT-based authentication.
- Register a new user via `/api/Auth/register`.
- Login with `/api/Auth/login` to receive a JWT token.
- Use the token in Swagger’s **Authorize** button or Postman headers as:
Authorization: Bearer <your_token>

## 🚀 How to Run

1. Open the solution in Visual Studio
2. Set the WebAPI project as the startup project
3. Apply any migrations:
 ```bash
 Update-Database
Run the project (F5) and test the secure endpoints using Swagger or Postman.

📌 Notes
This version is ideal to learn how to implement secure APIs with JWT in a clean, scalable architecture.
