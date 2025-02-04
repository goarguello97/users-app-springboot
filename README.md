# Users Backend

Este es un proyecto de backend desarrollado con Spring Boot 3.4.1. Proporciona una API REST para la gestión de usuarios, utilizando JPA para la persistencia de datos y MySQL como base de datos relacional.

## Tecnologías utilizadas

- Java 17
- Spring Boot 3.4.1
- Spring Data JPA
- Spring Security
- MySQL
- JWT (JSON Web Token) para autenticación
- Actuator para monitoreo
- Spring Boot DevTools para desarrollo
- Maven como herramienta de construcción

## Requisitos previos

Antes de ejecutar el proyecto, asegúrate de tener instalado lo siguiente:

- [Java 17](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/)

## Configuración

1. Clona el repositorio:
   ```sh
   git clone https://github.com/tu-usuario/users-backend.git
   cd users-backend
   ```

2. Configura la base de datos en `application.properties` o `application.yml`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/users_db
   spring.datasource.username=root
   spring.datasource.password=tu_contraseña
   spring.jpa.hibernate.ddl-auto=update
   ```

3. Ejecuta el proyecto:
   ```sh
   mvn spring-boot:run
   ```

## Autenticación

El sistema usa JWT para la autenticación. Para obtener un token, debes enviar credenciales válidas a `/login`. Luego, usa el token en la cabecera `Authorization: Bearer <TOKEN>` para acceder a los endpoints protegidos.

Desarrollado por [Gonzalo Argüello](https://www.gonzaloarguello.ar)

