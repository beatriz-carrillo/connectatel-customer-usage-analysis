
# 📊 ConnectaTel | Análisis de Consumo y Segmentación de Clientes

**Proyecto de Data Analytics | Python · Pandas · NumPy · Matplotlib · Seaborn**

Análisis exploratorio del comportamiento de clientes de telecomunicaciones en México y Colombia, enfocado en identificar patrones de consumo, detectar valores atípicos y generar recomendaciones comerciales basadas en datos.

## 🎯 Objetivo del proyecto

Analizar la actividad de llamadas y mensajes de los clientes de ConnectaTel para construir perfiles estadísticos, identificar segmentos de consumo y detectar comportamientos inusuales que permitan orientar futuras decisiones comerciales.

**Periodo de análisis:** Datos disponibles hasta 2024.

## 📂 Datasets utilizados

| Archivo | Contenido |
|---|---|
| `plans.csv` | Información de los planes de servicio, precios y beneficios incluidos. |
| `users.csv` | Datos demográficos de clientes, ciudad, fecha de registro, plan contratado y churn. |
| `usage.csv` | Registros de llamadas y mensajes, fechas y duración de las llamadas. |

Se analizaron 4,000 clientes y 40,000 registros de actividad, integrando la información por usuario.

## 🛠️ Herramientas y habilidades

- **Python:** desarrollo del análisis y automatización de operaciones.
- **Pandas y NumPy:** preparación, limpieza, transformación e integración de datos.
- **Matplotlib y Seaborn:** visualización de distribuciones y patrones de comportamiento.
- **Estadística descriptiva:** medidas de tendencia central, dispersión y cuartiles.
- **Método IQR:** detección de valores atípicos.
- **Segmentación:** clasificación de clientes por edad y nivel de consumo.

## 🔎 Metodología

1. **Exploración:** revisión de estructura, tipos de datos y calidad de los tres datasets.
2. **Limpieza:** tratamiento de valores faltantes, sentinels y fechas inconsistentes.
3. **Transformación:** creación de indicadores de llamadas y mensajes por cliente.
4. **Integración:** consolidación de actividad con datos demográficos mediante `merge`.
5. **Análisis estadístico:** cálculo e interpretación de medidas descriptivas.
6. **Visualización:** histogramas, boxplots y gráficos de distribución.
7. **Detección de outliers:** aplicación del rango intercuartílico (IQR).
8. **Segmentación:** clasificación por edades y nivel de actividad.
9. **Conclusiones:** interpretación de hallazgos y recomendaciones comerciales.

## 📈 Hallazgos principales

### Segmentación por consumo

| Segmento | Clientes | Participación |
|---|---:|---:|
| Uso medio | 2,943 | 73.58% |
| Bajo uso | 778 | 19.45% |
| Alto uso | 278 | 6.95% |
| Sin datos de uso | 1 | 0.03% |

**Hallazgo:** El segmento de uso medio concentra la mayoría de los clientes. Esto representa una oportunidad para evaluar la adecuación de los planes comerciales a sus patrones de consumo.

### Segmentación por edad

| Grupo | Clientes | Participación |
|---|---:|---:|
| Jóvenes (menores de 30 años) | 760 | 19.00% |
| Adultos (30–59 años) | 2,018 | 50.45% |
| Adultos mayores (60 años o más) | 1,222 | 30.55% |

**Hallazgo:** Los adultos de 30 a 59 años representan el principal grupo demográfico.

### Identificación de valores atípicos

- Se detectaron **109 registros de usuarios** por encima del límite superior IQR de minutos acumulados.
- El umbral superior calculado fue de **61.86 minutos**.
- El máximo observado fue de **155.69 minutos**.
- Los valores atípicos se conservaron, ya que pueden representar comportamientos válidos de clientes con mayor actividad.

## 💼 Recomendaciones de negocio

1. **Optimización de planes:** evaluar los beneficios de los planes para el segmento predominante de uso medio.
2. **Ofertas diferenciadas:** explorar alternativas flexibles para clientes de bajo consumo y beneficios adicionales para clientes de alto consumo.
3. **Segmentación comercial:** profundizar en las diferencias de consumo por edad y plan contratado.
4. **Monitoreo de patrones inusuales:** analizar casos extremos antes de tratarlos como errores.
5. **Retención:** ampliar el estudio incorporando churn, ingresos y rentabilidad de clientes.

## ⚠️ Consideraciones y limitaciones

El análisis se concentra en llamadas y mensajes registrados. Las diferencias de consumo por plan, la rentabilidad y las causas de abandono requieren evaluaciones adicionales.

Un valor atípico estadístico no demuestra por sí mismo la existencia de fraude o errores operativos.

## ▶️ Abrir el análisis en Google Colab

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/beatriz-carrillo/connectatel-customer-usage-analysis/blob/main/ConnectaTel_Customer_Usage_Analysis.ipynb)

También puedes consultar directamente el Notebook:

[Ver Notebook de ConnectaTel](ConnectaTel_Customer_Usage_Analysis.ipynb)

## 🔄 Guía de reproducción

1. Abrir el Notebook mediante el botón **Abrir en Colab**.
2. Disponer de los archivos `plans.csv`, `users.csv` y `usage.csv`.
3. Cargar los datasets en el entorno de ejecución y verificar que sus rutas coincidan con las utilizadas en el Notebook.
4. Instalar las librerías necesarias si no están disponibles.
5. Seleccionar **Entorno de ejecución → Ejecutar todas**.
6. Revisar los resultados, gráficos, segmentaciones y conclusiones.

**Nota:** Los archivos de datos no se incluyen en este repositorio. Su disponibilidad y publicación dependen de los permisos de distribución correspondientes.

## 📌 Estado del proyecto

**Proyecto finalizado y publicado en GitHub desde Google Colab.**

El Notebook documenta el proceso de preparación, exploración, análisis estadístico, segmentación e interpretación de resultados.

## 👩‍💻 Autora

**Beatriz Carrillo García**

Data Analytics | Business Intelligence | FP&A

[LinkedIn](https://www.linkedin.com/in/beatriz-carrillo-garcia-a83a3718/)

---

*Transformando datos en información estratégica para la toma de decisiones.*
