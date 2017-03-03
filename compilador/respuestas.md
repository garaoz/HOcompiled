PREGUNTAS Y RESPUESTAS:

1. Escriban qué esperan de cada uno de los pasos

Pre-procesador: Interpreta el codigo segun el lenguaje de programacion utilizado e incorpora los codigos (o headers de librerias) incluidos en el codigo principal.
Compilacion I: Conversion a codigo assembler y optimizacion de software. Desde esta etapa el codigo es independiente del lenguaje de programacion en el que fue creado.
Compilacion II: Conversion (o "traduccion") a codigo de maquina (binario)
Linkeo: Generacion del archivo ejecutable (para que el archivo binario sea compatible con el sistema operativo).

2. ¿Qué agregó el preprocesador?

El preprocesador agrego el codigo y los sub-codigos incluidos en "calculator.h".
En particular incluye la funcion "printf" que no estaba definida en "calculator.c"

3. Identificar en la rutina de assembler las funciones

Las funciones son: printf y add_numbers

4. Explicar qué quieren decir los símbolos que se crean en el objeto

Los simbolos que aparecen en el archivo "calculator.o" son T y U. La letra "T" (antes de add_numbers y de main) indica que se trata de un texto (Text), mientras que la letra "U" (antes de printf) indica que aun no se encuentra definida (Undefined). Esto es porque printf se define en calculator.h.

5. ¿En qué se diferencian los símbolos del objeto y del ejecutable?

En el archivo ejecutable aparecen simbolos que tienen que ver con el funcionamiento del linker.
Los simbolos en el archivo ejecutable aparecen en minusculas y mayusculas. En minusculas significa que son estaticos y no se pueden ver desde afuera. Por el contrario, las mayusculas significan que pueden verse desde afuera.
A su vez, en el archivo ejecutable aparecen los siguientes simbolos: "R" o "r": Read only (solo lectura) y "D" o "d": Data (datos).

