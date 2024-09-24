# EJERCICIOS BÁSICOS PTHON 🐍  
## VARIABLES, EXPRESIONES Y DECLARACIONES
### EJERCICIO 1: Escribe un programa que use input para pedirle a un usuario su nombre y luego le de la bienvenida.
### EJERCICIO 2: Escribe un programa para pedirle al usuario las horas y la tarifa por hora para calcular el pago bruto.
### EJERCICIO 3: Supongamos que ejecutamos las siguientes instrucciones de asignación:
width = 17  
height = 12.0  
### Para cada una de las siguientes expresiones, escriba el valor de la expresión y el tipo (del valor de la expresión). Use el intérprete de Python para verificar sus respuestas.
1. width//2
2. width/ 2.0
3. height/ 3
4. 1+2\*5
### EJERCICIO 4: Escribe un programa que solicite al usuario una temperatura en grados Celsius, convierta la temperatura a Fahrenheit e imprima la temperatura convertida

## CONDICIONALES
### EJERCICIO 5: Reescribe tu cálculo de pago (EJERCICIO 2) para darle al empleado 1.5 veces la tarifa por hora por las horas trabajadas por encima de las 40 horas. La salida es la siguiente:  
Enter Hours: 45  
Enter Rate: 10  
Pay: 475.0  
### EJERCICIO 6: Reescribe tu programa de pago usando (EJERCICIO 2) "try" y "except" para que su programa maneje la entrada no numérica correctamente imprimiendo un mensaje y saliendo del programa. A continuación se muestran una ejecución del programa:
Enter Hours: 20  
Enter Rate: nine  
Error, please enter numeric input  
### EJERCICIO 7: Escribe un programa para solicitar una puntuación entre 0.0 y 1.0. Si la puntuación está fuera de rango, imprime un mensaje de error. Si la puntuación está entre 0.0 y 1.0, imprime una calificación usando la siguiente tabla:
| Score   | Grade |
|---------|-------|
| >= 0.9  | A     |
| >= 0.8  | B     |
| >= 0.7  | C     |
| >= 0.6  | D     |
| < 0.6   | F     | 
### Ejecute el programa repetidamente para probar los diferentes valores de entrada.

## FUNCIONES
### EJERCICIO 8: Reescribe su cálculo de pago (EJERCICIO 2) con tiempo y medio para horas extras y crea una función llamada "computepay" que tome dos parámetros ("hours" y "rate").
### EJERCICIO 9: Reescribe el programa de calificación del capítulo anterior (EJERCICIO 7) utilizando una función llamada "computegrade" que tome una puntuación como parámetro y devuelva una nota como una cadena.
### EJERCICIO 10: Escribe un programa que lea números repetidamente hasta que el usuario ingrese "listo". Una vez que se ingrese "listo", imprima el total, el recuento y el promedio de los números. Si el usuario ingresa algo que no sea un número, detecta su error usando "try" y "except" e imprime un mensaje de error y salta al siguiente número. Ejemplo de ejecución: 
Enter a number: 4  
Enter a number: 5  
Enter a number: bad data  
Invalid input  
Enter a number: 7  
Enter a number: done  
16 3 5.333333333333333  
### EJERCICIO 11:  Escribe otro programa que solicite una lista de números como arriba y al final imprima el máximo y el mínimo de los números en lugar del promedio.

## CADENAS
### EJERCICIO 12: Toma el siguiente código de Python que almacena una cadena:  
"str = 'X-DSPAM-Confidence: 0.8475"  
### Usa "find" y el corte de cadena para extraer la parte de la cadena después del caracter de dos puntos y luego use la función "float" para convertir la cadena extraída en un número de punto flotante.  

## ARCHIVOS
### EJERCICIO 13: Escribe un programa para leer un archivo e imprime el contenido del mismo (línea por línea) todo en mayúsculas. Ejecutando el programa se verá como sigue:  
python shout.py  
Enter a file name: mbox-short.txt  
FROM STEPHEN.MARQUARD@UCT.AC.ZA SAT JAN  5 09:14:16 2008  
RETURN-PATH: <POSTMASTER@COLLAB.SAKAIPROJECT.ORG>  
RECEIVED: FROM MURDER (MAIL.UMICH.EDU [141.211.14.90])  
     BY FRANKENSTEIN.MAIL.UMICH.EDU (CYRUS V2.3.8) WITH LMTPA;  
     SAT, 05 JAN 2008 09:14:16 -0500  
### Puedes descargar el archivo desde  
www.py4e.com/code3/mbox-short.txt  

### EJERCICIO 14: Escribe un programa para solicitar un nombre de archivo. Luego lee el archivo y busca las líneas del formulario:  
X-DSPAM-Confidence: 0.8475  
### Cuando encuentra una línea que comienza con "X-DSPAM-Confidence:", separa la línea para extraer el número de punto flotante en la línea. Cuenta estas líneas y luego calcula el total de los valores de confianza de correo no deseado de estas líneas. Cuando llegues al final del archivo, imprime la confianza promedio del spam.  
Enter the file name: mbox.txt  
Average spam confidence: 0.894128046745

Enter the file name: mbox-short.txt  
Average spam confidence: 0.750718518519  

## LISTAS
### EJERCICIO 15: Escriba una función llamada "chop" que tome una lista y la modifique, eliminando el primer y último elemento y devuelva "None".  
### Luego escribe una función llamada "middle" que tome una lista y devuelva una nueva lista que contiene todos los elementos, excepto el primero y el último.

### EJERCICIO 16: Descarga una copia del archivo desde  
http://www.py4e.com/code3/romeo.txt  
### Escribe un programa para abrir el archivo romeo.txt y léelo línea por línea. Para cada línea, divide la línea en una lista de palabras usando la función split. Para cada palabra, verifica si la palabra ya está en una lista. Si la palabra no está en la lista, agrégala a la lista. Cuando se complete el programa, ordena e imprime las palabras resultantes en orden alfabético.  

### EJERCICIO 17: Escribe un programa para leer los datos del buzón de correo y cuando encuentre la línea que comienza con "From", dividirá la línea en palabras usando la función `split`. Estamos interesados ​​en quién envió el mensaje, que es la segunda palabra en la línea From.  
### Analizará la línea Desde e imprimirá la segunda palabra para cada línea From, también contará el número de líneas From (no From:) e imprimirá un recuento al final. Esta es una buena salida de muestra con algunas líneas eliminadas:  

```python  
python fromcount.py  
Enter a file name: mbox-short.txt  
stephen.marquard@uct.ac.za  
louis@media.berkeley.edu  
zqian@umich.edu  

[...some output removed...]  

ray@media.berkeley.edu  
cwen@iupui.edu  
cwen@iupui.edu  
cwen@iupui.edu  
There were 27 lines in the file with From as the first word  
```  
  
### EJERCICIO 18: Escribe un programa que solicita al usuario una lista de números e imprime el máximo y el mínimo de los números al final cuando el usuario ingresa "listo". Escribe el programa para almacenar los números que el usuario ingresa en una lista y use las funciones "max()" y "min()" para calcular los números máximo y mínimo después de que se complete el ciclo.  
Enter a number: 6  
Enter a number: 2  
Enter a number: 9  
Enter a number: 3  
Enter a number: 5  
Enter a number: done  
Maximum: 9.0  
Minimum: 2.0  

### DICCIONARIOS
### EJERCICIO 19: Escribe un programa que categorice cada mensaje de correo según el día de la semana en que se realizó la confirmación. Para hacer esto, busca líneas que comiencen con "From", luego busca la tercera palabra y manten un conteo de cada uno de los días de la semana. Al final del programa, imprime el contenido de tu diccionario (el orden no importa).  
### Línea de muestra:
From stephen.marquard@uct.ac.za Sat Jan  5 09:14:16 2008  
### Ejecución de la muestra:  
```
python dow.py
Enter a file name: mbox-short.txt
{'Fri': 20, 'Thu': 6, 'Sat': 1}  
```
### EJERCICIO 20: Escribe un programa que lea un registro de correo, cree un histograma usando un diccionario para contar cuántos mensajes has recibido de cada dirección de correo electrónico y luego imprima el diccionario.  
```
Enter file name: mbox-short.txt
{'gopal.ramasammycook@gmail.com': 1, 'louis@media.berkeley.edu': 3,
'cwen@iupui.edu': 5, 'antranig@caret.cam.ac.uk': 1,
'rjlowe@iupui.edu': 2, 'gsilver@umich.edu': 3,
'david.horwitz@uct.ac.za': 4, 'wagnermr@iupui.edu': 1,
'zqian@umich.edu': 4, 'stephen.marquard@uct.ac.za': 2,
'ray@media.berkeley.edu': 1}
```  
### EJERCICIO 21: Agrega código al programa anterior para averiguar quién tiene más mensajes en el archivo. Una vez que hayas leído todos los datos y se haya creado el diccionario, examina el diccionario utilizando un bucle máximo para encontrar quién tiene más mensajes e imprime cuántos mensajes tiene la persona.  
´´´  
Enter a file name: mbox-short.txt
cwen@iupui.edu 5

Enter a file name: mbox.txt
zqian@umich.edu 195  
´´´  
### EJERCICIO 22: Este programa registra el nombre de dominio (en lugar de la dirección) desde donde se envió el mensaje en lugar de a quién le llegó el correo (es decir, la dirección de correo electrónico completa). Al final del programa, imprime el contenido de tu diccionario.
´´´  
python schoolcount.py
Enter a file name: mbox-short.txt
{'media.berkeley.edu': 4, 'uct.ac.za': 6, 'umich.edu': 7,
'gmail.com': 1, 'caret.cam.ac.uk': 1, 'iupui.edu': 8}  
´´´  
