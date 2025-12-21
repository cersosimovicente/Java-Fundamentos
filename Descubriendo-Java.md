# Descubriendo Java 

Este tutorial está pensado como un **recorrido progresivo** para *descubrir Java*, desde cómo estructurar una aplicación simple y compilarla, hasta avanzar gradualmente en las características más importantes del lenguaje.


---

## 1. ¿Qué es Java?

Java es un **lenguaje de programación orientado a objetos**, multiplataforma y fuertemente tipado. Su principal característica es que el código se compila a **bytecode**, el cual se ejecuta en la **Java Virtual Machine (JVM)**.

> *"Write Once, Run Anywhere"*

---

## 2. Requisitos previos

Antes de comenzar, necesitamos:

- **JDK (Java Development Kit)** instalado
- Un editor de texto o IDE (VS Code, IntelliJ, NetBeans, etc.)
- Consola / terminal

Verificar instalación:

```bash
java --version
javac --version
```

---

## 3. Estructura básica de una aplicación Java

En Java, todo programa se organiza en **clases**.

### 3.1 Primer programa: `HolaMundo`

Crear un archivo llamado **HolaMundo.java**

```java
public class HolaMundo {

    public static void main(String[] args) {
        System.out.println("Hola Mundo desde Java");
    }
}
```

### ¿Qué estamos viendo?

- `class` → define una clase
- `public` → modificador de acceso
- `static` → pertenece a la clase
- `void` → no retorna valor
- `main` → punto de entrada del programa

---

## 4. Compilación y ejecución

Desde la carpeta donde está el archivo:

### 4.1 Compilar

```bash
javac HolaMundo.java
```

Esto genera:

```
HolaMundo.class
```

### 4.2 Ejecutar

```bash
java HolaMundo
```

---

## 5. Organización en paquetes

Los **paquetes** permiten organizar el código.

Ejemplo:

```java
package app;

public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("Hola Mundo con paquetes");
    }
}
```

Estructura de carpetas:

```
app/
 └── HolaMundo.java
```

Compilación:

```bash
javac app/HolaMundo.java
java app.HolaMundo
```

---

## 6. Variables y tipos de datos

Java es **fuertemente tipado**.

```java
int edad = 20;
double precio = 1500.50;
char letra = 'A';
boolean activo = true;
String nombre = "Juan";
```

---

## 7. Entrada y salida por consola

```java
import java.util.Scanner;

public class EntradaDatos {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Ingrese su nombre: ");
        String nombre = sc.nextLine();

        System.out.println("Hola " + nombre);
    }
}
```

---

## 8. Estructuras de control

### 8.1 Condicionales

```java
if (edad >= 18) {
    System.out.println("Mayor de edad");
} else {
    System.out.println("Menor de edad");
}
```

### 8.2 Bucles

```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

```java
while (contador < 5) {
    contador++;
}
```

---

## 9. Métodos

```java
public static int sumar(int a, int b) {
    return a + b;
}
```

Uso:

```java
int resultado = sumar(3, 4);
```

---

## 10. Introducción a la Programación Orientada a Objetos

### 10.1 Clases y objetos

```java
public class Persona {
    String nombre;
    int edad;

    void saludar() {
        System.out.println("Hola, soy " + nombre);
    }
}
```

```java
public class Principal {
    public static void main(String[] args) {
        Persona p = new Persona();
        p.nombre = "Ana";
        p.edad = 30;
        p.saludar();
    }
}
```

---

## 11. Conceptos clave que iremos descubriendo

En las siguientes etapas del tutorial se profundizará en:

- Encapsulamiento
- Constructores
- Herencia
- Polimorfismo
- Interfaces
- Excepciones
- Colecciones (List, Set, Map)
- Streams y lambdas
- Manejo de archivos (NIO.2)
- Maven y estructura profesional de proyectos

---




