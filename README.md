# Anlisis-del-rendimiento-acadmico
Este proyecto realiza un análisis exploratorio de datos de los estudiantes para comprender el rendimiento utilizando Python.

El objetivo es identificar características relacionadas con el rendimiento de los estudiantes mediante técnicas de limpieza, transformación, análisis estadístico y visualización de datos.

Conjunto de datos
Nombre: Rendimiento de los estudiantes en los exámenes

Fuente: Kaggle

Archivo utilizado: StudentsPerformance.csv

El cojunto de datos contenido, los datos consta de las calificaciones obtenidas por los estudiantes en diversas asignaturas.

El Dataset Students Performance in Exams, con las siguientes columnas:

Columna	Descripción
gender	Género del estudiante
race/ethnicity	Grupo (A-E)
parental level of education	Nivel educativo de los padres
lunch	Tipo de almuerzo (standard / free-reduced)
test preparation course	Si completó o no un curso de preparación
math score	Puntaje en Matemáticas (0-100)
reading score	Puntaje en Lectura (0-100)
writing score	Puntaje en Escritura (0-100)

¿Qué hace el análisis?
Carga y exploración inicial del dataset (dimensiones, tipos de datos, nulos, duplicados, estadísticas descriptivas).
Limpieza y normalización de nombres de columnas.
Creación de la variable average_score (promedio de las tres materias).
Clasificación del rendimiento en Bajo / Medio / Alto según rangos fijos sobre average_score (< 60, 60-79, ≥ 80).
Cinco preguntas de análisis respondidas con tablas agregadas (promedio por área, efecto del curso de preparación, nivel educativo de los padres, distribución por nivel de rendimiento, comparación por grupo).
Cuatro visualizaciones (histograma, barras y pastel).
Conclusiones finales.

Contenido
├── data/

│   └── StudentsPerformance.csv     # Dataset original

├── analisis.ipynb              # Notebook con todo el análisis

├── images/                         # Gráficas generadas por el notebook

├── requirements.txt                # Dependencias del proyecto

├── .gitignore

└── LÉAME.md
