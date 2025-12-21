# Cómo compilar y ejecutar su primer programa Java

Una vez que haya configurado correctamente su **JDK**, la variable **JAVA_HOME** y la variable **PATH**, estará listo para ejecutar su primer programa.

Todos los comandos que escribirá ahora deben hacerse en el mismo intérprete de comandos que utilizó para configurar estas variables.

Independientemente de si siguió el camino de **Windows**, **Linux** o **macOS**, el resto del proceso es el mismo.

---

## Compilación y ejecución del primer programa

1. Cambie al directorio donde guardó su primera clase `MyFirstJavaApp.java`.

   Puede comprobar que está en el directorio correcto escribiendo:

   ```bash
   dir
   ```

   Debería ver el archivo `MyFirstJavaApp.java`.

2. Compruebe que Java sea accesible desde este directorio:

   ```bash
   java -version
   ```

   Este comando debe mostrar la versión de Java instalada.  
   Si aparece un error, revise las variables **JAVA_HOME** y **PATH**.

3. Ejecute su primer programa Java:

   ```bash
   java MyFirstJavaApp.java
   ```

### Posibles resultados

- Si aparecen mensajes de error, el compilador no pudo compilar el código.  
  Corrija los errores y vuelva a intentarlo.
- Si no hay errores y se imprime:

  ```text
  Hello World!
  ```

   **¡Felicitaciones!** Su programa se compiló y ejecutó correctamente.

---

## Cómo hacer que su programa sea interactivo

Modifique su archivo `MyFirstJavaApp.java` y agregue el siguiente código:

```java
void main() {
   IO.println("Hello world!");
   var name = IO.readln("What is your name? ");
   IO.println("Hello " + name);
}
```

Ejecute nuevamente:

```bash
java MyFirstJavaApp.java
```

Salida esperada:

```text
Hello world!
What is your name? Mary
Hello Mary
```

 ¡Ahora está listo para crear aplicaciones más complejas!

---

## Problemas comunes y sus soluciones

### Problemas del compilador

#### Errores comunes en Microsoft Windows

**Error**
```text
javac is not recognized as an internal or external command
```

 Windows no puede encontrar el compilador `javac`.

Solución temporal (ejemplo con JDK 25):

```bash
C:\jdk25\bin\javac HelloWorldApp.java
```

Solución definitiva: agregar `C:\jdk25\bin` a la variable **PATH**.

---

**Error**
```text
Class names, HelloWorldApp, are only accepted if annotation processing is explicitly requested
```

 Olvidó incluir el sufijo `.java`.

Correcto:
```bash
javac HelloWorldApp.java
```

Incorrecto:
```bash
javac HelloWorldApp
```

---

#### Errores comunes en sistemas UNIX / Linux

**Error**
```text
javac: command not found
```

Solución temporal:

```bash
/ usr/local/jdk25/bin/javac HelloWorldApp.java
```

Solución definitiva: agregar la ruta del JDK a la variable **PATH**.

---

### Errores de sintaxis (todas las plataformas)

Ejemplo de error por falta de punto y coma:

```text
Testing.java:8: error: ';' expected
count++
^
1 error
```

 El programa no se compiló correctamente y no se generó el archivo `.class`.

---

### Errores semánticos

Ejemplo de uso de una variable no inicializada:

```text
Testing.java:8: error: variable count might not have been initialized
count++;
^
2 errors
```

 Corrija el error e intente nuevamente.

---

## Problemas en tiempo de ejecución

### Windows

**Error**
```text
Could not find or load main class HelloWorldApp.class
```

Solución:
1. Cambie al directorio donde está el archivo `.class`:
   ```bash
   cd c:\java
   ```
2. Ejecute:
   ```bash
   java HelloWorldApp
   ```

Si persiste el error, pruebe:
```bash
set CLASSPATH=
```

---

**Error**
```text
java.lang.NoSuchMethodError: main
```

 La clase no tiene un método `main` válido.

---

### UNIX / Linux

**Error**
```text
java.lang.NoClassDefFoundError: HelloWorldApp
```

Solución:
```bash
cd /home/jdoe/java
java HelloWorldApp
```

Si es necesario:
```bash
unset CLASSPATH
```

---

## Yendo más allá

Este primer programa Java mostró los pasos básicos:

1. Crear archivos fuente `.java`
2. Compilarlos en archivos `.class`
3. Ejecutarlos como una aplicación

En proyectos grandes, los desarrolladores utilizan **IDE (Entornos de Desarrollo Integrados)**, que facilitan la compilación, detección de errores y ejecución.

Algunos IDE populares y gratuitos:

- **Eclipse** (Eclipse Foundation)
- **NetBeans** (Apache Foundation)
- **IntelliJ IDEA Community Edition** (JetBrains)

---

 Fin del apunte introductorio de Java.

