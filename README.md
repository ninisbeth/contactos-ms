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
