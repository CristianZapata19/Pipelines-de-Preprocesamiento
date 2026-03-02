# Finance Trends Analysis & Machine Learning Pipeline 
## Este proyecto presenta un análisis exploratorio de datos (EDA) y la implementación de un Pipeline de procesamiento de extremo a extremo (End-to-End) utilizando Scikit-Learn. El objetivo es procesar tendencias financieras de inversión y preparar los datos para modelos predictivos de manera automatizada y escalable.

### Objetivos del Proyecto
- EDA Interactivo: Visualización de tendencias de inversión, distribución de género y expectativas de retorno.
- Ingeniería de Características: Implementación de un ColumnTransformer para manejar datos mixtos (numéricos y categóricos).
- Automatización: Uso de Pipeline para garantizar la reproducibilidad y evitar el Data Leakage.
- Personalización: Creación de un FunctionTransformer para inyectar lógica de negocio específica en el flujo de datos.

### Estructura del Pipeline
El flujo de procesamiento se divide en tres ramas principales que convergen en un modelo de clasificación:

- Rama Numérica: Imputación de valores faltantes por mediana y escalado estándar (StandardScaler).
- Rama Categórica: Imputación por valor más frecuente y codificación binaria (OneHotEncoder).
- Rama Personalizada: Transformador de funciones para segmentar perfiles de alta expectativa de retorno.

### Resultados y Conclusiones
- Robustez Técnica: El uso de pipelines permite que el modelo procese datos "sucios" o incompletos automáticamente sin errores de ejecución.
- Interpretabilidad: Gracias al método get_feature_names_out, podemos rastrear exactamente cómo influye cada variable original en la decisión final del modelo.
- Escalabilidad: El sistema está diseñado para integrarse con herramientas de despliegue, permitiendo pasar de datos crudos a predicciones en un solo paso.
