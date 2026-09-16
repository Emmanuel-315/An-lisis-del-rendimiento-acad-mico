# Anlisis-del-rendimiento-acadmico
Este proyecto realiza un análisis exploratorio de datos de los estudiantes para comprender el rendimiento utilizando Python.

# Objetivo:
Explorar el dataset para identificar qué factores están relacionados con un mejor o peor desempeño académico, calcular un promedio general por estudiante, clasificar el rendimiento en niveles (Bajo, Medio, Alto) y responder preguntas concretas sobre diferencias de desempeño según curso de preparación, nivel educativo de los padres y grupo étnico.

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

# Análisis realizados
Exploración inicial: dimensiones, tipos de datos, valores faltantes, duplicados y estadísticas descriptivas.
Limpieza y normalización de nombres de columnas.
Creación de la variable average_score (promedio de Matemáticas, Lectura y Escritura).
Clasificación del rendimiento en Bajo / Medio / Alto según rangos fijos sobre average_score (< 60, 60-79, ≥ 80).
Cinco preguntas de análisis: área con mejor promedio, efecto del curso de preparación, relación con el nivel educativo de los padres, porcentaje de estudiantes por nivel de rendimiento, y comparación de promedios por grupo étnico.
Cuatro visualizaciones: histograma de average_score, promedio por curso de preparación, promedio por nivel educativo de los padres, y proporción de estudiantes por nivel de rendimiento.
Resultados y conclusiones
Lectura es el área con el promedio más alto de las tres; Matemáticas es consistentemente la más baja.
Los estudiantes que completaron el curso de preparación obtienen en promedio mejores resultados que quienes no lo tomaron.
A mayor nivel educativo de los padres, mayor tiende a ser el promedio del estudiante.
La mayoría de los estudiantes (poco más de la mitad) se ubica en el nivel de rendimiento Medio; solo una minoría alcanza el nivel Alto (promedio ≥ 80).
Existen diferencias de desempeño entre los distintos grupos étnicos, lo que podría reflejar diferencias socioeconómicas o de acceso a recursos educativos que valdría la pena investigar más a fondo (por ejemplo, cruzando con el tipo de almuerzo como proxy de nivel socioeconómico).


Contenido:

data/ StudentsPerformance.csv     # Dataset original

analisis.ipynb              # Notebook con todo el análisis

images/                         # Gráficas generadas por el notebook

requirements.txt                # Dependencias del proyecto

.gitignore

LÉAME.md

# Instalación

Clonar el repositorio:

git clone URL_DEL_REPOSITORIO

Entrar al proyecto:
cd nombre-del-repositorio

Crear el entorno virtual:
python -m venv .venv

Activarlo e instalar dependencias:
 Windows
.venv\Scripts\activate

 macOS / Linux
source .venv/bin/activate

pip install -r requirements.txt
Ejecución

Abrir y ejecutar el notebook desde VS Code o Jupyter:
Abrir notebooks/analisis.ipynb, seleccionar el kernel del entorno .venv y ejecutar todas las celdas (Run All).
O ejecutarlo desde la terminal sin abrir la interfaz de Jupyter:
jupyter nbconvert --to notebook --execute --inplace notebooks/analisis.ipynb

Las gráficas generadas se guardan automáticamente en la carpeta images/.

En conjunto, los resultados sugieren que factores externos al desempeño individual —como la preparación previa y el contexto familiar— están relacionados con los resultados académicos, y podrían orientar programas de apoyo focalizados por parte de la institución.
