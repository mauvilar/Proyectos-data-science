# Proyectos de data science · Mauricio Vilar

Los notebooks ejecutados de mis proyectos de data science, con el código, las salidas y las gráficas tal
como corrieron. Los proyectos propios traen además el snapshot de datos con fecha, para que cualquier
cifra se pueda rastrear hasta su origen.

La forma más cómoda de recorrerlos es el portafolio: **https://mauvilarlandingpage.vercel.app**

## Proyectos propios

| Proyecto | Carpeta | De qué trata |
|---|---|---|
| Nearshoring en cifras: la inversión extranjera directa en México, 2006 a 2025 | [ied-nearshoring-mx](ied-nearshoring-mx/) | Proyecto propio sobre la API del datastore de datos.gob.mx (Secretaría de Economía): descarga paginada de ocho tablas, desacumulación de montos, confidenciales como nulos, conciliación al decimal contra los boletines y el informe trimestral, y una serie en dólares constantes con el CPI-U de FRED. En 2025 la IED sumó 40,812 mdd, el segundo año de veinte en dólares corrientes y el décimo en dólares de 2025, con 68 % de reinversión de utilidades contra 37 % de promedio 2006 a 2018. La Ciudad de México pasó de 20 % a 53 % de la IED y fuera de ella llegaron 19,209 mdd, el cuarto monto más bajo de la serie; seis estados sumaron el 80 % (nueve sin la capital). Las cifras de 2024 y 2025 son preliminares, así que el mínimo de nuevas inversiones de 2024 se presenta con su margen de revisión (4.9 %). Incluye el snapshot de datos con fecha. |
| ¿Cuánto se gana en México? El salario que registra el IMSS, 2018 a 2026 | [salarios-imss-mx](salarios-imss-mx/) | Datos Abiertos del IMSS: cinco cortes de agosto (2018 a 2026), archivos de 300 a 400 MB y 23 millones de filas procesados con Polars, validados contra el boletín del IMSS. El salario base de cotización está topado a 25 UMA (2.3 % de los puestos cotiza el tope y carga 10 % de la masa salarial), así que cada promedio se trata como cota inferior y se acompaña de la mediana y los cuartiles calculados desde los rangos salariales. El salario mínimo pasó de 2.5 veces la mediana a 1.7, y los puestos que cotizan a dos mínimos o menos pasaron de 40 % a 69 %. |
| Mercado de trabajo de IA: México vs Estados Unidos | [mercado-ia-mx-us](mercado-ia-mx-us/) | Corpus propio vía la API de Adzuna combinado con un dataset real de Kaggle, después de auditar las fuentes públicas (incluida la autopsia de un dataset sintético). Brecha salarial entre México y cinco áreas metropolitanas de Estados Unidos con intervalos de confianza bootstrap, primas por skill, y un modelo de imputación descartado a propósito porque no supera la validación contra un hold-out de 4 salarios mexicanos. |
| Riesgo crediticio: scoring de impago | [credit-risk-scoring](credit-risk-scoring/) | *Default of Credit Card Clients* (UCI, 30,000 tarjetahabientes de Taiwán, 2005): análisis exploratorio con prueba explícita de fuga de datos y partición estratificada reproducible, e ingeniería de 15 variables derivadas validadas por su ROC AUC univariado. `comparison.json` guarda la comparación de modelos de la fase de modelado, donde gana XGBoost con ROC AUC 0.783 en test. |

## Proyecto final del bootcamp

| Proyecto | Carpeta | De qué trata |
|---|---|---|
| Telecomunicaciones: operadores ineficaces | [Telecomunicaciones-Operadores-Ineficaces](Telecomunicaciones-Operadores-Ineficaces/) | Identificación de operadores ineficaces en un call center (EDA y clasificación), una prueba A/B sobre un sistema de recomendaciones y un bloque de consultas SQL. Incluye el plan de descomposición de tareas. |

## Formación: sprints del bootcamp de TripleTen

| Sprint | Proyecto | Qué se practica |
|---|---|---|
| [Sp_14](Sp_14/) | Model Fitness: churn y segmentación | Clasificación para predecir cancelaciones y segmentación con clustering jerárquico y K-Means. |
| [Sp_12](Sp_12/) | Embudo de eventos y test A/A/B | Embudo de conversión a partir de logs y evaluación de un test A/A/B. |
| [Sp_11](Sp_11/) | Test A/B | Priorización de hipótesis (ICE y RICE) y significancia entre grupos. |
| [Sp_10](Sp_10/) | Showz: análisis de marketing | Cohortes, retención, LTV, CAC y ROI por fuente de adquisición. |
| [Sp_8](Sp_8/) | Zuber: taxis en Chicago | Datos extraídos con SQL, demanda por barrio y empresa, y prueba de Welch sobre la duración de viajes con mal clima. |
| [Sp_6](Sp_6/) | Tienda de videojuegos | Patrones de éxito por plataforma, género y región, y pruebas de hipótesis sobre calificaciones. |
| [Sp_5](Sp_5/) | Megaline: ¿cuál es la mejor tarifa? | Estadística descriptiva e inferencial para comparar dos tarifas y sus ingresos. |
| [Sp_4](Sp_4/) | Instacart: llena ese carrito | EDA de pedidos: ausentes, duplicados y comportamiento de compra. |
| [Sp_3](Sp_3/) | Déjame escuchar música | Hábitos musicales en dos ciudades y prueba de hipótesis sobre días y géneros. |
| [Sp_2](Sp_2/) | Store 1: segunda fase | Python puro: listas anidadas, funciones y agregaciones para perfilar clientes. |
| [Sp_1](Sp_1/) | Store 1: primera fase | Limpieza de cadenas y manejo de listas y diccionarios. |

## Herramientas

Python 3.12 con pandas, Polars, NumPy, SciPy, scikit-learn, matplotlib, seaborn, requests y SQLAlchemy.
Jupyter, jupytext y `uv` para entornos reproducibles. Las gráficas de los proyectos propios usan la
identidad Editorial v3 de NyxAI Studio.

## Autor

Mauricio Vilar Giribet · [github.com/mauvilar](https://github.com/mauvilar) · [portafolio](https://mauvilarlandingpage.vercel.app)
