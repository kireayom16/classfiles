# classfiles
aqui se encuentran las practicas de progrgramacion analitica en colab

 Practica 1
 
 Este  proyecto el archivo mbox.txt para extraer únicamente los valores numéricos asociados a la etiqueta X-DSPAM-Confidence.

Cómo funciona

procesa el archivo mbox.txt para buscar todas las líneas que contienen la etiqueta X-DSPAM-Confidence:.
Cuando encuentra una, extrae el valor numérico que aparece después de los dos puntos, lo convierte a decimal (float) y lo guarda en una lista llamada mediciones.
Finalmente, imprime en pantalla todas las líneas encontradas.


Practica 2

Este proyecto lee un archivo de texto (informe_acciones.txt) que contiene informes de distintas empresas con información sobre el valor actual de sus acciones.
El código utiliza expresiones regulares (regex) para localizar automáticamente todas las frases que comienzan con "Te escribo para informarte sobre el valor actual de la acción de..." y extrae:
El nombre de la empresa.
El valor actual de la acción.
Una vez encontrados los datos, los muestra en consola en un formato claro y ordenado.

Cómo funciona

El script abre el archivo con codificación latin-1 para evitar errores con caracteres especiales.
Se define un patrón que identifica la frase clave, el nombre de la empresa y el valor.
re.findall() obtiene todas las coincidencias como una lista de tuplas (empresa, valor).
Se recorre la lista e imprime cada resultado en consola

Practica 3

Esta práctica tiene como objetivo principal desarrollar competencias fundamentales en el manejo de estructuras de datos y operaciones básicas con arreglos en Python.

Como funciona

Creación del arreglo: Usando np.random.randint(1, 101, 20) para generar 20 números aleatorios entre 1 y 100 .

Valor máximo: np.max() encuentra el valor más grande en el arreglo al recorrer todos los elementos y compararlos entre sí.

Valor mínimo: np.min() encuentra el valor más pequeño en el arreglo mediante la comparación de todos los elementos.

Media: np.mean() calcula el promedio sumando todos los elementos del arreglo y dividiendo esta suma entre la cantidad total de elementos.

Sumar 10 a cada elemento: Usando operaciones  de NumPy donde arreglo + 10 realiza la suma de 10 a cada elemento individual del arreglo de manera simultánea y eficiente, sin necesidad de usar bucles.


Practica 4

La finalidad de esta práctica es desarrollar competencias esenciales en el manejo y operación de matrices bidimensionales utilizando Python, específicamente con la biblioteca NumPy. 


como funciona 

Creación de matrices: np.random.randint(1, 11, (3, 3)) genera matrices 3x3 con valores entre 1 y 10.

Suma de matrices: Se realiza elemento por elemento de la matriz1 y matriz2.

Resta de matrices: Similar a la suma, pero restando elemento por elemento.

Multiplicación por escalar: Cada elemento de la matriz1 se multiplica por el escalar 2 .

Multiplicación matricial: utilizando np.dot() asegura que se siga la regla filas de la primera matriz × columnas de la segunda matriz.


Practica 5 

La finalidad es entender y aplicar máscaras booleanas en NumPy para:
Filtrar datos fácilmente según condiciones.
Trabajar de manera eficiente y sin bucles manuales.

Como funciona 

Primero se crea una lista de números al azar, en este caso 15 números entre 1 y 50.

Creación de la máscara booleana:

Después, se revisa cada número y se compara con el valor 25.

Si el número es mayor que 25, se marca con True.

Si es menor o igual a 25, se marca con False.

Esto genera una “máscara” de valores verdaderos y falsos del mismo tamaño que el arreglo original.


Con esa máscara, se extraen únicamente los números que tienen marcada la posición en True.


Finalmente, se suman las  veces que  apareció True en la máscara. Ese número corresponde a la cantidad de elementos mayores que 25.


Practica 6

El objetivo es aprender a manipular, analizar y extraer información útil de un conjunto de datos usando Pandas y NumPy.

Ejercicio 1: Distribución de supervivencia por sexo y clase

Se agrupan los pasajeros según su sexo y su clase de boleto.

Luego se calcula qué porcentaje sobrevivió en cada combinación.

Finalmente, se identifica qué grupo tuvo la mayor probabilidad de sobrevivir y cuál la menor.

Ejercicio 2: Identificación de familias grandes a bordo

Se calcula el tamaño de la familia de cada pasajero sumando los familiares a bordo.

Se consideran “familias grandes” aquellas con más de 3 integrantes.

Después, se cuentan cuántos pasajeros pertenecían a familias grandes y qué proporción de ellos sobrevivió.

Ejercicio 3: Segmentación por grupos de edad

Se clasifican los pasajeros en dos categorías:

Menor de edad 

Mayor de edad 

Ejercicio 4: Comparación entre promedios con NumPy y Pandas

Se calcula el promedio de las edades y de las tarifas pagadas de dos maneras:

Usando NumPy.

Usando las funciones propias de Pandas.

Ejercicio 5: Creación de intervalos de tarifas y análisis

Se divide el rango de tarifas en 5 intervalos equidistantes.

Cada pasajero se asigna al intervalo que corresponde según lo que pagó.

Luego se calcula:

Cuántos pasajeros hubo en cada intervalo.

Qué proporción de ellos sobrevivió.


Practica 7

El objetivo de esta práctica es aprender a explorar, analizar y visualizar datos utilizando el dataset clásico Iris con las librerías Seaborn y Matplotlib en Python.

Como funciona: 

a) Gráfico de barras

groupby("species"):
Agrupa los datos por la columna species.

mean():
 Se usa para comparar medidas promedio (petal_length y petal_width).

plot(kind="bar"):
Genera un gráfico de barras.


b) Histograma

sns.histplot():
Crea un histograma de frecuencias.

Parámetro bins: define el número de intervalos del histograma.

c) Gráfico de dispersión

sns.scatterplot():
Crea un diagrama de dispersión.

Parámetro hue="species":
Colorea los puntos según la especie.

d) Gráfico de cajas (box plot)

df.melt():
Se usa porque un boxplot necesita los datos en forma de pares (variable, valor) para comparar varias columnas.

sns.boxplot():
Genera un diagrama de cajas.


e) Gráfico de líneas

sns.lineplot():
Crea un gráfico de líneas.

Parámetro x=df.index:
Se coloca el índice como eje X.


Practica 8 

El objetivo es  utilizar Seaborn para crear visualizaciones más avanzadas y atractivas. A través del dataset “tips”

Como funciona:

a)Mapa de Calor

Función: sns.heatmap()

 Dibuja un mapa de colores en forma de tabla, donde cada celda representa un valor (en este caso, la correlación entre variables numéricas).

 b)Diagrama de Violín
 
 Función: sns.violinplot()
 
 Combina un boxplot con una distribución de densidad. Muestra la mediana, los cuartiles y la forma en que se distribuyen los valores.

 c)Gráfico de Dispersión

Función: sns.scatterplot()

Representa puntos en un plano cartesiano, usando un eje para cada variable numérica. Además, permite usar un tercer atributo (como hue) para diferenciar categorías por color.

d) Gráfico de Barras

Función: sns.barplot()

 Calcula automáticamente una medida estadística (por defecto, la media) y la muestra como una barra para cada categoría.

Practica 9 

El objetivo es aprender a crear gráficos de dispersión interactivos para visualizar y analizar relaciones entre variables socioeconómicas, específicamente entre el PIB per cápita y la esperanza de vida de diferentes países, utilizando el dataset Gapminder.

Como funciona:

Se importa Plotly Express y se carga el dataset Gapminder que contiene indicadores de desarrollo por país y año.

Se filtran los datos para conservar solo los del año 2007, permitiendo un análisis transversal.

x="gdpPercap": Establece el PIB per cápita en el eje X

y="lifeExp": Establece la esperanza de vida en el eje Y

size="pop": Representa el tamaño de la población con el tamaño de los puntos

color="continent": Diferenciación por color según el continente

size_max=60: Controla el tamaño máximo de los puntos

Practica 10

Esta práctica tiene como objetivo aprender a crear visualizaciones interactivas de datos utilizando gráficos de dispersión con Plotly Express y el dataset Gapminder.

Como funciona:

 px.scatter() - Función principal para crear gráficos de dispersión

 px.data.gapminder() - Carga el dataset Gapminder


Practica 11

El objetivo principal es aprender a crear y personalizar gráficos de líneas para visualizar la evolución temporal de datos financieros (acciones), utilizando la librería Plotly Express en Python.

Como Funciona:

Se importa Plotly Express.

Se carga el dataset de stocks incluido en Plotly Express.

px.line(): Función que crea un gráfico de líneas.

df: DataFrame con los datos.

x="date": Establece la columna "date" como eje X (variable temporal).

y=df.columns[1:]: Usa las columnas del DataFrame excluyendo la primera columna ('date')

title: Agrega un título al gráfico


Practica 12

El objetivo es aprender a crear mapas de calor interactivos utilizando plotly.graph_objects para visualizar datos matriciales, específicamente el número de pasajeros de vuelos a lo largo de los meses y años.

Como funciona:

seaborn: Para cargar el dataset de vuelos

pandas: Para manipulación y transformación de datos

plotly.graph_objects: Para crear visualizaciones interactivas

Se carga el dataset "flights" de Seaborn

Se transforma con pivot() para crear una matriz año-mes con los pasajeros como valores

go.Heatmap() crea el mapa de calor con los datos transformados

La escala "magma" ofrece buen contraste para visualizar patrones

Se agrega un título descriptivo al gráfico


Practicas 13-17
El objetivo es preprocesar un conjunto de datos en formato CSV usando Pandas, asegurando que:

Los datos irrelevantes sean eliminados.

Las columnas tengan nombres correctos y consistentes.

Los nombres de las columnas estén normalizados (estándar).

Los tipos de datos sean los adecuados para su análisis (ejemplo: convertir precios a números).

Se documente el dataframe resultante con un diccionario de datos.


Práctica 13: Carga de Datos

Funcionamiento:

Se usa pd.read_csv() para leer el archivo.

Con .iloc[:-1, :] se eliminó la última fila, ya que contiene texto que no pertenece a los datos.

Con df.tail(3) se revisa que la última fila no fue cargada.

Con df.shape se imprime el número de filas y columnas del dataframe.


Práctica 14: Agregar una Columna

Funcionamiento:

Se imprime df.columns para revisar los nombres actuales de las columnas.

Se verifica si la primera columna se llama INDEX MIIAD.

Si no es así, se renombra con df.rename(columns={df.columns[0]: "INDEX MIIAD"}, inplace=True).

Se vuelven a imprimir los nombres para verificar el cambio.


Práctica 15: Normalización de los nombres de las columnas

Funcionamiento:

Se convierten todos los nombres a minúsculas con .str.lower().

Se eliminan espacios sobrantes con .str.strip().

Se reemplazan los espacios por guiones bajos con .str.replace(" ", "_").

Finalmente, se imprimen los nuevos nombres para verificar.


Práctica 16: Errores en los Tipos de Datos

Funcionamiento:

Se imprime df.dtypes para revisar los tipos actuales.

Las columnas sale_price, land_square_feet, y gross_square_feet deben ser numéricas (float).

Se convierten con pd.to_numeric(df[col], errors="coerce").

errors="coerce" convierte los valores inválidos a NaN.

Se vuelven a imprimir los tipos de datos para confirmar los cambios.


Práctica 17: Diccionario de Datos

Funcionamiento:

Se construye un diccionario de Python (diccionario_datos) que contiene:

tipo de dato de la columna.

cantidad de valores nulos (NaN).

ejemplo de valor no nulo.

Se imprime el contenido del diccionario para documentar el dataset.

