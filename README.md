# sprint7-final-project
# Proyecto ConnectaTel - Análisis de Clientes y Patrones de Uso

## Objetivo del proyecto

El objetivo de este proyecto es analizar la información de clientes y registros de uso de la empresa ConnectaTel para identificar patrones de comportamiento, segmentos de clientes, problemas de calidad de datos y oportunidades de negocio que permitan optimizar la oferta de planes y mejorar la toma de decisiones.

## Datasets utilizados

### users

Contiene información demográfica y contractual de los clientes:

* user_id
* age
* city
* plan
* reg_date
* churn_date

### usage

Contiene los registros de actividad de los usuarios:

* user_id
* type
* date
* duration
* length

Donde:

* `type = call` representa llamadas telefónicas.
* `type = text` representa mensajes de texto.

## Etapas del análisis realizadas

### 1. Exploración inicial de datos

* Revisión de estructura, tipos de datos y estadísticas descriptivas.
* Identificación de valores faltantes e inconsistencias.

### 2. Limpieza y preparación de datos

* Corrección de edades inválidas (-999).
* Tratamiento de ciudades desconocidas representadas por "?".
* Corrección de fechas fuera de rango.
* Análisis de valores faltantes.
* Verificación del comportamiento de los nulos en función de la variable `type`.

### 3. Ingeniería y agregación de variables

* Cálculo de cantidad de mensajes por usuario.
* Cálculo de cantidad de llamadas por usuario.
* Cálculo de minutos totales de llamadas.
* Integración de métricas de uso con la tabla de usuarios.

### 4. Análisis exploratorio

* Distribución de edades.
* Distribución de planes contratados.
* Distribución de ciudades.
* Análisis de patrones de uso.
* Identificación de segmentos de clientes.

### 5. Detección de valores atípicos

* Análisis de outliers en llamadas, mensajes y minutos consumidos.
* Evaluación de posibles implicaciones para el negocio.

### 6. Generación de insights de negocio

* Identificación de segmentos más valiosos.
* Evaluación de oportunidades comerciales.
* Recomendaciones para optimizar la oferta de planes.

## Cómo ejecutar el notebook

### Opción 1: Google Colab

1. Abrir Google Colab.
2. Seleccionar **Archivo → Subir notebook**.
3. Cargar el archivo `.ipynb` del proyecto.
4. Ejecutar las celdas en orden desde el inicio.

### Opción 2: Jupyter Notebook

1. Instalar Python 3.
2. Instalar las librerías necesarias:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Abrir Jupyter Notebook.
4. Abrir el archivo del proyecto.
5. Ejecutar todas las celdas secuencialmente.

## Guía de reproducción

1. Cargar los datasets `users` y `usage`.
2. Ejecutar la sección de limpieza y validación de datos.
3. Ejecutar la agregación de métricas por usuario.
4. Realizar la unión de los datasets.
5. Generar visualizaciones y estadísticas descriptivas.
6. Analizar los segmentos de clientes y patrones de uso.
7. Revisar las conclusiones e insights ejecutivos para el negocio.
