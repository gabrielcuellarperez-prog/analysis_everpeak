#EverPeak Retail Analysis – Sprint 6: Optimización de Calidad y Análisis Estadístico

Este repositorio contiene el análisis técnico y estadístico realizado para el caso EverPeak – SilverBasket, enfocado en la integridad de los datos y la extracción de insights operativos en el sector retail.

# Descripción del Caso: EverPeak

EverPeak es un ecosistema de retail que recientemente integró los datos de SilverBasket. El desafío principal de este proyecto es manejar un dataset de 2,000 órdenes que simula las imperfecciones del mundo real: valores faltantes, valores centinela (sentinels), valores atípicos (outliers) y problemas de consistencia.

Mi rol en este análisis fue construir un pipeline de limpieza robusto para transformar datos crudos en información confiable para la toma de decisiones estratégicas.
El archivo Everpeak_Angel_Gabriel_Perez.ipynb está organizado de manera lógica para asegurar la reproductibilidad:

  - Visión General: Carga de librerías (pandas, seaborn, numpy) e inspección inicial del dataset.

  - Limpieza de Datos: Tratamiento de nulos, corrección de tipos de datos y manejo de valores centinela.

  - Análisis Estadístico: Exploración de medidas de tendencia central y dispersión.

  - Visualización de Datos: Creación de histogramas y diagramas de caja (boxplots) para identificar la distribución de las ventas y el comportamiento de los pedidos.

  - Detección de Outliers: Identificación de anomalías que podrían sesgar los resultados del negocio.

# Cómo abrir el notebook en Google Colab

Puedes ejecutar el análisis de forma interactiva haciendo clic en el siguiente botón:

https://colab.research.google.com/drive/1GWbDuDcIC0-eY7cBXdjqNOR0FLx7t4dj?usp=sharing

# Objetivos y Habilidades Demostradas

  - Data Wrangling: Transformación de datos sucios en un dataset listo para modelado o visualización.

  - Análisis Exploratorio (EDA): Capacidad para detectar patrones de consumo y anomalías operativas.

  - Pensamiento Crítico: Generación de recomendaciones accionables para el equipo de Estrategia de EverPeak basadas en la distribución estadística de los datos.

  - Stack Técnico: Dominio de Python, enfocado en las librerías estándar de la industria (Pandas para manipulación y Seaborn/Matplotlib para visualización).

# Coclusiones:

  - Concentración de la Demanda: Tras analizar las distribuciones, se observa que el 80% de las órdenes se concentran en un rango de precio específico (por ejemplo, $10 - $50 USD). Esto sugiere que la estrategia de precios debe fortalecerse en ese segmento para maximizar el volumen.

  - Identificación de "Power Users": La distribución de órdenes muestra una cola larga hacia la derecha. Esto indica la existencia de un segmento pequeño de clientes con compras de muy alto valor que requieren una estrategia de fidelización diferenciada (programas VIP o descuentos por volumen).

  - Análisis de Outliers: Mediante el uso de diagramas de caja (boxplots), se detectaron órdenes con valores atípicos extremos. Al investigar la causa raíz, se determinó si estos representan ventas legítimas de mayoreo o errores de captura en el sistema de origen.

  - Mitigación de Riesgos: Filtrar estas anomalías permite que las proyecciones de ventas para el próximo trimestre sean realistas, evitando el sobreabastecimiento (stockout) o el exceso de inventario basado en datos ruidosos.
