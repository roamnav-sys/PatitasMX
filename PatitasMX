# PatitasMX - Configuración Inicial

## 1. Ficha Técnica del Entorno

* **Stack Tecnológico:**
  * **Frontend:** HTML5, CSS3, JavaScript (Vanilla JS)
  * **Backend:** Node.js con Express.js
  * **Base de Datos:** MySQL
  * **Control de Versiones:** Git + GitHub
  * **Despliegue:** Vercel (frontend) / Railway (backend)

* **Justificación del Stack:** Se eligió HTML/CSS/JS puro en el frontend para mantener la simplicidad y velocidad de carga, priorizando la accesibilidad desde dispositivos móviles en zonas con conectividad limitada. Node.js con Express permite un backend ligero y escalable. MySQL ofrece una gestión relacional robusta para el catálogo de mascotas y solicitudes de adopción. Vercel y Railway fueron seleccionados por sus planes gratuitos ideales para proyectos académicos y de prototipado rápido.

* **Herramientas de Desarrollo (Tooling):**
  * **IDE:** Visual Studio Code 1.89+ con extensiones: Prettier, ESLint, REST Client, MySQL (extensión oficial)
  * **Control de versiones:** Git 2.44+ y GitHub (repositorio remoto)
  * **Entorno de ejecución:** Node.js v20 LTS
  * **Gestor de paquetes:** npm v10
  * **Pruebas de API:** Thunder Client (extensión de VS Code)
  * **Diseño de BD:** MySQL Workbench 8.0

---

## 2. Ingeniería Aumentada

* **Prompt Utilizado:**

> Actúa como un arquitecto de software senior especializado en aplicaciones web. Necesito el boilerplate completo para un proyecto llamado "PatitasMX", una plataforma de adopción de mascotas para México. El proyecto usa: Node.js + Express en el backend, MySQL como base de datos, y HTML/CSS/JS puro en el frontend. Genera: (1) la estructura de carpetas completa con nombres de archivos, (2) el archivo package.json con todas las dependencias necesarias (express, mysql2, dotenv, cors, nodemon), (3) el archivo principal server.js con configuración base de Express y conexión a MySQL, (4) un archivo .env.example con las variables de entorno necesarias, (5) un archivo .gitignore apropiado para Node.js, y (6) una ruta de ejemplo GET /api/mascotas que devuelva datos mock en JSON. Usa buenas prácticas: separación por capas (routes, controllers, models), manejo de errores, y variables de entorno.

* **Ajuste Humano (Gobernanza):** La IA generó correctamente la estructura de carpetas y el `server.js` base. Se realizaron los siguientes ajustes manuales:
  1. Se modificó el modelo de base de datos para agregar el campo `municipio` en la tabla `mascotas`, requerido para filtrar por ubicación dentro de Quintana Roo.
  2. Se renombró la ruta `/api/pets` (generada en inglés) a `/api/mascotas` para mantener consistencia con el contexto del proyecto.
  3. Se ajustó la configuración de CORS para permitir exclusivamente el dominio de despliegue en Vercel, limitando el acceso abierto que generó la IA por defecto.
  4. Se agregó manejo de errores personalizado con mensajes en español, ya que la IA los generó en inglés.

---

## 3. Instrucciones de Ejecución

Instrucciones claras para que cualquier otro desarrollador pueda clonar tu repositorio y ejecutar el proyecto localmente.

**Requisitos previos:**
* Node.js v20 LTS instalado
* MySQL 8.0 instalado y corriendo
* Git instalado

**Pasos:**

1. Clonar el repositorio.
```bash
git clone https://github.com/roamnav-sys/PatitasMX.git
cd PatitasMX
```

2. Instalar dependencias.
```bash
npm install
```

3. Configurar variables de entorno.
```bash
cp .env.example .env
# Editar .env con tus credenciales de MySQL y puerto deseado
```

4. Crear la base de datos.
```bash
mysql -u root -p < database/schema.sql
```

5. Ejecutar en entorno de desarrollo.
```bash
npm run dev
```

La aplicación estará disponible en `http://localhost:3000`

---

## Estructura del Proyecto

```
PatitasMX/
├── public/
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── main.js
├── src/
│   ├── routes/
│   │   └── mascotas.routes.js
│   ├── controllers/
│   │   └── mascotas.controller.js
│   ├── models/
│   │   └── mascota.model.js
│   └── config/
│       └── db.js
├── database/
│   └── schema.sql
├── server.js
├── package.json
├── .env.example
└── .gitignore
```

---

## Equipo de Desarrollo

| Nombre | Rol |
|--------|-----|
| Roman | Desarrollador Full Stack / Líder de proyecto |
| [Compañero/a de bina] | Desarrollador Full Stack |

**Docente:** MTI. Paloma Góngora Sabido  
**Materia:** Ingeniería de Software  
**Institución:** TecNM Campus Felipe Carrillo Puerto  
**Semestre:** Enero – Julio 2026
