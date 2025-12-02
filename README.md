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
