# GrupoF-GestionDeProyectos
Repositorio para el "Grupo F" de Gestion de Proyectos.

# Sistema Integral de Gestión Gastronómica ☕

### Este proyecto es un Ecosistema Gastronómico Digital e Integral diseñado para transformar establecimientos tradicionales en negocios inteligentes. Optimizando la comunicación en tiempo real entre clientes, mozos, barra/cocina, cajero y administración.

![Estado](https://img.shields.io/badge/estado-en%20desarrollo-yellow)
![Versión](https://img.shields.io/badge/versión-1.0.0-blue)
![Licencia](https://img.shields.io/badge/licencia-MIT-green)
![Java](https://img.shields.io/badge/Java-21-orange?logo=java)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.5-brightgreen?logo=springboot)

## 📖 Tabla de Contenidos

*   [Descripción](#descripción)
*   [Tecnologías](#tecnologías)
*   [Requisitos previos](#requisitos-previos)
*   [Instalación](#instalación)
*   [Uso](#uso)
*   [Estructura del proyecto](#estructura-del-proyecto)
*   [Equipo](#equipo)
*   [Licencia](#licencia)

## Descripción

**Sistema Integral de Gestión Gastronómica** es una plataforma integral desarrollada como proyecto final para la carrera de **Desarrollo de Software**. El sistema permite digitalizar y conectar en tiempo real todas las áreas de un establecimiento (salón, cocina, barra y administración), transformando un negocio tradicional en un establecimiento inteligente.

Está orientado a **dueños y administradores de establecimientos gastronómicos (Restobares y Cafeterías)** que buscan eliminar la fricción operativa y modernizar la experiencia del cliente final.

### Objetivo del sistema
El sistema resuelve el problema de la desorganización y la pérdida de información en los procesos manuales. Aporta valor a través de:

*   **Eliminación de errores:** Sustituye el lápiz y papel por terminales digitales (móviles y KDS) con actualización instantánea vía WebSockets.
*   **Control de costos preciso:** Implementa la lógica de **escandallo**, permitiendo que cada venta descuente automáticamente los insumos exactos (gramos, mililitros) del inventario.
*   **Optimización del servicio:** Empodera al cliente permitiéndole el control de su pedido mediante códigos QR, reduciendo tiempos de espera y carga de trabajo del personal de salón.
*   **Transparencia financiera:** Garantiza la integridad de los ingresos mediante auditorías de arqueo de caja "ciegos", asegurando que el stock físico coincida con la facturación.

## Tecnologías

| Capa | Tecnología | Versión |
| :--- | :--- | :--- |
| **Backend** | Java / Spring Boot | 21 / 4.0.5 |
| **Seguridad** | Spring Security (JWT) | 6.x |
| **Tiempo Real** | WebSockets (STOMP) | - |
| **Base de datos** | PostgreSQL (JPA / Hibernate) | 16.x |
| **Frontend Web** | Next.js | 14.x |
| **Mobile** | React Native (Expo) | - |
| **Control de versiones** | Git / GitHub / Mercurial | - |
| **Gestor de paquetes** | Maven / npm | - |
| **Entorno de Trabajo** | Devuan Linux (Excalibur) / Windows 10/11 | - |

## Requisitos previos

*   **Java Development Kit (JDK):** Versión 21
*   **Maven:** 3.9 o superior
*   **Node.js:** 20.x o superior (LTS)
*   **Base de datos:** PostgreSQL 16.x
*   **Git:** Para el control de versiones

## Instalación
En desarrollo...
### 🖥️ Backend
### 🌐 Frontend

## 🚀 Guía de Uso

El sistema está diseñado para que la información fluya sin interrupciones entre los cuatro perfiles principales:

### 1. Experiencia del Cliente (Autogestión)
*   **Acceso:** El cliente escanea el código QR de su mesa.
*   **Pedido:** Accede a la carta digital, selecciona sus productos y confirma el pedido.
*   **Pago:** Puede solicitar la cuenta o pagar de forma autónoma desde su móvil.

### 2. Personal de Salón (App Móvil)
*   **Gestión de Mesas:** El mozo visualiza en tiempo real qué mesas están libres, ocupadas o solicitando atención.
*   **Toma de Pedidos:** Carga pedidos directamente en la App, los cuales se sincronizan instantáneamente con la barra/cocina.

### 3. Cocina y Barra (Sistema KDS)
*   **Producción:** Los preparadores visualizan las comandas en pantallas digitales (KDS) organizadas por orden de llegada y prioridad.
*   **Notificación:** Al marcar un plato como "Listo", el personal de salón recibe una notificación inmediata para su entrega.

### 4. Administración y Caja (Panel Web)
*   **Control de Stock:** Visualización del inventario actualizado automáticamente mediante la lógica de **escandallo**.
*   **Cierre de Jornada:** Realización de **arqueos de caja ciegos** para garantizar la transparencia financiera y auditoría de ventas.

## Variables de entorno
En desarrollo...

## Estructura del proyecto
En desarrollo...

## Endpoints disponibles
En desarrollo... no esta completamente definida...
**Base URL:** `http://localhost:8080/api/v1`

| Método | Endpoint | Descripción | Auth requerida |
| :--- | :--- | :--- | :--- |
| **POST** | `/auth/login` | Inicio de sesión y obtención de token JWT | No |
| **GET** | `/mesas` | Listar estado de todas las mesas (Salón) | Sí |
| **GET** | `/productos` | Listar carta/menú disponible con stock real | Sí |
| **POST** | `/pedidos` | Crear una nueva orden (Mozo o QR Cliente) | Sí |
| **GET** | `/pedidos/pendientes` | Ver órdenes para preparar (Pantalla KDS) | Sí |
| **PATCH** | `/pedidos/{id}/estado` | Cambiar estado (En preparación / Entregado) | Sí |
| **GET** | `/inventario` | Ver stock de insumos y niveles críticos | Sí (Admin) |
| **POST** | `/arqueos` | Registrar cierre de caja "ciego" | Sí (Cajero) |

> **Nota sobre Tiempo Real:** Para la actualización instantánea de comandas en cocina y estados de mesa, el sistema utiliza **WebSockets** a través del endpoint `ws://localhost:8080/ws-gastronomico`.

## Estado del proyecto y sprint actual

| Módulo | Estado |
| :--- | :--- |
| **Backend (Java 21 / Spring Boot)** | Pendiente |
| **Autenticación (JWT)** | Pendiente |
| **Lógica de Escandallo (Inventario)** | Pendiente |
| **Comunicación en tiempo real (WebSockets)** | Pendiente |
| **Frontend Web (Next.js)** | Pendiente |
| **App Mobile (React Native / Expo)** | Pendiente |
| **Módulo de Arqueo de Caja Ciego** | Pendiente |

**Sprint actual:** Sprint 3 — Backend con SpringBoot
**Fecha de cierre estimada:** 22/06/2026

## Equipo de desarrollo

| Nombre completo | Rol en el proyecto | GitHub |
| :--- | :--- | :--- |
| :--- | :--- | :--- |
| [Apellido, Nombre] | Desarrollador Full Stack | [@usuario1](https://github.com) |
| [Apellido, Nombre] | Desarrollador Full Stack | [@usuario2](https://github.com) |
| [Apellido, Nombre] | Desarrollador Full Stack | [@usuario3](https://github.com) |
| [Apellido, Nombre] | Desarrollador Full Stack | [@usuario4](https://github.com) |
| [Apellido, Nombre Profesor] | Tutor / Product Owner | [@usuario_prof](https://github.com) |

**Docente:** [Nombre de tu Profesor/a]  
**Institución:** Tecnicatura Superior en Desarrollo de Software  
**Materia:** Proyecto Final / Prácticas Profesionalizantes II — **Año:** 2026

## Licencia

Este proyecto fue desarrollado íntegramente con fines académicos como parte del trabajo final de la carrera. Se encuentra distribuido bajo la licencia [MIT](LICENSE).

## Contribuciones

Este es un proyecto académico de carácter integrador. Si deseas reportar errores, bugs o realizar sugerencias para mejorar la lógica del ecosistema (especialmente en la implementación de WebSockets o el módulo de escandallo), por favor abre un [Issue](https://github.com/tu-usuario/tu-repositorio/issues) en este repositorio.


