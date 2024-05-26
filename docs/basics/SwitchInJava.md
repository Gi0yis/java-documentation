# El `switch` en Java

El `switch` es una estructura de control que permite ejecutar diferentes bloques de código basándose en el valor de una expresión. Es útil cuando necesitas comparar una variable contra múltiples valores posibles y ejecutar diferentes bloques de código según el valor de la variable.

## Sintaxis Básica

```java
switch (expresión) {
    case valor1:
        // código a ejecutar si expresión == valor1
        break;
    case valor2:
        // código a ejecutar si expresión == valor2
        break;
    // más casos ...
    default:
        // código a ejecutar si expresión no coincide con ningún caso
}
```


- **expresión:** La variable o expresión que se evalúa.
- **case valor:** Cada caso compara la expresión con un valor específico.
- **break:** Termina la ejecución del caso y sale del `switch`.
- **default:** (Opcional) Se ejecuta si la expresión no coincide con ningún caso.

## Ejemplo de `switch`

A continuación se muestra un ejemplo en el que se utiliza `switch` para determinar el nombre de un día de la semana basado en un número:

```java
public class EjemploSwitch {
    public static void main(String[] args) {
        int dia = 3;
        String nombreDia;

        switch (dia) {
            case 1:
                nombreDia = "Lunes";
                break;
            case 2:
                nombreDia = "Martes";
                break;
            case 3:
                nombreDia = "Miércoles";
                break;
            case 4:
                nombreDia = "Jueves";
                break;
            case 5:
                nombreDia = "Viernes";
                break;
            case 6:
                nombreDia = "Sábado";
                break;
            case 7:
                nombreDia = "Domingo";
                break;
            default:
                nombreDia = "Día inválido";
                break;
        }

        System.out.println("El día es: " + nombreDia);
    }
}
```

## Explicación del Ejemplo

1. **Declaración y Inicialización:**

    ```java
    int dia = 3;
    String nombreDia;
    ```

2. **Estructura `switch`:**

```java
    switch (dia) {
        case 1:
            nombreDia = "Lunes";
            break;
        case 2:
            nombreDia = "Martes";
            break;
        case 3:
            nombreDia = "Miércoles";
            break;
        case 4:
            nombreDia = "Jueves";
            break;
        case 5:
            nombreDia = "Viernes";
            break;
        case 6:
            nombreDia = "Sábado";
            break;
        case 7:
            nombreDia = "Domingo";
            break;
        default:
            nombreDia = "Día inválido";
            break;
    }
```

3. **Salida del Resultado:**

```java
    System.out.println("El día es: " + nombreDia);
```

## Salida

```css
El día es: Miércoles
```

En este ejemplo, la variable `dia` tiene el valor `3`, por lo que el caso correspondiente es `case 3`, y se asigna "Miércoles" a `nombreDia`. El uso del `break` asegura que solo se ejecute el código correspondiente al caso que coincide con `dia`, evitando la ejecución en cascada de otros casos. Si `dia` no coincide con ninguno de los valores especificados en los `case`, se ejecuta el bloque `default`.
