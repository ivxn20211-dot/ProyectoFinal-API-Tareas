# ProyectoFinal-API-Tareas
API REST de tareas con autenticación JWT + Frontend básico
Este proyecto consiste en una aplicación completa que incluye un backend desarrollado con Node.js, Express, MongoDB y JWT, junto con un frontend sencillo en HTML, CSS y JavaScript. El sistema permite registrar usuarios, iniciar sesión y gestionar tareas protegidas mediante autenticación.
---
Funcionalidades principales
Autenticación
• Registro de usuarios
• Inicio de sesión
• Generación y validación de tokens JWT
• Protección de rutas privadas
Gestión de tareas (CRUD)
• Crear tareas
• Listar tareas del usuario autenticado
• Eliminar tareas
• Cada usuario solo puede ver sus propias tareas
Frontend
• Formulario de inicio de sesión
• Formulario para crear tareas
• Listado de tareas
• Botón para eliminar tareas
---
Tecnologías utilizadas
Backend
• Node.js
• Express
• MongoDB y Mongoose
• JSON Web Tokens (JWT)
• CORS
• dotenv
Frontend
• HTML
• CSS
• JavaScript (Fetch API)
Herramientas adicionales
• Postman
• Visual Studio Code
• Git y GitHub

Estructura de el proyecto:
ProyectoFinal/
│ README.md
│ package.json
│ package-lock.json
│ .gitignore
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   ├── config/
│   ├── app.js
│   └── server.js
│
└── Frontend/
    ├── index.html
    ├── style.css
    └── app.js
    
Instalar dependencias:
npm install

Crear un archivo .env con el siguiente contenido:
MONGO_URI=tu_url_de_mongo
JWT_SECRET=tu_secreto
PORT=3000

Inicia el servidor:
npm run dev

El backend estara disponible en:
http://localhost:3000

Cómo usar el frontend
1. Abrir la carpeta Frontend
2. Ejecutar el archivo index.html en el navegador
3. Iniciar sesión con un usuario registrado
4. Crear tareas
5. Visualizar y eliminar tareas

Endpoints de la API
Autenticación
POST /api/auth/register
Permite registrar un nuevo usuario enviando nombre, email y contraseña.
POST /api/auth/login
Permite iniciar sesión. Devuelve un token JWT que se usa para acceder a las rutas protegidas.
---
Tareas (rutas protegidas con JWT)
GET /api/tasks
Devuelve todas las tareas del usuario autenticado.
Requiere enviar el token en los headers.
POST /api/tasks
Crea una nueva tarea asociada al usuario autenticado.
Requiere token.
DELETE /api/tasks/:id
Elimina una tarea por su ID.
Requiere token.

Colección de Postman
Se incluye una colección para probar la API:
• API_Tareas.postman_collection.json
Esta colección contiene todas las rutas necesarias para probar el sistema.
---
Screenshots
Se incluye una carpeta con capturas del funcionamiento del proyecto:
• Registro en Postman
• Inicio de sesión
• Creación de tareas
• Listado de tareas
• Frontend funcionando
---
Video demostrativo
Se incluye un video donde se muestra:
• Backend en ejecución
• Pruebas en Postman
• Funcionamiento del frontend
• CRUD completo de tareas
---
Archivo ZIP del proyecto
El archivo ZIP contiene:
• Código fuente completo
• Frontend
• Documentación
• Video
• Screenshots
• Colección de Postman
