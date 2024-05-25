# Tipos de Datos Primitivos en Java

Java es un lenguaje de programación fuertemente tipado, lo que significa que cada variable debe declararse con un tipo de dato específico. Los tipos de datos primitivos son los tipos más básicos que no son objetos y representan valores simples. Java tiene ocho tipos de datos primitivos:

## Enteros

1. **byte**
   - Tamaño: 8 bits
   - Rango: -128 a 127
   - Uso: Se utiliza para ahorrar espacio en matrices grandes donde los ahorros de memoria son importantes.
   - Ejemplo: `byte b = 100;`

2. **short**
   - Tamaño: 16 bits
   - Rango: -32,768 a 32,767
   - Uso: Similar a `byte`, pero con un rango mayor.
   - Ejemplo: `short s = 10000;`

3. **int**
   - Tamaño: 32 bits
   - Rango: -2^31 a 2^31-1
   - Uso: Tipo de datos entero más comúnmente utilizado.
   - Ejemplo: `int i = 100000;`

4. **long**
   - Tamaño: 64 bits
   - Rango: -2^63 a 2^63-1
   - Uso: Cuando se necesita un rango más amplio que el proporcionado por `int`.
   - Ejemplo: `long l = 100000L;`

## Punto Flotante

1. **float**
   - Tamaño: 32 bits
   - Precisión: Aproximadamente 7 dígitos decimales significativos
   - Uso: Utilizado para ahorrar memoria en grandes matrices de números decimales.
   - Ejemplo: `float f = 234.5f;`

2. **double**
   - Tamaño: 64 bits
   - Precisión: Aproximadamente 15 dígitos decimales significativos
   - Uso: Tipo de datos de punto flotante más utilizado.
   - Ejemplo: `double d = 123.4;`

## Caracter

1. **char**
   - Tamaño: 16 bits
   - Rango: '\u0000' (0) a '\uffff' (65,535)
   - Uso: Almacena caracteres individuales. Representa un solo carácter Unicode.
   - Ejemplo: `char c = 'A';`

## Booleano

1. **boolean**
   - Tamaño: 1 bit (pero la implementación real puede diferir)
   - Valores posibles: `true` o `false`
   - Uso: Representa valores verdaderos y falsos.
   - Ejemplo: `boolean b = true;`

## Tabla Resumen

| Tipo    | Tamaño  | Rango                            | Ejemplo              |
|---------|---------|----------------------------------|----------------------|
| byte    | 8 bits  | -128 a 127                       | `byte b = 100;`      |
| short   | 16 bits | -32,768 a 32,767                 | `short s = 10000;`   |
| int     | 32 bits | -2^31 a 2^31-1                   | `int i = 100000;`    |
| long    | 64 bits | -2^63 a 2^63-1                   | `long l = 100000L;`  |
| float   | 32 bits | Aproximadamente 7 dígitos        | `float f = 234.5f;`  |
| double  | 64 bits | Aproximadamente 15 dígitos       | `double d = 123.4;`  |
| char    | 16 bits | '\u0000' (0) a '\uffff' (65,535) | `char c = 'A';`      |
| boolean | 1 bit   | `true` o `false`                 | `boolean b = true;`  |

Los tipos de datos primitivos son los bloques de construcción básicos para la manipulación de datos en Java. Es importante comprender sus características y limitaciones para usarlos de manera efectiva en tus programas.
