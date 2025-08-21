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
