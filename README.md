Este es un proyecto simple que funciona como un gestor de tareas personalizadas. Cada usuario puede registrarse e iniciar sesión para acceder exclusivamente a sus tareas. Se implementa un sistema de autenticación basado en tokens que utiliza cookies para mantener la sesión activa. Antes de acceder a rutas protegidas, el sistema valida la autenticidad del token. Las tareas de los usuarios se almacenan en una base de datos MongoDB.

# Flujo de trabajo

# Back-End
El backend se encarga de manejar la lógica del servidor, la seguridad y la conexión con la base de datos. Las herramientas utilizadas son:

bcryptjs: Para cifrar las contraseñas antes de almacenarlas, garantizando la seguridad de los datos sensibles.
cookie-parser: Middleware que facilita el manejo de cookies en las solicitudes HTTP.
cors: Permite que el servidor sea accesible desde diferentes orígenes (URLs) durante el desarrollo y producción.
dotenv: Carga y administra variables de entorno para configurar el entorno de ejecución de manera segura.
express: Framework minimalista para construir aplicaciones web y APIs.
jsonwebtoken: Permite la generación y validación de tokens de autenticación.
mongoose: ODM (Object Data Modeling) para trabajar con bases de datos MongoDB.
morgan: Middleware que registra las solicitudes HTTP en la consola para facilitar el desarrollo y la depuración.
zod: Biblioteca que ayuda a validar y garantizar la estructura de los datos que el servidor recibe.

# Front-End
El frontend maneja la interfaz de usuario, haciendo que la experiencia sea fluida e interactiva. Las herramientas utilizadas son:

axios: Para realizar solicitudes HTTP al backend de forma sencilla.
dayjs: Ayuda a formatear y manejar fechas de manera efectiva.
js-cookie: Proporciona una forma simple de manipular cookies en el navegador.
react: Biblioteca para construir interfaces de usuario dinámicas y componentes reutilizables.
react-hook-form: Simplifica la gestión y validación de formularios en React.
react-router-dom: Permite implementar un sistema de navegación entre páginas y rutas en la aplicación.