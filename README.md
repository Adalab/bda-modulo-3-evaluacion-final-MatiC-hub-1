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
│   ├── resolucion_final.ipynb
│   └── bonus_estadistica_inferencial.ipynb
│
├── outputs/
│   ├── vuelos_por_mes.png
│   ├── distancia_volada_y_puntos_acumulados.png
│   ├── clientes_por_provincia.png
│   ├── salario_promedio_por_educacion.png
│   ├── proporcion_tarjetas_fidelidad.png
│   ├── clientes_por_estado_civil_genero.png
│   ├── matriz_correlacion.png
│   └── boxplot_vuelos_por_nivel_educativo.png
│
├── README.md

### Descripción de carpetas

**data/**  
Contiene los datasets originales proporcionados para el ejercicio, sin modificaciones.

**notebooks/**  
Incluye el notebook principal con todo el análisis exploratorio, estadístico y visual, así como un notebook adicional de bonus con un análisis de estadística inferencial.

**outputs/**  
Contiene las visualizaciones generadas durante el análisis, guardadas para facilitar su revisión independiente del notebook.

**README.md**  
Documento descriptivo del proyecto, metodología empleada y estructura del repositorio.

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

### 5.- BONUS: Estadística Inferencial

* De forma adicional, se incluye un notebook de bonus con un análisis de estadística inferencial (prueba de Kruskal–Wallis), utilizado como validación estadística de los resultados descriptivos y visuales del análisis principal.

* REPRODUCIBILIDAD Y ORGANIZACIÓN DEL ANÁLISIS: Cada notebook del proyecto es reproducible de forma independiente. Por este motivo, en el notebook de bonus de estadística inferencial se reconstruye el dataset final a partir de las fuentes originales y de las transformaciones clave realizadas, evitando dependencias implícitas entre notebooks.

* Este enfoque garantiza la trazabilidad del análisis, facilita su ejecución de principio a fin y refleja buenas prácticas habituales en proyectos de análisis de datos.


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

## 🧾 Notas finales

La variable **Distance** no especifica explícitamente su unidad de medida en los datasets originales. Dado que todos los registros corresponden a clientes de Canadá y que los valores observados son coherentes con programas de fidelización de aerolíneas en contexto norteamericano, se interpreta la distancia como expresada en **millas**. Esta suposición se documenta únicamente a efectos analíticos.

Este proyecto no solo busca cumplir con los requisitos de la evaluación, sino reflejar una forma de trabajar **ordenada, razonada y defendible**, alineada con el rol de analista de datos en un entorno profesional.

No se implementa un proceso **ETL completo**, ya que el objetivo del ejercicio es analítico y no productivo. No obstante, se realizan tareas propias de la fase de transformación de datos —limpieza, agregación y enriquecimiento— orientadas al análisis exploratorio, estadístico y visual.

El análisis se apoya en la estructura temporal del dataset, trabajando a nivel de **comportamiento mensual de los clientes**. Los resultados permiten comprender el patrón de reservas y sugieren que variables como el **nivel educativo no introducen diferencias significativas** en el número de vuelos reservados por mes.

En conjunto, el proyecto prioriza la claridad analítica, la correcta interpretación de los resultados y las buenas prácticas propias del análisis de datos, presentando un trabajo **reproducible, coherente y defendible**.

