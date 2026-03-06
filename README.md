# Desafio Telecom X Parte 2 - Análisis de Evasión de Clientes

Parte de la formacion de Alura Latam para Oracle.

# Objetivo:

- El objetivo de este desafio es continuar el trabajo de la parte 1 y desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios.

# Estructura del proyecto:

-> TelecomX_2_Latam_Josue_Marquez.ipynb : notebook colab
-> README.md : este archivo
-> datos_tratados.csv : archivo con los datos tratados de la parte 1

# Tareas:

- Preparar los datos para el modelado (tratamiento, codificación, normalización).

- Realizar análisis de correlación y selección de variables.

- Entrenar dos o más modelos de clasificación.

- Evaluar el rendimiento de los modelos con métricas.

- Interpretar los resultados, incluyendo la importancia de las variables.

- Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.

# Tecnologias:

- Python
- Pandas
- Seaborn
- Pyplot
- Sklearn
- Imblearn
- Google Colab
- Git

# Como ejecutar:

- Google Colab
    1. Descargar archivo notebook `TelecomX_2_Latam_Josue_Marquez.ipynb`
    2. Importar a Google Colab
    3. Hacer click en 'Ejecutar todo'

# Descripción del proceso de preparación de los datos:

1. Se selecciono las variables categoricas para luego procesarlas con OneHotEncoder y se dejo las variables numericas preparadas en la parte 1 como estaban.

2. Para el modelo Linear de Regresion Logistica se utilizo MinMaxScaler para normalizar las columnas numericas

3. Para probar cada modelo se ocupo StratifiedKFold con 'n_splits=5' que separo la data entre entrenamiento y prueba 5 veces cada vez.

4. Se eligio normalizar los datos ya que habia una gran diferencia numerica por ejemplo entre Cargo_Total y Antiguedad_Meses.

# Graficos:

Matriz de Correlacion
![alt text](/images/image.png)

Matriz de Confusion para el Modelo con Oversample:
![alt text](/images/image-1.png)

Matriz de Confusion para el Moldelo de Regresion Logistica
![alt text](/images/image-2.png)
