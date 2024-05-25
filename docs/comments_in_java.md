# Comentarios en Java

Los comentarios son fragmentos de texto que se incluyen en el código fuente de un programa para proporcionar información adicional sobre cómo funciona el código, su propósito o cualquier otra aclaración relevante. En Java, los comentarios son ignorados por el compilador y están presentes únicamente para ayudar a los desarrolladores a entender y mantener el código.

## Comentarios de una línea

Los comentarios de una línea, también conocidos como *single-line comments*, son una forma sencilla de añadir comentarios breves y concisos en el código Java. Estos comentarios comienzan con dos barras inclinadas (`//`) y se extienden hasta el final de la línea. El compilador de Java los ignora por completo, por lo que no afectan la ejecución del programa.

Ejemplo:

```java
// Declaración de variables
int num1 = 10;
int num2 = 20;

// Cálculo de la suma
int suma = num1 + num2;

// Impresión del resultado en la consola
System.out.println("La suma de " + num1 + " y " + num2 + " es: " + suma);
```

## Comentarios de varias líneas

Los comentarios de varias líneas, también conocidos como *multi-line comments*, se utilizan para explicar bloques más extensos de código. Estos comentarios comienzan con `/*` y terminan con `*/`.

Ejemplo:

```java
/*
 * Este es un comentario de varias líneas.
 * Puede abarcar múltiples líneas de código.
 * Es útil para explicar algoritmos o secciones complejas.
 */
```