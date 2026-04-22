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
 
This project is a RESTful authentication API designed to demonstrate secure user authentication using JWT (JSON Web Token).  
It follows clean architecture principles, separating responsibilities into layers such as controllers, security, and data access.
  
Este projeto é uma API REST de autenticação desenvolvida para demonstrar autenticação segura utilizando JWT (JSON Web Token).  
Ele segue princípios de arquitetura limpa, separando responsabilidades em camadas como controllers, segurança e acesso a dados.

---

## 🧱 Architecture | Arquitetura

```bash
src/main/java/com/example/loginauthapi
├── controllers       # Handles HTTP requests and responses / Controla requisições HTTP
├── domain            # Core business entities / Entidades principais
├── dto               # Data transfer objects / Objetos de transferência de dados
├── infra/security    # Security layer (JWT, filters, config) / Camada de segurança
├── repositories      # Data access layer / Acesso a dados

🔑 Features | Funcionalidades


User registration with validation
Secure authentication (login)
JWT token generation and validation
Route protection using Spring Security
Stateless authentication architecture


Registro de usuários com validação
Autenticação segura (login)
Geração e validação de token JWT
Proteção de rotas com Spring Security
Arquitetura stateless (sem estado)

🔐 Authentication Flow | Fluxo de Autenticação

Client → Login Request → Validate Credentials → Generate JWT → Access Protected Routes
Cliente → Requisição de Login → Validação → Geração de JWT → Acesso às rotas protegidas

📡 API Endpoints | Endpoints

🔓 Login
POST /auth/login

Request | Requisição

{
  "email": "user@email.com",
  "password": "123456"
}

Response | Resposta

{
  "token": "jwt_token_here"
}

📝 Register | Registro
POST /auth/register

Request | Requisição

{
  "email": "user@email.com",
  "password": "123456"
}

🔒 Authorization | Autorização

All protected endpoints require a valid JWT token in the request header.

Todas as rotas protegidas exigem um token JWT válido no header da requisição.

Authorization: Bearer {token}

⚡ Getting Started | Como rodar

📋 Requirements | Requisitos
Java 17+
Maven

▶️ Run the application | Executar o projeto
git clone https://github.com/Rafael078/jwt-auth-api.git
cd jwt-auth-api
mvn spring-boot:run

🧪 Testing | Testes

You can test the API using tools like:

Você pode testar a API utilizando ferramentas como:

Postman
Insomnia

📈 Future Improvements | Melhorias futuras

Role-based authorization (ADMIN / USER)
Refresh token mechanism
Swagger / OpenAPI documentation
Unit and integration tests
Docker support

👨‍💻 Author | Autor

Rafael Souza

⭐ Final Notes | Observações finais

This project was built to demonstrate backend development skills with focus on security, scalability, and clean code practices.

Este projeto foi desenvolvido para demonstrar habilidades em desenvolvimento backend com foco em segurança, escalabilidade e boas práticas de código.
