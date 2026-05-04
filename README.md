# FindBook — Sistema de Gestión de Libros Electrónicos

Plataforma web desarrollada en **Go** para la gestión y venta de libros electrónicos. Permite a autores publicar y gestionar sus obras, y a clientes explorar y adquirir libros digitales. Proyecto académico grupal desarrollado en segundo semestre de Ingeniería en Sistemas.

> **Estado:** Proyecto académico completado — base funcional implementada.

---

## Descripción general

FindBook es un sistema que ofrece a vendedores (autores) una plataforma para publicar y gestionar sus libros electrónicos fácilmente. Implementa operaciones **CRUD** completas sobre tres entidades principales: libros, clientes y proveedores.

---

## Funcionalidades

- **Gestión de Libros** — Crear, leer, actualizar y eliminar registros de libros
- **Gestión de Clientes** — Administración completa de datos de clientes
- **Gestión de Proveedores** — Control de datos de proveedores y autores
- **Interfaz Web** — Plantillas HTML para interacción con el sistema
- **Enrutamiento HTTP** — Manejo de rutas con `gorilla/mux`
- **Conexión a base de datos** — Integración con MySQL usando `go-sql-driver/mysql`

---

## Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| Go (Golang) | Lenguaje principal del backend |
| MySQL | Base de datos relacional |
| gorilla/mux | Enrutador HTTP |
| go-sql-driver/mysql | Driver de conexión a MySQL |
| HTML | Plantillas de interfaz web |
| GitHub | Control de versiones |

---

## Estructura del proyecto

```
findbook-sistema-gestion-libros/
├── codig_go/          # Código fuente Go (entidades, CRUD, servidor)
├── imagenes/          # Recursos gráficos del proyecto
├── mysq/              # Scripts SQL de la base de datos
├── plantillas_html/   # Páginas HTML (inicio, 404, etc.)
└── README.md
```

---

## Arquitectura

El sistema está organizado en paquetes:

- **`base`** — Definición de estructuras y métodos para Clientes, Libros y Proveedores
- **`bdsql`** — Conexión a la base de datos y operaciones CRUD
- **`servidor`** — Manejo de solicitudes HTTP y enrutamiento de rutas

---

## Instalación

```bash
# Clonar el repositorio
git clone https://github.com/norah30/findbook-sistema-gestion-libros.git
cd findbook-sistema-gestion-libros

# Instalar dependencias
go mod tidy

# Configurar la base de datos
# Importar el script SQL desde la carpeta mysq/

# Ejecutar el servidor
go run codig_go/main.go
```

---

## Equipo

Proyecto desarrollado en equipo:

- Nora Calle
- José Córdova
- Omar Llano

---

## Aprendizajes

Este proyecto permitió aplicar conceptos de:
- Desarrollo backend con Go
- Diseño de bases de datos relacionales con MySQL
- Arquitectura en capas (modelo, datos, servidor)
- Trabajo colaborativo con Git y GitHub
