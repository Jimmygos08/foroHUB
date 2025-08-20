# foroHUB
🗨️ Foro Hub

Foro Hub es una API REST desarrollada en Java con Spring Boot cuyo objetivo es gestionar un foro de discusión en línea, centrado en la administración de tópicos.

El proyecto replica la lógica de un foro a nivel de back end, implementando un CRUD completo con autenticación y persistencia en base de datos.

✨ Funcionalidades

Nuestra API permitirá a los usuarios:

➕ Crear un nuevo tópico

📋 Mostrar todos los tópicos creados

🔎 Mostrar un tópico específico

✏️ Actualizar un tópico

🗑️ Eliminar un tópico

Además:

✅ Validaciones basadas en reglas de negocio

🗄️ Base de datos para persistencia de la información

🔐 Autenticación y autorización para proteger el acceso

🛠️ Tecnologías utilizadas

☕ Java 17+

🌱 Spring Boot (Web, Data JPA, Security)

🗄️ MySQL / PostgreSQL (base de datos relacional)

🔑 Spring Security + JWT (autenticación/autorización)

📦 Maven (gestión de dependencias)

⚙️ Instalación y ejecución

Clona este repositorio:

git clone https://github.com/tu-usuario/foro-hub.git
cd foro-hub


Configura tu base de datos en application.properties o application.yml:

spring.datasource.url=jdbc:mysql://localhost:3306/foro_hub
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update


Compila y ejecuta el proyecto:

mvn spring-boot:run

🔑 Endpoints principales
Método	Endpoint	Descripción
POST	/topicos	Crear un nuevo tópico
GET	/topicos	Listar todos los tópicos
GET	/topicos/{id}	Consultar un tópico específico
PUT	/topicos/{id}	Actualizar un tópico
DELETE	/topicos/{id}	Eliminar un tópico
📂 Estructura del proyecto
foro-hub/
│── src/main/java/com/forohub/
│   ├── controller/   # Controladores REST
│   ├── model/        # Entidades
│   ├── repository/   # Repositorios JPA
│   ├── service/      # Lógica de negocio
│   └── security/     # Configuración JWT & Security
│── src/main/resources/
│   ├── application.properties
│── README.md

🔐 Seguridad

Registro e inicio de sesión mediante JWT (JSON Web Token).

Rutas protegidas para garantizar que solo usuarios autenticados puedan acceder o modificar información.

🤝 Contribuciones

Las contribuciones son bienvenidas 🙌.
Puedes crear un issue o enviar un pull request con mejoras y nuevas funcionalidades.

📜 Licencia

Este proyecto está bajo la licencia MIT.
