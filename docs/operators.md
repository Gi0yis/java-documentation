# Operadores en Java

Los operadores en Java son símbolos especiales que realizan operaciones en uno o más operandos. Aquí se presentan los diferentes tipos de operadores que puedes encontrar en Java:

## Operadores Aritméticos

Los operadores aritméticos se utilizan para realizar operaciones matemáticas básicas.

- **Suma (+)**: Suma dos operandos.
- **Resta (-)**: Resta el segundo operando del primero.
- **Multiplicación (*)**: Multiplica dos operandos.
- **División (/)**: Divide el primer operando por el segundo.
- **Módulo (%)**: Devuelve el residuo de la división.

## Operadores de Asignación

Los operadores de asignación se utilizan para asignar valores a variables.

- **Asignación simple (=)**: Asigna el valor del lado derecho al operando del lado izquierdo.
- **Asignación compuesta (+=, -=, *=, /=, %=)**: Realiza una operación específica y luego asigna el resultado a la variable.

## Operadores de Comparación

Los operadores de comparación se utilizan para comparar valores.

- **Igual a (==)**: Comprueba si dos operandos son iguales.
- **No igual a (!=)**: Comprueba si dos operandos no son iguales.
- **Mayor que (>)**: Comprueba si el operando de la izquierda es mayor que el operando de la derecha.
- **Mayor o igual que (>=)**: Comprueba si el operando de la izquierda es mayor o igual que el operando de la derecha.
- **Menor que (<)**: Comprueba si el operando de la izquierda es menor que el operando de la derecha.
- **Menor o igual que (<=)**: Comprueba si el operando de la izquierda es menor o igual que el operando de la derecha.

## Operadores Lógicos

Los operadores lógicos se utilizan para realizar operaciones lógicas en valores booleanos.

- **AND lógico (&&)**: Devuelve verdadero si ambos operandos son verdaderos.
- **OR lógico (||)**: Devuelve verdadero si al menos uno de los operandos es verdadero.
- **NOT lógico (!)**: Devuelve el valor opuesto del operando.

## Operadores de Incremento y Decremento

Los operadores de incremento y decremento se utilizan para aumentar o disminuir el valor de una variable en uno.

- **Incremento (++var o var++)**: Aumenta el valor de la variable en uno.
- **Decremento (--var o var--)**: Disminuye el valor de la variable en uno.

## Operadores de Ternario

El operador ternario es una forma abreviada de escribir una instrucción if-else.

- **Operador ternario (condición ? expr1 : expr2)**: Si la condición es verdadera, devuelve expr1; de lo contrario, devuelve expr2.

## Operador de Concatenación de Cadenas

El operador de concatenación de cadenas (`+`) se utiliza para concatenar dos cadenas.

- **Concatenación de Cadenas (+)**: Une dos cadenas de texto.

Ejemplo:

```java
String firstName = "John";
String lastName = "Doe";
String fullName = firstName + " " + lastName;
System.out.println(fullName); // Imprimirá "John Doe"
