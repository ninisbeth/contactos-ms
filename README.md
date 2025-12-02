[![Java 21](https://img.shields.io/badge/Java-21-ED8B00?logo=openjdk&logoColor=white&style=flat-square)](https://openjdk.org/)
[![Spring Boot 3.3](https://img.shields.io/badge/Spring_Boot-3.3-6DB33F?logo=springboot&logoColor=white&style=flat-square)](https://spring.io/projects/spring-boot)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white&style=flat-square)](https://www.docker.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white&style=flat-square)](https://www.postgresql.org/)
[![Maven](https://img.shields.io/badge/Maven-3.9-C71A36?logo=apachemaven&logoColor=white&style=flat-square)](https://maven.apache.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Stars](https://img.shields.io/github/stars/ninisbeth/contactos-ms?style=social)](https://github.com/ninisbeth/contactos-ms/stargazers)
[![Forks](https://img.shields.io/github/forks/ninisbeth/contactos-ms?style=social)](https://github.com/ninisbeth/contactos-ms/network/members)
[![Build Status](https://img.shields.io/github/actions/workflow/status/ninisbeth/contactos-ms/ci-cd.yml?logo=githubactions)](https://github.com/ninisbeth/contactos-ms/actions)  <!-- Si agregas GitHub Actions -->
[![Coverage](https://img.shields.io/badge/Coverage-85%25-brightgreen?logo=codecov)](https://codecov.io/gh/ninisbeth/contactos-ms)  <!-

# Contactos Microservice 🟢

Microservicio de gestión de contactos desarrollado con **Spring Boot 3**, **Spring Data JPA**, **Spring Cloud** y preparado para despliegue con **Docker** y **Docker Compose**.

Ideal como base para arquitecturas de microservicios, cursos, portafolios profesionales o proyectos empresariales.

## 🚀 Tecnologías utilizadas

| Tecnología              | Versión     | Uso                              |
|-------------------------|-------------|----------------------------------|
| Java                    | 21          | Lenguaje principal               |
| Spring Boot             | 3.3.x       | Framework base                   |
| Spring Data JPA         | latest      | Persistencia con Hibernate       |
| Spring Cloud Config     | 2024.0.x    | Configuración centralizada (opcional) |
| PostgreSQL              | 16          | Base de datos                    |
| Docker & Docker Compose | latest      | Contenedores y orquestación      |
| Lombok                  | latest      | Reducción de boilerplate         |
| OpenAPI / Swagger       | 2.2.x       | Documentación automática API     |
| Maven                   | 3.9+        | Gestión de dependencias          |

## 🏃‍♂️ Inicio rápido (3 minutos)

### Opción 1: Con Docker (recomendado)

```bash
git clone https://github.com/ninisbeth/contactos-ms.git
cd contactos-ms
docker compose up --build
```

### Opción 2: Ejecución local
```bash
./mvnw spring-boot:run -Dspring-boot.run.profiles=dev
```

##📍 Endpoints principales (OpenAPI)
Método,Endpoint,Descripción
GET,/api/v1/contactos,Listar todos los contactos
GET,/api/v1/contactos/{id},Buscar por ID
POST,/api/v1/contactos,Crear nuevo contacto
PUT,/api/v1/contactos/{id},Actualizar
DELETE,/api/v1/contactos/{id},Eliminar

Documentación completa: /swagger-ui.html | /v3/api-docs

##🐳 Docker
```bash
# Construir solo la imagen del microservicio
docker build -t contactos-ms:latest .

# Levantar todo (app + postgres)
docker compose up -d
```

⚙️ Perfiles Spring

dev  → H2 en memoria (para pruebas rápidas)
prod → PostgreSQL externo
docker → PostgreSQL en contenedor

🤝 Contribuir
¡Toda contribución es bienvenida! Abre un issue o un PR.
📄 Licencia
MIT License – siéntete libre de usar este proyecto en tu portafolio, empresa o curso.

Hecho con ❤️ para la comunidad de microservicios en español
