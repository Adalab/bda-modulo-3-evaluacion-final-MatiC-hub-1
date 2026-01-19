# bda-modulo-3-evaluacion-final-MatiC-hub-1
bda-modulo-3-evaluacion-final-MatiC-hub-1 created by GitHub Classroom

# Evaluación - Módulo 3.- Transformación y análisis de datos

## Descripción del proyecto

Este repositorio contiene la resolución del **ejercicio de evaluación del Módulo 3 de "Transformación y análisis de datos"**. El objetivo del proyecto es realizar un análisis exploratorio, estadístico y visual de datos relacionados con el comportamiento de clientes dentro de un **programa de lealtad de una aerolínea**, utilizando Python y las librerías vistas durante el módulo.

El trabajo sigue una metodología clara y reproducible, similar a la que se utilizaría en un entorno profesional de análisis de datos.

---

## Estructura del repositorio

├── data/
│   ├── Customer Flight Activity.csv
│   └── Customer Loyalty History.csv
│
├── notebooks/
│   └── resolucion_final.ipynb
│
├── outputs/
│   ├── vuelos_por_mes.png
│   ├── distancia_volada_y_puntos_acumulados.png
│   ├── clientes_por_provincia.png
│   ├── salario_promedio_por_educacion.png
│   ├── proporcion_tarjetas_fidelidad.png
│   ├── clientes_por_estado_civil_y_genero.png
│   ├── matriz_correlacion.png
│   └── boxplot_vuelos_por_nivel_educativo.png
│
└── README.md

### Descripción de carpetas

* **data/**: contiene los datasets originales proporcionados para el ejercicio (sin modificar).
* **notebooks/**: notebook principal con todo el análisis, limpieza, visualizaciones e interpretaciones.
* **outputs/**: resultados generados durante el análisis (principalmente gráficos).
* **README.md**: documentación del proyecto.

---

## Metodología de trabajo

El proyecto se desarrolla siguiendo las siguientes fases:

### 1- Exploración y limpieza de datos (EDA)

* Carga de los datasets.
* Exploración inicial (`head`, `info`, `describe`).
* Identificación y tratamiento de valores nulos y duplicidades lógicas.
* Análisis de posibles duplicados y agregación de la información cuando fue necesario para garantizar la consistencia del análisis.
* Verificación de tipos de datos y consistencia.
* Unión de los datasets mediante la clave `Loyalty Number`.

### 2- Análisis estadístico

* Estadísticas descriptivas de variables numéricas relevantes.
* Identificación de valores atípicos.
* Análisis de correlaciones.
* Análisis de variables categóricas mediante distribuciones de frecuencia.

En todos los casos, los resultados se acompañan de una **interpretación en lenguaje natural**, orientada a un público no técnico.

El análisis se realiza a nivel de comportamiento mensual, en coherencia con la estructura temporal del dataset.

### 3- Visualización de datos

Se utilizan gráficos adecuados para responder a las preguntas planteadas en el enunciado, entre ellas:

* Distribución de vuelos reservados por mes.
* Relación entre distancia volada y puntos acumulados.
* Distribución geográfica de clientes.
* Comparación de salarios según nivel educativo.
* Distribución de tipos de tarjeta de fidelidad.
* Análisis conjunto de estado civil y género.

Cada visualización incluye una breve interpretación en lenguaje natural, orientada a facilitar la comprensión de los resultados.

Las visualizaciones generadas durante el análisis se guardan en la carpeta outputs/ para facilitar su revisión independiente del notebook.

### 4- Evaluación de diferencias por nivel educativo

* Preparación del subconjunto de datos relevante.
* Agrupación por nivel educativo.
* Cálculo de estadísticas descriptivas del número de vuelos reservados.
* Interpretación de los resultados.

---

## Outputs generados

Durante la Fase 2 de análisis estadístico se ha generado y guardado el siguiente gráfico en la carpeta `outputs/`:

* `matriz_correlacion.png`: matriz de correlación entre las principales variables numéricas del dataset.

Durante la Fase 3 de visualización se han generado y guardado los siguientes gráficos en la carpeta `outputs/`:

* `vuelos_por_mes.png`: distribución mensual del número de vuelos reservados.
* `distancia_volada_y_puntos_acumulados.png`: relación entre la distancia volada y los puntos acumulados.
* `clientes_por_provincia.png`: distribución de clientes por provincia, destacando las tres provincias con mayor concentración.
* `salario_promedio_por_educacion.png`: comparación del salario promedio según nivel educativo.
* `proporcion_tarjetas_fidelidad.png`: proporción de clientes por tipo de tarjeta de fidelidad.
* `clientes_por_estado_civil_y_genero.png`: distribución conjunta de clientes por estado civil y género.

Durante la Fase 4 de evaluación de diferenccias se ha generado y guardado el siguiente gráfico en la carpeta `outputs/`:

* `boxplot_vuelos_por_nivel_educativo.png`: comparación de la distribución del número de vuelos reservados por mes entre los distintos niveles educativos.

---

## Herramientas utilizadas

* **Python**
* **Pandas**: manipulación y análisis de datos.
* **NumPy**: operaciones numéricas.
* **Matplotlib** y **Seaborn**: visualización de datos.
* **Os**: gestión de rutas y creación de directorios para la generación de outputs.

---

## Buenas prácticas

* Código comentado y estructurado.
* Uso de nombres de variables claros.
* Separación entre datos originales y resultados.
* Commits descriptivos durante el desarrollo del proyecto.

---

## Notas finales

La variable Distance no especifica la unidad de medida en los datasets originales. Dado que todos los registros corresponden a clientes de Canadá y que los valores observados son coherentes con programas de fidelización de aerolíneas en contexto norteamericano, se interpreta la distancia como expresada en millas. Esta suposición se documenta únicamente a efectos analíticos.

Este proyecto no solo busca cumplir con los requisitos de la evaluación, sino reflejar una forma de trabajar ordenada, razonada y defendible, alineada con el rol de analista de datos en un entorno profesional.

En este proyecto no se implementa un proceso ETL completo, ya que el objetivo es analítico y no productivo. Sin embargo, se realizan tareas propias de la fase de transformación de datos, como la limpieza, agregación y enriquecimiento de la información, orientadas al análisis exploratorio, estadístico y visual de los datos.

El enfoque seguido refleja una forma de trabajo habitual en el rol de analista de datos, priorizando la comprensión del comportamiento de los clientes y la correcta interpretación de los resultados frente a la automatización de procesos, en coherencia con los objetivos del ejercicio.

Este ejercicio presenta un análisis exploratorio, estadístico y visual de datos de un programa de fidelización, siguiendo una metodología estructurada y coherente con la naturaleza temporal del dataset. Los resultados permiten comprender el comportamiento mensual de los clientes y sugieren que variables como el nivel educativo no introducen diferncias significativas en el número de vuelos reservados.

El enfoque adoptado prioriza la claridad analítica, la interpretación razonada y las buenas prácticas propias del rol de analista de datos, reflejando una forma de trabajo ordenada, defendible y alineada con un entorno profesional.