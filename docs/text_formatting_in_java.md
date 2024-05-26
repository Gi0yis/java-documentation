# Formato de Textos en Java

En Java, el formato de textos se puede realizar utilizando varias técnicas y clases que ofrecen diferentes niveles de control y flexibilidad. Aquí te muestro algunas de las formas más comunes de formatear textos en Java:

## 1. Uso de `String.format()`

El método `String.format()` es una forma conveniente de formatear cadenas. Este método toma una cadena de formato y una lista de argumentos, y devuelve una nueva cadena con los argumentos insertados en los lugares apropiados.

### Ejemplo:

```java
int edad = 25;
String nombre = "Juan";
String mensaje = String.format("Mi nombre es %s y tengo %d años.", nombre, edad);
System.out.println(mensaje);
```

### Salida:

```css

Mi nombre es Juan y tengo 25 años.
```
## 2. Uso de System.out.printf()

El método System.out.printf() funciona de manera similar a String.format(), pero imprime directamente la cadena formateada en lugar de devolverla.
Ejemplo:

```java

int edad = 25;
String nombre = "Juan";
System.out.printf("Mi nombre es %s y tengo %d años.%n", nombre, edad);
```

### Salida:

```css

Mi nombre es Juan y tengo 25 años.
```

## 3. Uso de MessageFormat

La clase MessageFormat es útil para formatear mensajes con más complejidad y es particularmente buena para la internacionalización.
Ejemplo:

```java

import java.text.MessageFormat;

int edad = 25;
String nombre = "Juan";
String patron = "Mi nombre es {0} y tengo {1} años.";
String mensaje = MessageFormat.format(patron, nombre, edad);
System.out.println(mensaje);
```

### Salida:

```css

Mi nombre es Juan y tengo 25 años.
```

## 4. Uso de DecimalFormat

Para formatear números con más precisión, como decimales y porcentajes, puedes usar la clase DecimalFormat.
Ejemplo:

```java

import java.text.DecimalFormat;

double numero = 12345.6789;
DecimalFormat df = new DecimalFormat("#,###.00");
String formateado = df.format(numero);
System.out.println(formateado);
```

### Salida:

```css

12,345.68
```

## 5. Uso de SimpleDateFormat

Para formatear fechas, puedes utilizar la clase SimpleDateFormat.
Ejemplo:

```java

import java.text.SimpleDateFormat;
import java.util.Date;

Date fecha = new Date();
SimpleDateFormat sdf = new SimpleDateFormat("dd/MM/yyyy");
String fechaFormateada = sdf.format(fecha);
System.out.println(fechaFormateada);
```

## Salida (puede variar dependiendo de la fecha actual):

```css

25/05/2024
```

## 6. Uso de StringBuilder o StringBuffer

Para concatenar y construir cadenas de manera eficiente en un contexto en el que se realizan múltiples modificaciones de la cadena, StringBuilder o StringBuffer pueden ser útiles.
Ejemplo:

```java

StringBuilder sb = new StringBuilder();
sb.append("Mi nombre es ");
sb.append("Juan");
sb.append(" y tengo ");
sb.append(25);
sb.append(" años.");
System.out.println(sb.toString());
```

### Salida:

```css

Mi nombre es Juan y tengo 25 años.
```

Estas son algunas de las técnicas más comunes para formatear textos en Java. Dependiendo de tus necesidades específicas, puedes elegir la que mejor se adapte a tu caso.