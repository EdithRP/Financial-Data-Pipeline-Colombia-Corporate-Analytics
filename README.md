# Financial Data Pipeline: Colombia Corporate Analytics 📊🇨🇴

## 📝 Project Overview
Este proyecto está diseñado para centralizar y analizar la salud financiera de las empresas en Colombia. Utilizando la API de **Datos Abiertos (Socrata)**, el pipeline automatiza la captura de estados financieros, transformando datos crudos en insights accionables mediante un proceso robusto de ETL (Extract, Transform, Load).

El objetivo principal es permitir una exploración profunda de indicadores financieros clave a nivel nacional, facilitando la toma de decisiones basada en datos.

## 🏗️ Technical Architecture
El flujo de datos se divide en tres capas principales para garantizar la integridad y eficiencia:

1.  **Data Source Layer:** Conexión y autenticación con la API de Datos Abiertos de entidades gubernamentales colombianas.
2.  **Processing Layer (macOS):** * **Python:** Limpieza, normalización de cifras y manejo de tipos de datos financieros con `Pandas`.
    * **PostgreSQL:** Estructuración de datos en un modelo relacional optimizado para consultas.
3.  **Visualization Layer (Windows):** * **Power BI:** Conexión remota a la base de datos para modelado de datos y diseño de dashboards interactivos.

## 🌟 Key Features
* **Extracción Automatizada:** Implementación de peticiones paginadas para manejar grandes volúmenes de datos financieros.
* **Integración Híbrida:** Desarrollo optimizado utilizando macOS para el procesamiento de datos y Windows para la visualización avanzada en Power BI.
* **Base de Datos Estructurada:** Almacenamiento en PostgreSQL que permite análisis históricos y comparativos eficientes.
* **Insights Sectoriales:** Capacidad de segmentar el análisis por sector económico, ubicación geográfica y periodos fiscales.

## 🛠️ Technologies Used
* **Python 3.10:** (Pandas, Requests, SQLAlchemy, Psycopg2)
* **PostgreSQL:** Motor de base de datos relacional.
* **Conda:** Gestión de entornos virtuales.
* **Git/GitHub:** Control de versiones.
* **Power BI:** Business Intelligence, modelado y DAX.

---
