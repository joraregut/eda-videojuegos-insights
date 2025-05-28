# EDA de Ventas de Videojuegos para Ice: Identificando Patrones de Éxito

Desarrollé un Análisis **Exploratorio de Datos** (EDA) exhaustivo para Ice, una **tienda global de videojuegos**, con el objetivo de comprender a fondo los factores que impulsan el éxito en la industria. El proyecto se centró en un dataset rico en **información histórica** (hasta diciembre de 2016), que incluye datos de ventas, reseñas de usuarios y expertos, géneros, plataformas (como Xbox y PlayStation) y la clasificación ESRB de cada juego.

Para llevar a cabo este análisis, **utilicé un conjunto de herramientas y librerías clave** en **Python**. Empleé `Pandas` para la manipulación y organización eficiente de los datos, y `NumPy` para operaciones numéricas complejas. La visualización de los patrones y tendencias se realizó con `Matplotlib` y `Seaborn`, permitiendo una comprensión intuitiva de las **relaciones entre las variables**. Además, utilicé la librería `SciPy` para realizar **análisis estadísticos** que ayudaron a validar las hipótesis y extraer inferencias significativas.

Mi objetivo principal fue **identificar los patrones de éxito** de los videojuegos a través de una exploración profunda de estos datos. Los hallazgos derivados de este EDA son cruciales y permitirán a Ice la **detección temprana de títulos prometedores** y la **optimización de sus estrategias de marketing** para 2017. Asegurando así decisiones basadas en evidencia, la planificación de futuras campañas más precisa y efectiva.


# Problema de Negocio / Motivación, por qué este análisis es importante para Ice.

La industria de los videojuegos es dinámica y competitiva. Ice, como tienda online global, necesita entender qué factores impulsan el éxito de un juego para tomar decisiones estratégicas en marketing y selección de inventario. Este proyecto aborda la necesidad de identificar patrones de rendimiento para optimizar la inversión en campañas publicitarias.

# Objetivos del Análisis.
- Identificar las tendencias de ventas a lo largo del tiempo y por región.
- Determinar los géneros y plataformas más populares en diferentes mercados.
- Evaluar la correlación entre las reseñas de usuarios/expertos y el éxito en ventas.
- Analizar el impacto de la clasificación ESRB en las ventas de juegos.
- Predecir qué tipo de juegos tienen mayor probabilidad de éxito en el futuro cercano (en el contexto de la planificación para 2017).
- Responder las hipótesis:
	- Las calificaciones de los usuarios para los juegos en las plataformas con mayores ventas es igual o muy cercana.
	- Las calificaciones de los usuarios para los géneros de mas vendidos es diferente.

# Metodología
- El proceso incluyó la carga y limpieza de datos, el manejo de valores faltantes, la ingeniería de características (creación de variables con base en los datos brutos), el análisis univariado y la creación de visualizaciones para revelar patrones y anomalías.

# Herramientas y Tecnologías
-Python 3.12
- `Jupyter Notebook`
- `pandas` (pd): Manipulación y análisis de datos.
- `numpy` (np): Operaciones numéricas.
- `matplotlib` (plt): Creación de visualizaciones estáticas.
- `seaborn` (sns): Visualizaciones estadísticas atractivas.
- `scipy.stats` (st): Pruebas estadísticas y funciones.

# Hallazgos Clave / Insights

- **Pico de Lanzamientos**: Se identificó el periodo de 2008 a 2011 como el de mayor cantidad de lanzamientos de videojuegos.
- **Plataformas Líderes en Ventas**: Determinamos las tres plataformas con mayores ventas generales.
- **Ciclo de Vida de Consolas**: Observamos que las ventas de las plataformas fluctúan significativamente con la aparición de nuevas consolas, con un ciclo de vida promedio de aproximadamente 10 años.
- **Ventana de Sugerencia para Juegos Prometedores**: Establecimos un rango de 4 años como convención para identificar juegos con potencial.
- **Géneros Emergentes**: Se identificaron géneros con mayor potencial de crecimiento para el año 2017.
- **Ventas vs. Calificación de Usuario**: No se encontró correlación significativa entre las ventas de videojuegos y la calificación de los usuarios.
- **Dependencia de Ventas por Plataforma**: Las ventas de un videojuego están fuertemente ligadas a la plataforma en la que se lanza.
- **Diversidad Regional de Plataformas**: La plataforma más vendida varía considerablemente entre regiones.
- **Consistencia de Géneros Regionales**: El género de los juegos vendidos muestra poca variación entre regiones.
- **Independencia de Calificación por Plataforma**: La calificación de usuario de un juego no cambia en función de la plataforma.

# Recomendaciones de Negocio

- `Dominio del Género 'Action': El género de Acción es el más rentable, con $849.6 millones de dólares (MDD) en ventas, superando ampliamente a 'Strategy', que solo alcanzó $38.8 MDD. Priorizar el desarrollo y la comercialización de juegos de Acción es clave.
 Liderazgo de Ventas en Norteamérica: La región de Norteamérica (NA) presenta el mayor volumen de ventas de videojuegos por plataforma. Esto sugiere un mercado maduro y de alto potencial.
- **Preferencias por Plataforma Regionales**:
  - **En Norteamérica (NA)**, la Xbox 360 es la consola con mayores ventas.
  - **En Europa (EU)**, la Wii domina el mercado.
  - **En Japón (JP)**, el Nintendo DS lidera las ventas.
- **Adaptar las estrategias de lanzamiento y marketing a estas preferencias regionales es crucial.
  - **Géneros Dominantes por Región**:
    - **Los géneros Acción y Role-Playing son los más populares en **Norteamérica (NA)**.
    - **En Europa (EU)**, Acción y Racing son los géneros principales.
    - **En Japón (JP)**, Role-Playing y Platform destacan.
- Validación de Hipótesis de Calificación:
  - Se confirma que las calificaciones de usuario para Xbox One y PC son muy similares, lo que sugiere que la **plataforma no influye significativamente en la percepción de calidad en estos casos**.
  - Se valida que las calificaciones de usuario difieren notablemente entre los géneros de Acción y Deportes, indicando que **la satisfacción del usuario varía sustancialmente por tipo de juego**.
   
# Cómo Ejecutar el Proyecto
- Clonar el repositorio: git clone https://github.com/joraregut/eda-videojuegos-insights
- Instalar las dependencias:
  - Versión de Pandas: 2.2.2
  - Versión de NumPy: 1.26.4
  - Versión de Matplotlib: 3.9.0
  - Versión de Seaborn: 0.13.2
  - Versión de SciPy: 1.14.0
- Abrir el notebook: jupyter notebook **nombre_del_notebook.ipynb**

# Estructura del Repositorio
.
├── notebook/              # Cuadernos Jupyter con el análisis

│   └── eda_ice_games.ipynb

├── datasets/              # Archivos de datos originales y/o procesados

│   └── games.csv

├── README.md              # Este archivo

└── LICENSE                # Licencia

