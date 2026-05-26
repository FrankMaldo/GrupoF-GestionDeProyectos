# GrupoF-GestionDeProyectos
Repositorio para el "Grupo F" de Gestion de Proyectos.

---

# Sistema Integral de Gestión Gastronómica - Coffee Blinders ☕

Un ecosistema digital e integral diseñado para transformar la gestión tradicional de establecimientos gastronómicos en un modelo inteligente, agilizando la interacción en tiempo real entre clientes, mozos, cocina y administración. Esta solución está completamente adaptada y personalizada para las necesidades operativas de la cafetería **Coffee Blinders**.

![Estado](https://img.shields.io/badge/estado-en%20desarrollo-yellow)
![Versión](https://img.shields.io/badge/versión-1.0.0-blue)
![Licencia](https://img.shields.io/badge/licencia-MIT-green)
![Java](https://img.shields.io/badge/Java-21-orange?logo=java)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.X-brightgreen?logo=springboot)

## 📋 Tabla de Contenidos

* [1. Descripción del Proyecto](#3-descripción-del-proyecto)
* [2. Stack Tecnológico](#4-stack-tecnológico)
* [3. Requisitos Previos e Instalación](#5-requisitos-previos-e-instalación)
* [4. Variables de Entorno](#6-variables-de-entorno)
* [5. Estructura del Proyecto](#7-estructura-del-proyecto)
* [6. Endpoints de la API](#8-endpoints-de-la-api)
* [7. Estado del Proyecto y Sprint Actual](#9-estado-del-proyecto-y-sprint-actual)
* [8. Equipo de Desarrollo](#10-equipo-de-desarrollo)
* [9. Licencia y Contribuciones](#11-licencia-y-contribuciones)

## 1. Descripción del Proyecto

**Sistema Integral de Gestión Gastronómica** es un ecosistema digital e integrado diseñado para transformar la gestión tradicional de establecimientos gastronómicos en un modelo inteligente. El sistema permite a los usuarios interactuar en tiempo real mediante un flujo automatizado que abarca desde el escaneo de códigos QR en las mesas, la toma de comandas, el procesamiento en pantallas de producción, hasta el control de caja y la administración centralizada de inventarios. 

Está orientado a establecimientos del sector gastronómico (tales como restobares y cafeterías) que busquen modernizar su operación, optimizar sus tiempos de servicio y eliminar los errores humanos del proceso manual. Para este caso de estudio y despliegue inicial, la solución se encuentra completamente adaptada y personalizada a las necesidades y dinámicas operativas de la cafetería **Coffee Blinders**.

### 🎯 Objetivo del Sistema

El principal objetivo de la plataforma es resolver las ineficiencias críticas de la atención analógica (demoras por traslados físicos del personal, malentendidos por letra ilegible, pérdidas de comandas en papel y descuadres financieros en los cierres de caja). 

Al centralizar las operaciones en una arquitectura digital integrada de solicitud y respuesta, el sistema aporta valor en cada eslabón del negocio:
* **Autonomía al Cliente:** Permite que los usuarios escaneen un código QR físico para realizar pedidos y solicitar la cuenta directamente desde sus dispositivos móviles, acelerando la experiencia de consumo.
* **Sincronización en Producción:** Reemplaza los tickets de papel por terminales de visualización digital en el área de preparación (barra/cocina), organizando los pedidos automáticamente por orden de llegada y prioridad.
* **Optimización del Personal de Salón:** Libera a los mozos de tareas mecánicas de traslado de información, permitiéndoles enfocar sus esfuerzos en la calidad de la atención y en la supervisión del estado del salón en tiempo real.
* **Control Financiero y de Stock Riguroso:** Provee a la administración de un control exacto de insumos actualizados al segundo, junto con cierres de caja guiados ("ciegos") y un panel de auditoría permanente para garantizar la transparencia del negocio.

## 2. Stack Tecnológico

El ecosistema está construido bajo una arquitectura desacoplada y robusta, garantizando la escalabilidad del sistema, la integridad de las transacciones financieras y una experiencia fluida de usuario en todos los dispositivos.

| Capa / Componente | Tecnología / Herramienta | Versión / Ámbito |
| :--- | :--- | :--- |
| **Arquitectura General** | Cliente-Servidor (Solicitud-Respuesta) | Api Rest Asíncrona |
| **Backend (Servidor)** | Spring Boot | 4.0.X |
| **Gestor de Dependencias** | Maven | Integrado en Backend |
| **Base de Datos** | PostgreSQL | Relacional / Transaccional |
| **Frontend Web (KDS / Admin)** | TypeScript (React) (Next.js) | Vistas de Producción y Control |
| **Frontend Móvil (Cliente / Mozo)**| React Native (Expo) | Entornos Móviles Multiplataforma |
| **Lenguaje de Programación** | Java | 21 |
| **Entorno de Desarrollo (IDE)** | IntelliJ IDEA | Community Edition (Gratuito) |
| **Control de Versiones** | Mercurial | Gestión de Código Fuente |
| **Entornos de Trabajo** | Linux Devuan Excalibur / Windows 10/11 | Sistemas de Desarrollo y Pruebas |

## 3. Requisitos Previos e Instalación

Para poner en marcha el entorno de desarrollo local, asegúrese de cumplir con los siguientes componentes de software instalados en su sistema operativo (**Linux Devuan Excalibur** o **Windows 10/11**).

### 📋 Requisitos Previos

* **Java Development Kit (JDK):** Versión 21 instalado y configurado en las variables de entorno (`JAVA_HOME`).
* **Apache Maven:** Versión 3.9 o superior para la gestión del ciclo de vida del backend.
* **PostgreSQL:** Versión 15 o superior ejecutándose localmente o en un contenedor.
* **Node.js & npm:** Versión 20.x o superior (necesario para las dependencias del ecosistema frontend).
* **Mercurial:** Herramienta de control de versiones instalada (`hg`).

PENDIENTE - EN DESARROLLO...
### ⚙️ Instalación y Configuración del Servidor (Backend)
### 🖥️ Instalación y Configuración del Frontend

PENDIENTE - EN DESARROLLO...
## 4. Variables de Entorno y Configuración

PENDIENTE - EN DESARROLLO...
## 5. Estructura del Proyecto

PENDIENTE - EN DESARROLLO...
## 6. Endpoints de la API

La comunicación entre las aplicaciones cliente y el servidor central se realiza a través de peticiones HTTP asíncronas.

### 📱 Módulo 1: Gestión de Mesas y Sesiones (Cliente / Mozo)
Destinado a los flujos de apertura de mesa mediante códigos QR, solicitudes de asistencia y control del estado del salón.

### ☕ Módulo 2: Comandas y Producción (Pedidos / KDS)
Gestión transaccional de los consumos realizados en el establecimiento y su visualización en pantallas de barra o cocina.

### 🔒 Módulo 3: Seguridad, Personal y Auditoría (Administración / Cajero)
Endpoints restringidos para el control de accesos basados en roles (RBAC), cierres financieros y auditoría de datos.

---

EN DESARROLLO
## 7. Estado del Proyecto y Sprint Actual

El desarrollo del sistema se gestiona mediante metodologías ágiles divididas en ciclos de incremento tecnológico (Sprints). Actualmente, el proyecto se encuentra en una etapa de transición crucial, habiendo completado la fase analítica y de diseño visual para dar inicio a la construcción del núcleo del servidor.

### 📊 Matriz de Estado de Módulos

| Épica / Componente | Estado Operativo | Observaciones / Cobertura |
| :--- | :--- | :--- |
| **Análisis de Requisitos e Historias de Usuario** |  Completado - Revisar | Base conceptual validada para las reglas de negocio de Coffee Blinders. |
| **Arquitectura de Software y Modelado UML** |  Completado - Revisar | Diagramas de casos de uso, secuencia, actividades y clases finalizados. |
| **Diseño Visual e Interfaces (Wireframes)** |  Completado - Revisar | Estructura UI/UX de las apps móviles y el panel web completamente definida. |
| **Estructura y Base de Datos (PostgreSQL)** |  En Progreso | Creación de scripts, esquemas lógicos y mapeo inicial de tablas. |
| **Servidor y API REST (Spring Boot)** |  En Progreso | Inicialización del entorno de persistencia y controladores esenciales. |
| **Aplicación Móvil (Clientes y Mozos)** | ⏳ Pendiente | Segunda fase (Alineada al consumo de los endpoints síncronos). |
| **Panel Web (KDS y Administración)** | ⏳ Pendiente | Segunda fase (Vistas de producción de barra y control de personal). |
| **Pruebas Unitarias e Integración** | ⏳ Pendiente | Planificado para ejecutarse en paralelo con la lógica de servicios. |

---

### 🚀 Sprint Actual

* **Sprint Activo:** Sprint 3 — Construcción del Núcleo del Servidor y Persistencia Transaccional. Backend con SpringBoot
* **Hitos del Periodo:**
  1. Inicialización y hosting del repositorio oficial del proyecto dentro de la plataforma interna **Kallithea**.
  2. Configuración del proyecto base con Maven e inyección de dependencias de seguridad y persistencia relacional.
  3. Desarrollo de la arquitectura de capas base (`Controllers`, `Services`, `Repositories` y `Models`).
* **Sprints Anteriores (Historial):**
  * **Sprint 1 (Completado):** Relevamiento de campo, ingeniería de requerimientos (RF/RNF) y redacción formal de historias de usuario bajo estándar Gherkin.
  * **Sprint 2 (Completado):** Maquetación e interconexión de interfaces visuales de usuario (Wireframes), junto con el desarrollo de diagramas de casos de uso, clases generales, actividades y secuencia.

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


