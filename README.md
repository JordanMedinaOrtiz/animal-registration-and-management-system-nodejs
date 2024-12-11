<h1 align="center">Sistema de Registro y Gestión de Animales 🐾</h1>
<p>Este proyecto es una aplicación backend que permite a los usuarios registrarse, iniciar sesión y agregar animales con los datos de nombre y tipo. Fue desarrollado para aprender a implementar autenticación segura utilizando bcrypt para encriptar contraseñas y jsonwebtoken para manejar tokens de acceso con buenas prácticas.</p>
<hr>
<h1 align="center">Tecnologías Utilizadas</h1>
<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="40" alt="NodeJS"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" height="40" alt="MongoDB"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="Javascript"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/express/express-original-wordmark.svg" height="40" alt="Express" />
</div>
<hr>
<h1 align="center">Objetivo</h1>
<p>El objetivo principal de este proyecto fue:</p>
<ol>
  <li>Aprender a implementar autenticación segura con JWT.</li>
  <li>Practicar el manejo de contraseñas encriptadas con bcrypt.</li>
  <li>Consolidar conocimientos sobre Express y MongoDB mediante la creación de un sistema de autenticación funcional.</li>
</ol>
<hr>
<h1 align="center">Características Principales</h1>
<ul>
  <li>Registro de usuarios:</li>
    <ul>
      <li>Guarda usuarios en la base de datos con contraseñas encriptadas utilizando bcrypt.</li>
    </ul>
  <li>Protección de rutas:</li>
     <ul>
      <li>Solo los usuarios autenticados pueden agregar animales.</li>
     </ul>
  <li>Gestión de animales:</li>
     <ul>
      <li>Permite a los usuarios autenticados agregar animales con información de nombre y tipo.</li>
     </ul>
  <li>Buenas prácticas de seguridad:</li>
     <ul>
      <li>Encriptación segura de contraseñas.</li>
      <li>Tokens seguros para sesiones de usuario.</li>
     </ul>
</ul>
<hr>
<h1 align="center">Aprendizajes Adquiridos</h1>
<p>A través de este proyecto, aprendí a:</p>
<ul>
  <li>Configurar y utilizar bcrypt para encriptar y verificar contraseñas.</li>
  <li>Crear y validar tokens JWT con jsonwebtoken.</li>
  <li>Proteger rutas en Express utilizando express-jwt.</li>
  <li>Integrar autenticación con operaciones CRUD en MongoDB.</li>
  <li>Mejorar la estructura y modularidad del código backend.</li>
</ul>
<hr>

### Instalación

1. Clona este reposotorio en tu máquina local:

   ```sh
   git clone https://github.com/JordanMedinaOrtiz/SistemadeRegistroyGestiondeAnimales.git
   cd SistemadeRegistroyGestiondeAnimales
   ```

2. Instala las dependencias:

   ```sh
   npm install
   ```

3. Configura el entorno:
   <ul>
     <li>Crea un archivo .env en la raíz del proyecto.</li>
     <li>Define las siguientes variables:</li>
   </ul>
   
   
   ```sh
   SECRET=tu_llave_secreta_para_jwt
   DATABASE=tu_ruta_de_conexión_a_mongodb
   ```
 4. Inicia el servidor:
    
    ```sh
     node api.js
    ```
 5. Prueba la API:
    <ul>
      <li>Usa herramientas como Postman o Insomnia para probar los siguientes endpoints:</li>
      <ul>
        <li>POST /register: Registrar un nuevo usuario.</li>
        <li>POST /login: Iniciar sesión y obtener un token JWT.</li>
        <li>POST /animals: Agregar un animal (requiere autenticación con el token JWT).</li>
      </ul>
    </ul>
    
<p>Este proyecto me permitió profundizar en la implementación de autenticación segura y protección de rutas en aplicaciones backend. Aprendí a utilizar herramientas esenciales para garantizar buenas prácticas de seguridad, como el uso de bcrypt y JWT, y a combinarlas con operaciones CRUD en un sistema real.</p>
