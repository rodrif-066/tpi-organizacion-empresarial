# Módulo Integrado de Gestión y Sincronización Transaccional de Licencias Digitales (MGDL)
> **Trabajo Práctico Integrador y Progresivo (TPI)**  
> **Asignatura:** Organización Empresarial  
> **Carrera:** Tecnicatura Universitaria en Programación a Distancia (TUP AD)  
> **Institución:** Universidad Tecnológica Nacional (UTN - FRGP)  
> **Caso de Estudio:** CAPCOM Co., Ltd.  

---

## 🔗 Enlaces Rápidos y Accesos Directos

* 📋 **Tablero Ágil del Proyecto (GitHub Projects / Jira):** [Ver Tablero Kanban de Historias de Usuario](https://github.com/users/rodrigofonseca/projects/1)
* 📄 **Documentación Consolidada (PDF):** `docs/tpi_final_consolidado_capcom.pdf`

---

## 📌 Descripción General del Sistema

El **Módulo Integrado de Gestión y Sincronización Transaccional de Licencias Digitales (MGDL)** es una solución tecnológica desarrollada para la empresa multinacional **CAPCOM Co., Ltd.** (Sector Terciario / Software de Entretenimiento). 

El objetivo principal del sistema es autenticar, validar y sincronizar en tiempo real los callbacks transaccionales emitidos por tiendas digitales de terceros (Steam, PlayStation Network, Xbox Network, Nintendo eShop). Al procesar la compra, el módulo valida la firma criptográfica de la clave del producto, habilita el servicio en los servidores de juegos y emite de forma automatizada la entrada contable correspondiente en el ERP de la compañía (reconociendo el ingreso neto en los Activos y en el Patrimonio Neto).

---

## 👥 Integrantes del Proyecto

| Nombre y Apellido | Legajo | Rol en el Proyecto | Usuario GitHub |
| :--- | :---: | :--- | :--- |
| **Rodrigo Agustín Fonseca Arias** | `123456` | Lead Software Architect / Backend Dev | [@rodrigofonseca](https://github.com/rodrigofonseca) |

---

## 🏛️ Cuerpo Docente

* **Docente Titular:** Prof. Gabriela Martínez
* **Docente Adjunta / Tutora:** Prof. Mónica Mut
* **Equipo Docente:** Prof. Carolina Bruno, Prof. Mario Raúl López, Prof. Andrea Ramos

---

## 🗺️ Estructura del Repositorio

```text
├── docs/
│   ├── organigrama_capcom.png
│   ├── diagrama_gantt.png
│   ├── diagrama_bpmn_mgdl.png
│   └── tpi_final_consolidado_capcom.pdf
├── src/
│   ├── backend/
│   │   ├── controllers/
│   │   ├── models/
│   │   └── services/
│   └── database/
│       └── schema.sql
├── README.md
└── .gitignore
```

---

## ⚙️ Arquitectura de Versiones y GitFlow

Para garantizar la trazabilidad del trabajo colaborativo se implementó la metodología **GitFlow** mediante el uso de ramas secundarias y Pull Requests (PR):

* `main`: Rama de producción con releases estables.
* `develop`: Rama principal de integración de características.
* `feature/modelo-datos`: Creación y formalización del Diccionario de Datos (PK/FK).
* `feature/bpmn-proceso`: Modelado de procesos de negocio en BPMN 2.0.
* `fix/gateway-decision-bpmn`: Corrección de flujo en compuertas de excepción.

### Convención de Commits Utilizada
Se adoptó la convención **Conventional Commits**:
* `feat:` Nuevas funcionalidades desarrolladas.
* `fix:` Corrección de errores en código o modelos.
* `docs:` Modificaciones en documentación (`README.md`, PDFs).
* `chore:` Tareas auxiliares y configuración del repositorio.

---

## 📊 Backlog del Proyecto y Historias de Usuario

Las tareas e Historias de Usuario fueron gestionadas en un tablero interactivo tipo Kanban divididas en los estados **Por Hacer (To Do)**, **En Progreso (In Progress)** y **Listo (Done)**:

1. **HU-01 (Autenticación de Licencias):** *Como* backend del módulo MGDL, *quiero* recibir y validar el callback transaccional de las tiendas distribuidoras, *para* habilitar el acceso al cliente con una latencia menor a 500 ms. `[Estado: LISTO]`
2. **HU-02 (Registro Contable ERP):** *Como* gerente financiero, *quiero* que cada venta sincronizada genere automáticamente un asiento en el ERP, *para* eliminar descalces entre balances mensuales y reportes de tiendas. `[Estado: LISTO]`
3. **HU-03 (Auditoría Ciberseguridad y GDPR):** *Como* especialista de Staff de Ciberseguridad, *quiero* auditar los eventos transaccionales encriptados, *para* asegurar el cumplimiento de normativas internacionales de protección de datos. `[Estado: EN PROGRESO]`

---

## 🤖 Declaración de Transparencia sobre el Uso de Inteligencia Artificial

De acuerdo a las pautas de transparencia de la cátedra de Organización Empresarial:

1. **Herramienta Utilizada:** Generadores de Código / Modelos de Lenguaje (LLM).
2. **Propósito Específico:** 
   * Asistencia en el maquetado estético de tablas de markdown y estructura formal del repositorio.
   * Generación vectorial auxiliar (SVG) para esquemas BPMN y de la matriz FODA.
3. **Control y Revisión Humana:** Todo el marco teórico referente a la Teoría General de Sistemas (TGS), la modelación del tramo de control de la empresa CAPCOM Co., Ltd., el diseño de Claves Primarias/Foráneas y los criterios de evaluación KPI del módulo MGDL fueron redactados, validados y revisados de forma crítica por el alumno.