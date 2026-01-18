# bda-modulo-3-evaluacion-final-MatiC-hub-1
bda-modulo-3-evaluacion-final-MatiC-hub-1 created by GitHub Classroom

# Evaluación - Módulo 3.- Transformación y análisis de datos

## 📌 Descripción del proyecto

Este repositorio contiene la resolución del **ejercicio de evaluación del Módulo 3 de "Transformación y análisis de datos"**. El objetivo del proyecto es realizar un análisis exploratorio, estadístico y visual de datos relacionados con el comportamiento de clientes dentro de un **programa de lealtad de una aerolínea**, utilizando Python y las librerías vistas durante el módulo.

El trabajo sigue una metodología clara y reproducible, similar a la que se utilizaría en un entorno profesional de análisis de datos.

---

## 📂 Estructura del repositorio

```text
├── data/
│   ├── Customer Flight Activity.csv
│   └── Customer Loyalty History.csv
│
├── notebooks/
│   └── resolucion_final.ipynb
│
├── outputs/
│   ├── vuelos_por_mes.png
│   └── distancia_volada_y_puntos.png
│
├── README.md
```

### Descripción de carpetas

* **data/**: contiene los datasets originales proporcionados para el ejercicio (sin modificar).
* **notebooks/**: notebook principal con todo el análisis, limpieza, visualizaciones e interpretaciones.
* **outputs/**: resultados generados durante el análisis (principalmente gráficos).
* **README.md**: documentación del proyecto.

---

## 🧠 Metodología de trabajo

El proyecto se desarrolla siguiendo las siguientes fases:

### 1️⃣ Exploración y limpieza de datos (EDA)

* Carga de los datasets.
* Exploración inicial (`head`, `info`, `describe`).
* Identificación y tratamiento de valores nulos y duplicidades lógicas.
* Análisis de posibles duplicados y agregación de la información cuando fue necesario para garantizar la consistencia del     análisis.
* Verificación de tipos de datos y consistencia.
* Unión de los datasets mediante la clave `Loyalty Number`.

### 2️⃣ Análisis estadístico

* Estadísticas descriptivas de variables numéricas relevantes.
* Identificación de valores atípicos.
* Análisis de correlaciones.
* Análisis de variables categóricas mediante distribuciones de frecuencia.

En todos los casos, los resultados se acompañan de una **interpretación en lenguaje natural**, orientada a un público no técnico.

### 3️⃣ Visualización de datos

Se utilizan gráficos adecuados para responder a las preguntas planteadas en el enunciado, entre ellas:

* Distribución de vuelos reservados por mes.
* Relación entre distancia volada y puntos acumulados.
* Distribución geográfica de clientes.
* Comparación de salarios según nivel educativo.
* Distribución de tipos de tarjeta de fidelidad.
* Análisis conjunto de estado civil y género.

Cada visualización incluye una breve interpretación.

Las visualizaciones generadas durante el análisis se guardan en la carpeta outputs/ para facilitar su revisión independiente del notebook.

### 4️⃣ Evaluación de diferencias por nivel educativo (en desarrollo)

* Preparación del subconjunto de datos relevante.
* Agrupación por nivel educativo.
* Cálculo de estadísticas descriptivas del número de vuelos reservados.
* Interpretación de los resultados.

---

## 🛠️ Herramientas utilizadas

* **Python**
* **Pandas**: manipulación y análisis de datos.
* **NumPy**: operaciones numéricas.
* **Matplotlib** y **Seaborn**: visualización de datos.
* **Os**: gestión de rutas y creación de directorios para la generación de outputs.

---

## 📌 Buenas prácticas

* Código comentado y estructurado.
* Uso de nombres de variables claros.
* Separación entre datos originales y resultados.
* Commits descriptivos durante el desarrollo del proyecto.

---

## ✍️ Notas finales

La variable Distance no especifica la unidad de medida en los datasets originales. Dado que todos los registros corresponden a clientes de Canadá y que los valores observados son coherentes con programas de fidelización de aerolíneas en contexto norteamericano, se interpreta la distancia como expresada en millas. Esta suposición se documenta únicamente a efectos analíticos.

Este proyecto no solo busca cumplir con los requisitos de la evaluación, sino reflejar una forma de trabajar ordenada, razonada y defendible, alineada con el rol de analista de datos en un entorno profesional.

