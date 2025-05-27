# Proyecto de Gestión de Deudas

## Introducción
Esta aplicación web dinámica permite registrar y gestionar las deudas que amigos o personas cercanas tienen contigo. Está desarrollada en Eclipse (Dynamic Web Project) usando Java Servlets y POJOs, con un frontend en HTML5, CSS3 y JavaScript. Se despliega sobre un servidor Apache Tomcat y almacena los datos en una base de datos MySQL (gestionada vía phpMyAdmin).

## Documentación Técnica
A continuación se detallan los artefactos y se dejan espacios para que añadas las imágenes correspondientes.

### 1. Análisis de requisitos
#### Objetivos
- Facilitar el registro de nuevas deudas con datos: nombre, fecha, importe, motivo y archivo adjunto (foto/PDF).
- Ofrecer un panel de administración para visualizar, ordenar y gestionar todas las deudas.
- Permitir la subida y revisión de justificantes de pago.
- Garantizar acceso seguro mediante autenticación.

#### Funcionalidades
- **Insertar Deuda**: formulario para añadir una deuda (`insertar_deuda.html`).
- **Listar Deudas**: vista administrativa (`admin.html`) con opción de ordenar por importe (ascendente/descendente).
- **Editar/Eliminar Deuda**: modificar o borrar un registro existente.
- **Gestión de Justificantes**: subida (`justificante.html`) y revisión (`revisar_justificacion.html`) de comprobantes.
- **Login/Logout**: inicio de sesión seguro (`login.html`).

### 2. Diseño del Sistema
Se incluyen los diagramas UML que ilustran la arquitectura y las interacciones.

#### 2.1 Diagrama de Casos de Uso
![Diagrama de Casos de Uso](docs/diagrama_casos_uso.png)  
*(Inserta aquí el diagrama de casos de uso que representa las acciones del usuario y del administrador.)*

#### 2.2 Diagrama de Clases
![Diagrama de Clases](docs/diagrama_clases.png)  
*(Inserta aquí el diagrama de clases que modela las entidades Deuda, Usuario y Justificante.)*

#### 2.3 Diagrama de Secuencia
![Diagrama de Secuencia](docs/diagrama_secuencia.png)  
*(Inserta aquí el diagrama de secuencia para el flujo ‘Insertar Deuda’.)*

### 3. Modelo de Datos
El modelo entidad-relación define las tablas y sus relaciones en MySQL.

![Modelo de Datos](docs/modelo_datos.png)  
*(Inserta aquí el diagrama ER de la base de datos con tablas: DEUDAS, USUARIOS, JUSTIFICANTES.)*

### 4. Guía de Instalación y Uso
1. **Clona el repositorio** y abre el proyecto en Eclipse como Dynamic Web Project.  
2. **Configura la conexión** a MySQL en `config.js`:
   ```js
   export const dbConfig = {
     host: 'localhost',
     port: 3306,
     user: 'tu_usuario',
     password: 'tu_contraseña',
     database: 'nombre_bd'
   };
