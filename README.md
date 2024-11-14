# BookReviewApp

**BookReviewApp** es una aplicación web que permite a los usuarios descubrir libros, leer reseñas, dejar sus propias calificaciones y comentarios, y gestionar su perfil. Esta aplicación está dividida en dos partes principales:
- **Frontend**: Una interfaz de usuario construida con **Angular**.
- **Backend**: Una API RESTful construida con **.NET** (ASP.NET Core), que maneja la lógica de negocio y la comunicación con la base de datos.

## Requisitos Previos

### Backend (.NET)
Antes de comenzar, asegúrate de tener instalados los siguientes programas en tu máquina:

- **.NET 8 SDK** (o la versión que estés utilizando)
  - [Descargar .NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- **MySQL** o una base de datos compatible (Puedes usar [PlanetScale](https://planetscale.com/) para MySQL si lo deseas).
  - [Descargar MySQL](https://dev.mysql.com/downloads/)
  
### Frontend (Angular)
Para el frontend, asegúrate de tener instalados:

- **Node.js** (versión recomendada: 16.x o superior)
  - [Descargar Node.js](https://nodejs.org/)
- **Angular CLI** (global)
  - Instálalo ejecutando `npm install -g @angular/cli`

## Instrucciones de Configuración

### 1. Configuración del Backend (.NET)

#### 1.1 Clonar el Repositorio

Primero, clona el repositorio:

```bash
git clone https://github.com/tu-usuario/BookReviewApp.git
cd BookReviewApp

2.Configurar la Base de Datos
CREATE DATABASE bookreviewapp;

En el archivo backend/BookReviewApp/appsettings.json, configura la cadena de conexión para MySQL:
{
  "ConnectionStrings": {
    "DefaultConnection": "server=localhost;database=bookreviewapp;user=root;password=tu-contraseña"
  }
}

3. Restaurar y Ejecutar el Backend: cd backend/BookReviewApp
Restaura las dependencias del proyecto: dotnet restore

Ejecuta el proyecto: dotnet run

En la terminal, navega a la carpeta del proyecto backend:

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.2.11.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.
