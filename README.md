# Sistema de Registro y Gestión de Animales 🐾

Este proyecto es una aplicación backend que permite a los usuarios registrarse, iniciar sesión y agregar animales con los datos de nombre y tipo. Fue desarrollado para aprender a implementar autenticación segura utilizando bcrypt para encriptar contraseñas y jsonwebtoken para manejar tokens de acceso con buenas prácticas.

---

## 🛠️ Tecnologías Utilizadas

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="40" alt="NodeJS"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" height="40" alt="MongoDB"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="Javascript"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/express/express-original-wordmark.svg" height="40" alt="Express" />
</div>

---

## 🎯 Objetivo

El objetivo principal de este proyecto fue:

1. Aprender a implementar autenticación segura con JWT.
2. Practicar el manejo de contraseñas encriptadas con bcrypt.
3. Consolidar conocimientos sobre Express y MongoDB mediante la creación de un sistema de autenticación funcional.

---

## 🚀 Características Principales

- **Registro de usuarios:**
  - Guarda usuarios en la base de datos con contraseñas encriptadas utilizando bcrypt.

- **Protección de rutas:**
  - Solo los usuarios autenticados pueden agregar animales.

- **Gestión de animales:**
  - Permite a los usuarios autenticados agregar animales con información de nombre y tipo.

- **Buenas prácticas de seguridad:**
  - Encriptación segura de contraseñas.
  - Tokens seguros para sesiones de usuario.

---

## 📚 Aprendizajes Adquiridos

A través de este proyecto, aprendí a:

- Configurar y utilizar bcrypt para encriptar y verificar contraseñas.
- Crear y validar tokens JWT con jsonwebtoken.
- Proteger rutas en Express utilizando express-jwt.
- Integrar autenticación con operaciones CRUD en MongoDB.
- Mejorar la estructura y modularidad del código backend.

---

## 🧩 Instalación

1. Clona este repositorio en tu máquina local:

```bash
git clone https://github.com/JordanMedinaOrtiz/SistemadeRegistroyGestiondeAnimales.git
cd SistemadeRegistroyGestiondeAnimales
```

2. Instala las dependencias:

```bash
npm install
```

3. Configura el entorno:

- Crea un archivo `.env` en la raíz del proyecto.
- Define las siguientes variables:

```env
SECRET=tu_llave_secreta_para_jwt
DATABASE=tu_ruta_de_conexión_a_mongodb
```

4. Inicia el servidor:

```bash
node api.js
```

5. Prueba la API:

- Usa herramientas como Postman o Insomnia para probar los siguientes endpoints:
  - `POST /register`: Registrar un nuevo usuario.
  - `POST /login`: Iniciar sesión y obtener un token JWT.
  - `POST /animals`: Agregar un animal (requiere autenticación con el token JWT).

---

Este proyecto me permitió profundizar en la implementación de autenticación segura y protección de rutas en aplicaciones backend. Aprendí a utilizar herramientas esenciales para garantizar buenas prácticas de seguridad, como el uso de bcrypt y JWT, y a combinarlas con operaciones CRUD en un sistema real.