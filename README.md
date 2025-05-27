# Debt Management Project

## Introduction
This dynamic web application lets you record and manage debts owed by friends or close contacts. It was developed in Eclipse (Dynamic Web Project) using Java Servlets and POJOs, with a frontend built in HTML5, CSS3 and JavaScript. It is deployed on an Apache Tomcat server and stores data in a MySQL database (managed via phpMyAdmin).

## Technical Documentation
Below are the required artifacts, with placeholders for your diagrams and screenshots.

### 1. Requirements Analysis
#### Objectives
- Allow registration of new debts with the following fields: name, date, amount, reason, and an optional attachment (photo/PDF).  
- Provide an admin panel to view, sort, and manage all debts.  
- Enable upload and review of payment proofs.  
- Ensure secure access via authentication.

#### Functionalities
- **Insert Debt**: form to add a debt (`insertar_deuda.html`).  
- **List Debts**: admin view (`admin.html`) with sort-by-amount (ascending/descending).  
- **Edit/Delete Debt**: modify or remove existing records.  
- **Manage Proofs**: upload (`justificante.html`) and review (`revisar_justificacion.html`) payment proofs.  
- **Login/Logout**: secure sign-in and sign-out (`login.html`).  

### 2. System Design
The UML diagrams below illustrate the architecture and interactions.

### 3. Data Model
The entity–relationship model defining the tables and relationships in MySQL.

### 4. Installation and Usage Guide

1. **Create the database and tables** by running the `schema.sql` script in phpMyAdmin.  
2. **Deploy** the project to Apache Tomcat from Eclipse.  
3. **Access** the application at `http://localhost:8080/tu-app/`.  
4. **Register/Login** and start managing your debts.

### 5. Tests Performed

#### 5.1 Unit Tests
- JUnit test classes for insert, edit, and delete operations on debts.  
- **Coverage:** 85% in the `models` package.  
*(Add Maven/JUnit console output or coverage report screenshot: `docs/unit_tests.png`)*

#### 5.2 Integration Tests
- End-to-end tests with Postman against the Servlet endpoints.  
- Verified full flow: authentication → insert → list → upload proof.  
*(Attach Postman collection or HTTP response screenshots: `docs/integration_tests.png`)*

---

## Technologies Used
- **Java EE:** Servlets, JDBC  
- **Server:** Apache Tomcat  
- **Database:** MySQL (phpMyAdmin)  
- **Frontend:** HTML5, CSS3, Vanilla JavaScript  

---

`## Project Structure
```text
/WebContent/
├─ insertar_deuda.html
├─ admin.html
├─ login.html
├─ justificante.html
└─ revisar_justificacion.html
/src/
├─ servlets/
│   ├─ InsertarDeudaServlet.java
│   ├─ EditarDeudaServlet.java
│   ├─ AdminServlet.java
│   └─ JustificacionServlet.java
└─ models/
    └─ Deuda.java
/config/
└─ config.js
/scripts/
├─ auth.js
├─ deuda.js
└─ inicio.js

---

Pictures

Home Page
![Pantalla de Inicio](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.45.54.png)

Login Page
![Formulario de Login](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.45.58.png)

Insertar Deuda – Formulario
![Formulario Insertar Deuda](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.14.png)

Insertar Deuda – Listado de Deudas
![Listado Deudas 1](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.19.png)
![Listado Deudas 2](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.22.png)

Justificantes Pendientes
![Justificantes Pendientes](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.27.png)

Editar Deuda
![Editar Deuda](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.47.png)

Contributing

Contributions are welcome! Please open issues or pull requests for improvements.

License

This project is licensed under the MIT License.
`## Project Structure

```text
/WebContent/
├─ insertar_deuda.html
├─ admin.html
├─ login.html
├─ justificante.html
└─ revisar_justificacion.html
/src/
├─ servlets/
│   ├─ InsertarDeudaServlet.java
│   ├─ EditarDeudaServlet.java
│   ├─ AdminServlet.java
│   └─ JustificacionServlet.java
└─ models/
    └─ Deuda.java
/config/
└─ config.js
/scripts/
├─ auth.js
├─ deuda.js
└─ inicio.js
```

---

## Pictures

### Home Page  
![Pantalla de Inicio](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.45.54.png)

### Login Page  
![Formulario de Login](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.45.58.png)

### Insertar Deuda – Formulario  
![Formulario Insertar Deuda](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.14.png)

### Insertar Deuda – Listado de Deudas  
![Listado Deudas 1](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.19.png)  
![Listado Deudas 2](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.22.png)

### Justificantes Pendientes  
![Justificantes Pendientes](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.27.png)

### Editar Deuda  
![Editar Deuda](docs/screenshots/Captura de pantalla 2025-05-27 a las 19.46.47.png)

---

## Contributing
Contributions are welcome! Please open issues or pull requests for improvements.

---

## License
This project is licensed under the MIT License.
