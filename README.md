# 🔐 JWT Auth API

<p align="center">
  API de autenticação segura com JWT usando Spring Boot e Spring Security  
  <br/>
  Secure authentication API using JWT with Spring Boot and Spring Security
</p>

---

## 🚀 Stack

<p>
  <img src="https://img.shields.io/badge/Java-17-red" />
  <img src="https://img.shields.io/badge/Spring_Boot-✔-green" />
  <img src="https://img.shields.io/badge/Spring_Security-✔-green" />
  <img src="https://img.shields.io/badge/JWT-Auth-blue" />
  <img src="https://img.shields.io/badge/Maven-Build-orange" />
</p>

---

## 📌 Sobre o projeto

API REST desenvolvida para demonstrar autenticação segura utilizando JWT.  
Permite registro, login e proteção de rotas com Spring Security.

This REST API demonstrates secure authentication using JWT, including user registration, login, and protected routes.

---

## 🧱 Arquitetura

```bash
src/main/java/com/example/loginauthapi
├── controllers     # Endpoints da API
├── domain          # Entidades
├── dto             # Requests/Responses
├── infra.security  # Segurança (JWT, filtros, config)
├── repositories    # Acesso a dados
