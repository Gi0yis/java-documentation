# Clase `Scanner` en Java

La clase `Scanner` en Java se utiliza para leer la entrada del usuario a través de varias fuentes, como la consola. Es una herramienta poderosa y fácil de usar para manejar la entrada en programas Java.

## Sintaxis Básica

Para utilizar la clase `Scanner`, primero debes importarla de la biblioteca `java.util`.

```java
import java.util.Scanner;
```

## Creación de un Objeto `Scanner`

Puedes crear un objeto `Scanner` utilizando la consola como fuente de entrada:

```java
Scanner scanner = new Scanner(System.in);
```

## Métodos Comunes de la Clase `Scanner`

- `nextInt()`: Lee un entero.
- `nextDouble()`: Lee un número de punto flotante.
- `nextLine()`: Lee una línea completa de texto.
- `next()`: Lee una sola palabra.
- `hasNext()`: Devuelve `true` si hay otra palabra en la entrada.
- `hasNextInt()`, `hasNextDouble()`: Verifican si el siguiente token es del tipo especificado.

## Ejemplo de Uso: Leer Desde la Consola

A continuación se muestra un ejemplo simple de cómo usar la clase `Scanner` para leer diferentes tipos de datos desde la consola.

```java
import java.util.Scanner;

public class EjemploScanner {
    public static void main(String[] args) {
        // Crear un objeto Scanner para leer desde la consola
        Scanner scanner = new Scanner(System.in);

        // Leer un entero
        System.out.print("Ingresa un número entero: ");
        int numero = scanner.nextInt();

        // Leer un número de punto flotante
        System.out.print("Ingresa un número con decimales: ");
        double decimal = scanner.nextDouble();

        // Consumir la línea restante
        scanner.nextLine();

        // Leer una línea completa de texto
        System.out.print("Ingresa una línea de texto: ");
        String linea = scanner.nextLine();

        // Leer una sola palabra
        System.out.print("Ingresa una palabra: ");
        String palabra = scanner.next();

        // Mostrar los datos leídos
        System.out.println("Número entero: " + numero);
        System.out.println("Número decimal: " + decimal);
        System.out.println("Línea de texto: " + linea);
        System.out.println("Palabra: " + palabra);

        // Cerrar el objeto Scanner
        scanner.close();
    }
}
```

## Explicación del Ejemplo

1. **Importar la Clase `Scanner`:**

    ```java
    import java.util.Scanner;
    ```

2. **Crear un Objeto `Scanner`:**

    ```java
    Scanner scanner = new Scanner(System.in);
    ```
    

3. **Leer Diferentes Tipos de Datos:**

    - `nextInt()`: Lee un número entero.
    - `nextDouble()`: Lee un número de punto flotante.
    - `nextLine()`: Lee una línea completa de texto.
    - `next()`: Lee una sola palabra.

4. **Cerrar el Objeto `Scanner`:**

    ```java
    scanner.close();
    ```

Es importante cerrar el objeto `Scanner` después de que hayas terminado de usarlo para liberar los recursos asociados.

La clase `Scanner` es una herramienta fundamental para manejar la entrada del usuario en aplicaciones Java, proporcionando métodos fáciles de usar para leer y procesar datos de diferentes tipos.