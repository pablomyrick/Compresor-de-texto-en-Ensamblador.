# Compresor-de-texto-en-Ensamblador.
📌 Proyecto de Programación en Ensamblador – Compresión de Texto

Este repositorio contiene el desarrollo del proyecto de programación en ensamblador para la asignatura Estructura de Computadores. El objetivo principal es implementar un algoritmo de compresión y descompresión de texto sin pérdida de información, utilizando ensamblador para el procesador Motorola 88110.

🔹 Características del proyecto:

✔️ Implementación de subrutinas para la compresión y descompresión de texto.

✔️ Uso de estructuras de memoria para almacenar los datos comprimidos.

✔️ Aplicación de técnicas de optimización en ensamblador.

✔️ Ejecución en un emulador del procesador 88110, sin interacción con periféricos.


📂 Estructura del Repositorio:

CDV25.ens/ → Código fuente en ensamblador.

memoria.pdf/ → Documentación del proyecto y enunciado original.

ResultadosCorreciones/ → Resultados de los casos de prueba para verificar el correcto funcionamiento de las subrutinas.


🚀 Cómo compilar y ejecutar el programa en el emulador MC88110

1️⃣ Compilar el código ensamblador

Ejecuta el ensamblador con el siguiente comando:

      88110e -e 0 -ml -o programa.bin programa.ens


Explicación de los parámetros:

-e 0 → Define la dirección de entrada del programa en 0.

-ml → Usa ordenamiento de bytes en Little Endian.

-o programa.bin → Nombre del archivo de salida con el código máquina.

programa.ens → Nombre del archivo ensamblador.


2️⃣ Cargar y ejecutar el programa en el emulador

      mc88110 programa.bin

Interacción con el emulador:

e → Ejecutar el programa completo.

t → Ejecutar paso a paso (modo traza).

p + <dirección> → Establecer un punto de interrupción en una dirección específica.

d <dirección> → Desensamblar instrucciones en memoria.

v <dirección> → Ver contenido de memoria.


3️⃣ Depuración y seguimiento
Para ejecutar en modo traza y analizar el estado de los registros después de cada instrucción:

      t
      
      r
Para visualizar los datos en memoria después de la ejecución:

      v 1000
