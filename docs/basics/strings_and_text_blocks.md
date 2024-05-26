# Strings y Bloques de Texto en Java

En Java, la clase `String` es una de las más importantes y utilizadas. Esta clase se encarga de representar una secuencia de caracteres, es decir, un texto.

## Creación de Strings

Para crear una `String` en Java, simplemente se utilizan comillas dobles para delimitar el texto. Por ejemplo:

```java
String nombre = "Juan";
```

En este ejemplo, la variable nombre recibe una String con el texto "Juan". Es posible concatenar dos o más Strings utilizando el operador +, por ejemplo:

```java

String saludo = "Hola, ";
String nombre = "Juan";
String mensaje = saludo + nombre + "!";
```

En este caso, la variable mensaje recibirá la cadena "¡Hola, Juan!".
Comparación de Strings

En Java, es posible comparar dos Strings utilizando el operador ==. Sin embargo, este operador solo verifica si las dos variables apuntan al mismo objeto en la memoria, no si el contenido de las Strings es igual. Para comparar el contenido de dos Strings, es necesario utilizar el método equals(). Por ejemplo:

```java

String contrasena = "12345";
if (contrasena.equals("12345")) {
    System.out.println("¡Acceso autorizado!");
} else {
    System.out.println("Contraseña incorrecta.");
}
```

En este caso, el método equals() se utiliza para comparar el contenido de la variable contrasena con la cadena "12345". Si las dos cadenas son iguales, se imprimirá el mensaje "¡Acceso autorizado!", de lo contrario, se imprimirá el mensaje "Contraseña incorrecta".

Más adelante, también trabajaremos con el método equalsIgnoreCase(), que se utiliza para que la comparación de Strings no distinga entre mayúsculas y minúsculas. Utilizando solo equals, las cadenas "alura" y "Juan" se considerarían diferentes.
Bloque de Texto

Introducido en la versión 15 de Java, el bloque de texto (Text Block) es una nueva forma de representar cadenas que facilita la escritura de textos con múltiples líneas. En lugar de utilizar comillas dobles para delimitar el texto e insertar saltos de línea manualmente o utilizar concatenaciones, es posible utilizar una sintaxis más sencilla que permite insertar el texto exactamente como es.
Sintaxis del Bloque de Texto

Para crear un bloque de texto en Java, simplemente se utilizan tres comillas dobles para delimitar el texto, seguidas de un salto de línea. Por ejemplo:

```java

String mensaje = """
                  Hola, mundo!
                  Este es un Text Block.
                  Permite escribir textos con múltiples líneas
                  sin necesidad de usar caracteres de escape, saltos de línea manualmente o concatenaciones.
                  """;
```

En este ejemplo, la variable mensaje recibe un bloque de texto (Text Block) con el texto "¡Hola, mundo! Este es un bloque de texto. Permite escribir textos con varias líneas sin necesidad de usar caracteres de escape, saltos de línea manualmente o concatenaciones."