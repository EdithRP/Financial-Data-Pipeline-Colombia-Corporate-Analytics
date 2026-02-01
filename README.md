# Financial Data Pipeline: Colombia Corporate Analytics 📊🇨🇴

## 📝 Project Overview
Este proyecto implementa un flujo de datos **End-to-End** diseñado para extraer, procesar y visualizar la salud financiera de empresas colombianas. 

El sistema utiliza a **Rappi** como caso de estudio inicial, pero está arquitectado para ser dinámico: mediante el ingreso del **NIT**, el pipeline automatiza la generación de insights financieros clave, permitiendo una auditoría rápida y técnica de cualquier entidad registrada en las bases de datos oficiales.

## 🏗️ Technical Architecture
El proyecto sigue una arquitectura de nube híbrida optimizada para eficiencia de costos y rendimiento:

1.  **Data Ingestion:** Scripts de Python utilizando la librería `sodapy` para consumir la API de **Socrata** (Datos Abiertos Colombia).
2.  **ELT Process:** Transformación y limpieza de datos con `Pandas`, aplicando principios **DRY (Don't Repeat Yourself)** para asegurar un código mantenible y escalable.
3.  **Data Persistence:** Almacenamiento robusto en una base de datos **PostgreSQL**.
4.  **Reporting & Visualization:** Reportes dinámicos en **Power BI Service**, conectados mediante un **On-premises Data Gateway** para garantizar que los datos fluyan desde el entorno local a la nube.


## 🌟 Key Features
* **Consulta por NIT:** Capacidad de parametrizar la extracción para obtener datos específicos de cualquier empresa.
* **Procesamiento Eficiente:** Lógica de transformación modular que prepara los estados financieros para análisis de ratios e indicadores de liquidez.
* **Visualización Proactiva:** Dashboard en Power BI diseñado para resaltar automáticamente los insights más importantes (EBITDA, margen neto, apalancamiento).
* **Escalabilidad con n8n:** Arquitectura preparada para integrar automatización de flujo de trabajo (n8n) en fases futuras.

## 🛠️ Technologies Used
* **Python:** (Sodapy, Pandas, SQLAlchemy)
* **Database:** PostgreSQL
* **BI Tool:** Power BI & Power BI Gateway
* **Environment:** Conda (macOS para desarrollo / Windows para BI)
* **Version Control:** Git & GitHub

