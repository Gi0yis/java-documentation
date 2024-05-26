# Casting en Java

En Java, el casting es el proceso de convertir un valor de un tipo de dato a otro. Existen dos tipos principales de casting: el casting implícito (automático) y el casting explícito (manual). Aquí te explico ambos tipos con ejemplos.

## 1. Casting Implícito (Automático)

El casting implícito ocurre cuando el compilador convierte automáticamente un tipo de dato en otro tipo compatible. Esto generalmente ocurre cuando se convierte un tipo de dato más pequeño en un tipo de dato más grande.

### Ejemplo:

```java
int entero = 100;
double doble = entero; // Conversión implícita de int a double

System.out.println(doble); // Salida: 100.0
```

En este ejemplo, el valor entero 100 se convierte automáticamente en un valor de tipo double.

## 2. Casting Explícito (Manual)

El casting explícito es necesario cuando se desea convertir un tipo de dato más grande en un tipo de dato más pequeño o en un tipo de dato incompatible. Este tipo de casting debe ser especificado manualmente.
Ejemplo:

```java

double doble = 100.25;
int entero = (int) doble; // Conversión explícita de double a int

System.out.println(entero); // Salida: 100
```

En este ejemplo, el valor 100.25 de tipo double se convierte manualmente en un valor de tipo int. La parte decimal se pierde durante esta conversión.

## 3. Casting en Tipos de Datos Primitivos

El casting también se puede realizar entre tipos de datos primitivos. A continuación se muestra cómo se puede convertir entre tipos numéricos.
Ejemplo:

```java

byte b = 10;
int i = b; // Conversión implícita de byte a int

int j = 100;
byte k = (byte) j; // Conversión explícita de int a byte

System.out.println(i); // Salida: 10
System.out.println(k); // Salida: 100
```

En este ejemplo, el valor de byte se convierte implícitamente a int, y el valor de int se convierte explícitamente a byte.

## Consideraciones Importantes

    - Pérdida de Datos: Al realizar el casting de un tipo más grande a uno más pequeño, es posible perder información, especialmente en el caso de números decimales y enteros.
    -  Seguridad en Tiempo de Ejecución: Siempre verifica la compatibilidad de tipos antes de realizar el downcasting usando instanceof para evitar excepciones.

El casting es una herramienta poderosa en Java, pero debe usarse con cuidado para evitar errores y pérdidas de datos.

# Tabla de Conversión de Tipos de Datos en Java

Esta tabla muestra ejemplos de cómo convertir entre diferentes tipos de datos primitivos en Java utilizando casting implícito y explícito.

| Tipo de Dato Original | Tipo de Dato Destino | Tipo de Casting     | Ejemplo                                                      | Resultado         |
|-----------------------|----------------------|---------------------|--------------------------------------------------------------|-------------------|
| `byte`                | `int`                | Implícito           | `byte b = 10; int i = b;`                                     | `i` = 10          |
| `int`                 | `byte`               | Explícito           | `int i = 100; byte b = (byte) i;`                             | `b` = 100         |
| `int`                 | `double`             | Implícito           | `int i = 100; double d = i;`                                  | `d` = 100.0       |
| `double`              | `int`                | Explícito           | `double d = 100.25; int i = (int) d;`                         | `i` = 100         |
| `float`               | `double`             | Implícito           | `float f = 10.5f; double d = f;`                              | `d` = 10.5        |
| `double`              | `float`              | Explícito           | `double d = 10.5; float f = (float) d;`                       | `f` = 10.5        |
| `long`                | `int`                | Explícito           | `long l = 100L; int i = (int) l;`                             | `i` = 100         |
| `int`                 | `long`               | Implícito           | `int i = 100; long l = i;`                                    | `l` = 100L        |
| `char`                | `int`                | Implícito           | `char c = 'A'; int i = c;`                                    | `i` = 65          |
| `int`                 | `char`               | Explícito           | `int i = 65; char c = (char) i;`                              | `c` = 'A'         |
| `short`               | `int`                | Implícito           | `short s = 10; int i = s;`                                    | `i` = 10          |
| `int`                 | `short`              | Explícito           | `int i = 100; short s = (short) i;`                           | `s` = 100         |
| `byte`                | `short`              | Implícito           | `byte b = 10; short s = b;`                                   | `s` = 10          |
| `short`               | `byte`               | Explícito           | `short s = 10; byte b = (byte) s;`                            | `b` = 10          |

**Nota:** El resultado del casting explícito puede perder información si el valor original no encaja en el rango del tipo de dato destino.

## Ejemplos de Código

### Conversión Implícita de `int` a `double`

```java
int entero = 100;
double doble = entero; // Conversión implícita de int a double

System.out.println(doble); // Salida: 100.0
```