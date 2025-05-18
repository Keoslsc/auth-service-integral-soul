# Auth API – Microservicio de Autenticación para Integral Soul

Este microservicio es responsable de la autenticación centralizada en la arquitectura de microservicios de **Integral Soul**. Maneja:

- Registro e inicio de sesión con email y contraseña
- Login con Google o Apple mediante Firebase
- Emisión y revocación de tokens vía Sanctum
- Control de acceso con roles `admin` y `super-admin` (usando Spatie)
- Separación lógica por guards (`clients`, `admins`)
- Envío de correos (registro, recuperación) usando Mailtrap

---

## 📦 Librerías utilizadas

- **Laravel 11** – Framework base
- **Sanctum** – Autenticación basada en tokens
- **Spatie Laravel-Permission** – Roles y permisos para `admins`
- **Firebase JWT (verificación)** – Para login social
- **MySQL** – Base de datos compartida con otros servicios

---