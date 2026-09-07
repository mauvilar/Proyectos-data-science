# Proyectos Data Science

Recopilación de proyectos del bootcamp de Data Science de TripleTen. Cada carpeta `Sp_*` corresponde a un sprint y contiene el notebook con el análisis correspondiente.

## Índice de proyectos

| Sprint | Proyecto | Tipo de análisis |
|--------|----------|------------------|
| [Sp_1](Sp_1/) | Store 1 — Primera fase | Limpieza de strings y manipulación de listas/diccionarios para preparar datos de clientes. |
| [Sp_2](Sp_2/) | Store 1 — Segunda fase | Procesamiento avanzado en Python puro: listas anidadas, funciones y agregaciones para perfilar clientes y categorías de compra. |
| [Sp_3](Sp_3/) | Déjame escuchar música | Análisis exploratorio con pandas: hábitos musicales de usuarios en dos ciudades, prueba de hipótesis sobre días de la semana y géneros. |
| [Sp_4](Sp_4/) | Instacart — Llena ese carrito | EDA completo de pedidos de comestibles: limpieza, valores ausentes y duplicados, y análisis de comportamiento de compra. |
| [Sp_5](Sp_5/) | Megaline — ¿Cuál es la mejor tarifa? | Estadística descriptiva e inferencial: comparación de tarifas Surf vs. Ultimate y prueba de hipótesis sobre ingresos. |
| [Sp_6](Sp_6/) | Tienda de videojuegos | EDA y análisis de patrones de éxito por plataforma, género y región; pruebas de hipótesis sobre calificaciones de usuarios. |
| [Sp_8](Sp_8/) | Zuber — Taxis en Chicago | Análisis de datos extraídos vía SQL, visualización de demanda por barrio/empresa y prueba de hipótesis (Welch t-test) sobre duración de viajes con clima adverso. |
| [Sp_10](Sp_10/) | Showz — Análisis de marketing | Métricas de producto y marketing: cohortes, retención, LTV, CAC y ROI por fuente de adquisición. |
| [Sp_11](Sp_11/) | Test A/B | Análisis estadístico de un test A/B: priorización de hipótesis (ICE/RICE) y evaluación de significancia entre grupos. |
| [Sp_12](Sp_12/) | Embudo de eventos y test A/A/B | Análisis de logs de eventos: construcción de embudo de conversión y evaluación de un test A/A/B. |
| [Sp_14](Sp_14/) | Model Fitness — Churn y segmentación | Machine learning: predicción de cancelación de clientes (clasificación) y segmentación mediante clustering jerárquico/K-Means. |
| [Telecomunicaciones — Operadores Ineficaces](Telecomunicaciones-Operadores-Ineficaces/) | Identificación de operadores ineficaces en un call center | Proyecto integral con tres casos: análisis principal con clasificación de operadores ineficaces (EDA + ML), prueba A/B sobre un sistema de recomendaciones, y resolución de tareas con SQL. Incluye también el plan de descomposición de tareas. |
| [mercado-ia-mx-us](mercado-ia-mx-us/) | Mercado de trabajo de IA: México vs Estados Unidos | Proyecto propio de punta a punta: auditoría de fuentes públicas (incluida la autopsia de un dataset sintético), corpus propio vía la API de Adzuna combinado con un dataset real de Kaggle, brecha salarial entre México y cinco metros de Estados Unidos con intervalos de confianza bootstrap, primas salariales por skill, y un modelo de imputación explícitamente descartado por no superar la validación contra un hold-out de n=4. |
| [credit-risk-scoring](credit-risk-scoring/) | Riesgo crediticio: scoring de impago | Dos fases de un sistema de scoring sobre *Default of Credit Card Clients* (UCI, 30,000 tarjetahabientes de Taiwán, 2005): análisis exploratorio con prueba explícita de fuga de datos y partición estratificada reproducible, e ingeniería de 15 variables derivadas validadas por su ROC AUC univariado. `comparison.json` guarda la comparación de los cuatro modelos de la fase 3, donde gana XGBoost con ROC AUC 0.783 en test. Los notebooks 03 y 04 están escritos pero aún sin ejecutar. |

## Stack utilizado

- **Lenguaje:** Python 3
- **Librerías principales:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `scikit-learn`, `requests`, `pyarrow`
- **Entorno:** Jupyter Notebook · `uv` (gestión de dependencias en `mercado-ia-mx-us`)

## Autor

Mau Vilar — [github.com/mauvilar](https://github.com/mauvilar)
