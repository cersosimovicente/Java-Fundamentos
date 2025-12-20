# Creando un primer programa Java

El primer paso que debes saber es que el código Java que escribes se guarda en **archivos de texto sin formato**. En este tutorial, tu aplicación se escribirá en un solo archivo de texto. Las aplicaciones más grandes pueden requerir miles de archivos de este tipo.

## Creación del archivo

El primer paso consiste en crear un archivo y asignarle un nombre. A continuación, asumiremos que el nombre es: `MyFirstJavaApp.java` 

Podes asignarle cualquier nombre, siempre que conserve la extensión `.java`. 

#### tarea 1
Crea en la carpeta raiz el archivo `MyFirstJavaApp.java` y abrilo con el editor de codigo
```java 
touch MyFirstJavaApp.java
```

## Convenciones de nombres en Java

También existen restricciones sobre el primer carácter del nombre del archivo. Para simplificar, podes usar una **letra** como primer carácter.  
Existe una convención en Java: **el nombre de un archivo Java debe empezar con mayúscula**.

> Esto no es obligatorio, pero todos los desarrolladores Java siguen esta convención.  
> Cuando te conviertas en un desarrollador Java experimentado, ver una clase que no siga esta convención te resultará extraño.

## Editor de texto

Ahora podes abrir este archivo en un editor de texto.  
 **Advertencia**: debes usar un **editor de texto simple** para crear y guardar este archivo.  
Usar un procesador de texto no funcionará.

Algunos ejemplos de editores de texto adecuados son:

- Bloc de notas
- Visual Studio Code
- Notepad++
- Sublime Text

## Primer código Java

Una vez que hayas abierto el archivo `MyFirstJavaApp.java`, podes copiar y pegar el siguiente código en él.

Como sabrán, existe una larga tradición en informática: escribir un programa que muestre **"¡Hola, mundo!"** en la consola de su aplicación.

¡Hagámoslo!

```java
//funciona solo para java 25
void main() {
    IO.println("Hello, World!");
}
```
Podes verificar la version con `java --version`
```java
//cualquier version de java
class MyFirstJavaApp {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```
# Preparando la ejecución de su primer programa

La compilación y la ejecución de programas simples son solo un paso que sigue a la creación de su primer programa.

Hasta ahora, la única herramienta que has usado es un **editor de texto plano**. Ejecutar este programa requiere otra herramienta; algo que quizás no tengas en tu computadora. Afortunadamente, podes descargar este compilador y usarlo de forma gratuita. 

## ¿Qué es el JDK?

Actualmente, descargar **Java** implica descargar el **Kit de Desarrollo de Java (JDK)**.

El JDK contiene numerosas herramientas, entre ellas las que se utilizan para:

- Compilar aplicaciones Java
- Ejecutar aplicaciones Java

El JDK es distribuido oficialmente por:

- **OpenJDK**
- **Oracle**

## Otros términos relacionados con Java

Es posible que hayas oído hablar de otros componentes que también se denominan “Java”. A continuación, aclaramos las diferencias.

### JRE (Java Runtime Environment)

- Es un **subconjunto del JDK**
- Ya no es distribuido por OpenJDK ni por Oracle
- Solo contiene las herramientas necesarias para **ejecutar** aplicaciones Java
- ❌ **No permite compilar código Java**

### Java EE / J2EE / Jakarta EE

- Estas siglas se refieren a **Java Enterprise Edition**
- Es un conjunto de **herramientas y bibliotecas** para crear aplicaciones empresariales
- Es diferente del JDK
- ❌ **No es necesario** para compilar y ejecutar la aplicación sencilla que estamos creando en este tutorial

> Java EE queda fuera del alcance de este tutorial.

