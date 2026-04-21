# the-mauricio-anomaly-case

## 🎬 We Need to Talk About Mauricio

### 🔍 Exploratory Data Analysis: Restaurant Performance & Server Anomalies

<details>
<summary>🇲🇽 <b>Versión en Español (Resumen Completo del Proyecto)</b></summary>

## Project Overview
El objetivo de este proyecto es realizar un análisis forense de datos (EDA) sobre las ventas de un restaurante durante el periodo 2014-2015. El reto principal fue identificar inconsistencias operativas y analizar la productividad del personal de servicio.

El proyecto se centra en la detección de la **"Anomalía de Mauricio"**, un patrón de datos inusual donde un mesero clave presenta vacíos críticos en sus registros de ventas, lo que permitió auditar la integridad de los sistemas de captura y la continuidad del personal.

## 🛠 Tech Stack
* **Language:** Python 3.x
* **Libraries:** * `Pandas` & `NumPy`: Limpieza de datos (ETL), tratamiento de valores nulos y normalización de columnas.
    * `Matplotlib` & `Seaborn`: Visualización de matrices de calor (Heatmaps) y tendencias temporales.
    * `Unidecode / Regex`: Procesamiento de texto para estandarizar nombres de columnas con caracteres especiales.
* **Environment:** Jupyter Notebook / Pop!_OS.

## 📈 Key Process
1. **Data Cleaning (ETL):** Normalización de nombres de columnas eliminando acentos, espacios y convirtiendo a minúsculas mediante un mapeo optimizado para evitar errores de codificación.
2. **Feature Engineering:** Extracción de componentes temporales (Año, Mes) y creación de tablas dinámicas (`pivot_table`) para cruzar ventas totales por mesero.
3. **Heatmap Analysis:** Generación de mapas de calor para visualizar la densidad de ventas. Se aplicó formato `.0f` para eliminar decimales y mejorar la legibilidad de las métricas de ingresos.
4. **Anomaly Detection:** Comparativa mensual entre empleados para identificar periodos de inactividad o fallos en el registro de comandas.

---

## 💡 Conclusions
* **Identificación de la Anomalía:** Se detectó que, a diferencia del resto del staff, Mauricio presenta una ausencia total de datos en periodos específicos de 2014, lo que sugiere errores administrativos o una gestión inconsistente de turnos.
* **Rendimiento Operativo:** El análisis de los mapas de calor permitió ver que las ventas están altamente concentradas en ciertos meseros, identificando cuellos de botella durante las horas pico.
* **Calidad de los Datos:** La estandarización inicial de las columnas previno errores de "KeyError" y facilitó un flujo de análisis reproducible.

## 🚀 Recommendations
1. **Auditoría de Sistemas:** Implementar validaciones en tiempo real en el sistema de comandas para asegurar que cada transacción esté vinculada correctamente a un mesero activo.
2. **Optimización de Turnos:** Utilizar la estacionalidad detectada en el Heatmap para reforzar el personal durante los meses de mayor demanda, basándose en el desempeño histórico.
3. **Seguimiento de Retención:** Investigar las causas de los "huecos" en los registros de Mauricio para determinar si se trata de rotación de personal o fallas técnicas en la asignación de mesas.
4. **Dashboard de Monitoreo:** Desarrollar un tablero en tiempo real para que la gerencia pueda detectar anomalías de ventas en la misma semana que ocurren.
</details>

---

<details>
<summary>🇺🇸 <b>English Version (Full Project Overview)</b></summary>

# The Mauricio Anomaly Case: Restaurant Sales EDA 🔍

## Project Overview
The objective of this project was to conduct a forensic **Exploratory Data Analysis (EDA)** on a restaurant's sales dataset from 2014-2015. The primary focus was identifying operational inconsistencies and analyzing the productivity of the service staff.

The project is highlighted by the **"Mauricio Anomaly"**, an unusual data pattern where a key server showed critical gaps in sales records. This finding served as a catalyst for auditing data integrity and staff continuity.

## 🛠 Tech Stack
* **Libraries:** `Pandas` & `NumPy` (ETL, Null handling, Column normalization), `Matplotlib` & `Seaborn` (Heatmap visualizations and temporal trends), `Unidecode / Regex` (Text processing for special character standardization).

## 💡 Conclusions
* **Anomaly Detection:** The analysis revealed that, unlike the rest of the staff, Mauricio showed a total absence of data during specific months in 2014, suggesting administrative errors or inconsistent shift management.
* **Operational Performance:** Heatmap analysis identified that sales are highly concentrated among certain servers, highlighting bottlenecks during peak hours.
* **Data Quality:** Proactive column standardization prevented encoding errors and ensured a reproducible analysis workflow.

## 🚀 Recommendations
* **System Auditing:** Implement real-time validations in the ordering system to ensure every transaction is correctly linked to an active server.
* **Shift Optimization:** Leverage the seasonality detected in the Heatmap to reinforce staffing during high-demand months based on historical performance.
* **Retention Tracking:** Investigate the root causes of Mauricio's record gaps to determine if they stem from staff turnover or technical failures in table assignments.
* **Monitoring Dashboard:** Develop a real-time dashboard for management to detect sales anomalies within the week they occur.

</details>

---
**Author:** [Daniel Perez](https://edanielprz.info) | Data Analyst