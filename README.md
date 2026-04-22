# 🔐 JWT Auth API

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,maven" />
</p>

<p align="center">
  <b>Secure authentication API built with Java, Spring Boot and Spring Security</b><br/>
  API de autenticação segura utilizando JWT com Java e Spring Boot
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-red" />
  <img src="https://img.shields.io/badge/Spring_Boot-✔-green" />
  <img src="https://img.shields.io/badge/Spring_Security-✔-green" />
  <img src="https://img.shields.io/badge/JWT-Authentication-blue" />
  <img src="https://img.shields.io/badge/Status-Active-success" />
</p>

---

## 📌 About the Project | Sobre o Projeto

This project is a **RESTful authentication API** designed to demonstrate secure user authentication using **JWT (JSON Web Token)**.

It follows clean architecture principles, separating responsibilities into layers such as controllers, security, and data access.

🔎 From a recruiter perspective, this project demonstrates:
- Secure authentication implementation  
- Backend architecture organization  
- Use of industry-standard technologies  
- Understanding of API security concepts  

---

Este projeto é uma **API REST de autenticação** desenvolvida para demonstrar boas práticas de segurança utilizando JWT.

Ele segue princípios de organização de código e separação de responsabilidades, comuns em aplicações profissionais.

---

## 🧱 Architecture

```bash
src/main/java/com/example/loginauthapi
├── controllers      # API endpoints
├── domain           # Entities
├── dto              # Data transfer objects
├── infra.security   # Security layer (JWT, filters, config)
├── repositories     # Database access

🔑 Features
✔️ User registration
✔️ Secure login authentication
✔️ JWT token generation
✔️ Protected routes with Spring Security
✔️ Stateless authentication
🔐 Authentication Flow
User Login → Validate Credentials → Generate JWT → Access Protected Routes
📡 API Endpoints
🔓 Login
POST /auth/login
{
  "email": "user@email.com",
  "password": "123456"
}

✔️ Response:

{
  "token": "jwt_token_here"
}
📝 Register
POST /auth/register
{
  "email": "user@email.com",
  "password": "123456"
}
🔒 Authorization

All protected endpoints require a JWT token:

Authorization: Bearer {token}
⚡ Getting Started
Requirements
Java 17+
Maven
Run the project
git clone https://github.com/Rafael078/jwt-auth-api.git
cd jwt-auth-api
mvn spring-boot:run
🧪 Testing

You can test the API using:

Postman
Insomnia
📈 Future Improvements
🔹 Role-based authorization (ADMIN / USER)
🔹 Refresh tokens
🔹 Swagger / OpenAPI documentation
🔹 Unit and integration tests
🔹 Docker support
👨‍💻 Author

Rafael Souza

⭐ Final Notes

This project was built to showcase backend development skills with a focus on security, scalability, and clean code practices.
