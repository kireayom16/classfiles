# classfiles
aqui se encuentran las practicas de progrgramacion analitica en colab

 Practica 1



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
