# Product Store 🛒

## Descripción

Product Store es una aplicación web para gestionar productos. Permite a los usuarios ver, agregar, editar y eliminar productos de una base de datos MongoDB. La aplicación utiliza un backend en Node.js con Express.js y un frontend en React.js con Chakra UI.

## Tecnologías utilizadas

### Backend:

- Node.js
- Express.js
- MongoDB (Mongoose)
- dotenv

### Frontend:

- React.js
- Zustand (para gestión de estado)
- Chakra UI (para estilos y componentes de UI)

## Instalación y configuración

### Prerrequisitos

Asegurate de tener instalado:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Pasos para ejecutar el proyecto

1. Clonar el repositorio:

   ```sh
   git clone https://github.com/tu-usuario/product-store.git
   cd product-store
   ```

2. Instalar las dependencias:

   ```sh
   npm run build
   ```

3. Crear un archivo `.env` en la carpeta raiz y agregar las siguientes variables de entorno:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   ```

4. Iniciar el servidor backend:

   ```sh
   npm run start
   ```



La aplicación estará disponible en `http://localhost:5000`.

## Endpoints de la API

### **Productos**

| Método | Ruta                | Descripción                     |
| ------ | ------------------- | ------------------------------- |
| GET    | `/api/products`     | Obtiene todos los productos     |
| POST   | `/api/products`     | Crea un nuevo producto          |
| PUT    | `/api/products/:id` | Actualiza un producto existente |
| DELETE | `/api/products/:id` | Elimina un producto             |

## Estructura del proyecto

```
📦 product-store
 ┣ 📂 backend
 ┃ ┣ 📂 config
 ┃ ┃ ┗ 📜 db.js
 ┃ ┣ 📂 controllers
 ┃ ┃ ┗ 📜 product.controller.js
 ┃ ┣ 📂 models
 ┃ ┃ ┗ 📜 product.model.js
 ┃ ┣ 📂 routes
 ┃ ┃ ┗ 📜 product.route.js
 ┃ ┣ 📜 server.js
 ┣ 📂 frontend
 ┃ ┣ 📂 src
 ┃ ┃ ┣ 📂 components
 ┃ ┃ ┃ ┣ 📜 Navbar.jsx
 ┃ ┃ ┃ ┗ 📜 ProductCard.jsx
 ┃ ┃ ┣ 📂 pages
 ┃ ┃ ┃ ┣ 📜 HomePage.jsx
 ┃ ┃ ┃ ┗ 📜 CreatePage.jsx
 ┃ ┃ ┣ 📂 store
 ┃ ┃ ┃ ┗ 📜 product.js
 ┃ ┃ ┣ 📜 app.jsx
 ┃ ┃ ┗ 📜 main.jsx
 ┃ ┗ 📜 package.json
 ┣ 📜 package.json
 ┣ 📜 .env
 ┗ 📜 README.md
```

## Autor

Desarrollado por Santiago Chimko.

