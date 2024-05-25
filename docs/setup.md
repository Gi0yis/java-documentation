# Configuración del Entorno

El JDK (Java Development Kit) es un conjunto de herramientas y bibliotecas de software que permite el desarrollo de aplicaciones Java.

## Instalaremos el JDK para empezar a crear nuestros primeros programas en Java.

### Linux

1. Abre la terminal y ejecuta el siguiente comando para actualizar la lista de paquetes disponibles en los repositorios del sistema:

    ```bash
    sudo apt update
    ```

2. Instala la versión 17 del JDK con el siguiente comando:

    ```bash
    sudo apt install openjdk-17-jdk
    ```

    Esto descargará e instalará el paquete OpenJDK 17 JDK, permitiéndote desarrollar aplicaciones Java en Linux.

3. Configura la variable de entorno `JAVA_HOME`, que indica la ubicación del JDK. Esto es necesario para usar herramientas del JDK como `javac`.

    ```bash
    sudo update-alternatives --config java
    ```

4. Copia la ruta mostrada hasta `/bin`, por ejemplo: `/usr/lib/jvm/java-17-openjdk-amd64/bin`.

5. En la terminal, escribe el siguiente comando, reemplazando la ruta por la que copiaste:

    ```bash
    export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64/bin
    ```

6. Presiona "Enter". El JDK está instalado y configurado. Para verificarlo, escribe los siguientes comandos en la terminal:

    ```bash
    javac -version
    java -version
    ```

### Mac

1. Accede al sitio web de Oracle ([Java Downloads | Oracle](https://www.oracle.com/java/technologies/javase-downloads.html)) o busca "Java Download Oracle" en el navegador y haz clic en el primer enlace.
2. Selecciona la versión de Java. En este curso utilizaremos Java 17 LTS, la versión de soporte a largo plazo más reciente para la plataforma Java SE.
3. Selecciona Mac como sistema operativo y realiza la descarga.

### Windows

1. Accede al sitio web de Oracle ([Java Downloads | Oracle](https://www.oracle.com/java/technologies/javase-downloads.html)) o busca "Java Download Oracle" en el navegador y haz clic en el primer enlace.
2. Selecciona la versión de Java. En este curso utilizaremos Java 17 LTS, la versión de soporte a largo plazo más reciente para la plataforma Java SE.
3. Selecciona Windows como sistema operativo y realiza la descarga.
4. Una vez descargado, ejecuta el instalador y sigue las instrucciones de instalación.
5. Para verificar la instalación, abre la ventana de comandos y ejecuta los siguientes comandos:

    ```bash
    java -version
    javac -version
    ```

### Configuración de la Variable PATH en Windows

1. Ve al Panel de Control y busca "Sistema", luego haz clic en "Configuración avanzada del sistema".
2. En la pestaña "Avanzado", haz clic en "Variables de entorno".
3. En la nueva ventana, selecciona la variable de entorno llamada "Path" y haz clic en "Editar".
4. Haz clic en el botón "Nuevo" y añade la ruta hacia el directorio `bin` dentro de la carpeta `jdk`, que se encuentra dentro de la carpeta `Java`.
5. Cierra la ventana de comandos y ábrela nuevamente. Ejecuta los siguientes comandos para verificar la configuración:

    ```bash
    java -version
    javac -version
    ```
