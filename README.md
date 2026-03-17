# 🎮 Proyecto Final - Colección de Videojuegos (Lucas Figal)

<p align="center">
  <a href="#english"><b>English Version</b></a> | 
  <a href="#español"><b>Versión en Español</b></a>
</p>

---

<a name="english"></a>
## 🇺🇸 English Version

### 🛠️ Configuration Steps

This project uses the **Django** framework and an **SQLite** database to manage video game, console, and company data with the following configurations:

1. **Clone the repository.**

2. **Create and activate the virtual environment** (check the `requirements.txt` file if dependencies need to be installed).

3. **Run Migrations:** Ensure the database is up to date with the models.

4. **Create Superuser:** To access the admin panel and manage user data.

5. **Run the local server:**

The project should be available at `http://127.0.0.1:8000/`.

### 💻 App Usage and Functionalities

The project implements a complete **Authentication** and **CRUD** (Create, Read, Update, Delete) system for the three main models.

#### 🗺️ Access Points and Functionalities

| URL Path | View Name | Key Functionality |
| :--- | :--- | :--- |
| **`/`** | `views.inicio` | ✅ Main index and navigation links. |
| **`/usuarios/register/`** | `UserRegistrationView` | ✅ New user creation (Authentication). |
| **`/games/list/**` | `views.game_list` | ✅ Listing, Search, and Alert Message. |
| **`/games/add/**` | `views.create_game` | ✅ Record creation (ModelForm). |
| **`/games/detail/<pk>/`** | `GameDetail` | ✅ Detail and access to edit/delete. |
| **`/about-me/**` | `views.about_me` | ✅ Static content about the author/project. |

#### 📋 Test Steps (Recommended Testing Order for Demo)

1. **Authentication:**
    * Register a new user at `/usuarios/register/`.
    * Log in and log out.

2. **Full CRUD:**
    * Access `/games/add/` and create a new game, including an image (MEDIA).
    * Verify that the list updates.
    * Access the game detail, then **Edit** and **Delete** the record.

3. **Search and Filter:**
    * Use the search function to filter the game list by title.
    * Verify that the "alert message" is displayed if there are no results.

4. **Final Verification:**
    * Access the Django Admin (`http://127.0.0.1:8000/admin/`) to verify that the `Game`, `Console`, and `Company` models are registered and that the `User` model is functional.

---

<a name="español"></a>
## 🇲🇽 Versión en Español

### 🛠️ Pasos de Configuración

Este proyecto utiliza el framework **Django** y una base de datos **SQLite** para gestionar datos de videojuegos, consolas y empresas, con las siguientes configuraciones:

1. **Clonar el repositorio.**

2. **Crear y activar el entorno virtual** (revisar el archivo `requirements.txt` si es necesario instalar dependencias).

3. **Realizar Migraciones:** Asegurarse de que la base de datos esté actualizada con los modelos.

4. **Crear Superusuario:** Para acceder al administrador y gestionar datos de usuarios.

5. **Ejecutar el servidor local:**

El proyecto debería estar disponible en `http://127.0.0.1:8000/`.

## 💻 Uso de la Aplicación y Funcionalidades

El proyecto implementa un sistema completo de **Autenticación** y **CRUD** (Crear, Leer, Actualizar, Eliminar) para los tres modelos principales.

### 🗺️ Puntos de Acceso y Funcionalidades

| Ruta URL | Nombre de la Vista | Funcionalidad Clave |
| :--- | :--- | :--- |
| **`/`** | `views.inicio` | ✅ Índice principal y enlaces de navegación. |
| **`/usuarios/registro/`** | `RegistroUsuarioView` | ✅ Creación de nuevos usuarios (Autenticación). |
| **`/juegos/lista/**` | `views.lista_juegos` | ✅ Listado, Búsqueda y Mensaje de Aviso. |
| **`/juegos/agregar/**` | `views.crear_juego` | ✅ Creación de registros (Formulario ModelForm). |
| **`/juegos/detalle/<pk>/`** | `JuegoDetalle` | ✅ Detalle y acceso a edición/eliminación. |
| **`/acerca-de-mi/**` | `views.acerca_de_mi` | ✅ Contenido estático del autor/proyecto. |

### 📋 Pasos de Prueba (Orden de Prueba Recomendado para la Demostración)

1. **Autenticación:**
    * Registrar un nuevo usuario en `/usuarios/registro/`.
    * Iniciar sesión y cerrar sesión.

2. **CRUD Completo:**
    * Acceder a `/juegos/agregar/` y crear un nuevo juego, incluyendo una imagen (MEDIA).
    * Verificar que el listado se actualice.
    * Acceder al detalle del juego, luego **Editar** y **Eliminar** el registro.

3. **Búsqueda y Filtro:**
    * Utilizar la función de búsqueda para filtrar la lista de juegos por título.
    * Verificar que se muestre el "mensaje de aviso" si no hay resultados.

4. **Verificación Final:**
    * Acceder al Administrador de Django (`http://127.0.0.1:8000/admin/`) para verificar que los modelos de `Juego`, `Consola` y `Empresa` están registrados y que el modelo `User` está funcional.