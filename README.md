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
> 
# Configuración de un Kit de Desarrollo de Java (JDK)
Podes descargar el JDK desde diferentes sitios. Existe una página que siempre te remite a la **última versión del JDK**:
 https://jdk.java.net/

Al seleccionar la última versión del JDK **“Listo para usar”**, accederás a una página donde podrás descargar la versión del JDK que necesitas según tu sistema operativo.

## Versiones disponibles

Desde esta página puedes descargar las siguientes versiones:

- Linux/AArch64  
- Linux/x64  
- macOS/x64  
- macOS/AArch64  
- Windows/x64  

Esta página proporciona **compilaciones de código abierto listas para producción** del *Java Development Kit*, una implementación de la plataforma **Java SE** bajo la **Licencia Pública General GNU, versión 2**, con la **excepción Classpath**.

---

## Configuración de un JDK para Windows/x64

Descarguemos la versión para **Windows/x64**.

Al hacerlo, obtendrás un archivo **ZIP** de aproximadamente **200 MB**, que puedes abrir con cualquier utilidad de compresión ZIP.  
Este archivo ZIP contiene el JDK completo.

Podes **descomprimirlo en cualquier ubicación** de tu computadora.

---

## Configuración de la variable de entorno JAVA_HOME

Una vez descomprimido el JDK, debes crear una **variable de entorno** llamada `JAVA_HOME` que apunte al directorio donde se encuentra el JDK.

### Pasos

1. Abre un **Símbolo del sistema**.
2. Si descomprimiste el JDK 25 en el directorio `D:\jdk\`, escribe el siguiente comando:

```bash
set JAVA_HOME=D:\jdk\jdk-25
```
⚠️ Nota:
En este ejemplo (y en los siguientes), el carácter inicial > solo indica que debes escribir el comando en la consola.
No debes escribir ni copiar ese carácter, ya que no forma parte del comando set.

## Verificación de la variable JAVA_HOME
Puedes comprobar que la variable JAVA_HOME se ha configurado correctamente escribiendo el siguiente comando:
```bash
echo %JAVA_HOME%
```
Si la configuración es correcta, se mostrará en pantalla la ruta al directorio del JDK.

Este comando debería imprimir lo siguiente:
```sh
D:\jdk\jdk-25
```
## Configuración de la variable de entorno PATH

Luego, debes actualizar la variable de entorno `PATH` para agregar el directorio `bin` de tu JDK.  
Esto se puede hacer con el siguiente comando:

```bash
set PATH=%JAVA_HOME%\bin;%PATH%
```
⚠️ Importante
Debes tener mucho cuidado al configurar estas dos variables, ya que un solo error —como un espacio en blanco agregado o un punto y coma faltante— provocará una falla en la ejecución de los comandos de Java.

#### Advertencia sobre la sesión de la consola
No cierres este símbolo del sistema.
Si lo cierras y lo vuelves a abrir, deberás volver a crear las variables JAVA_HOME y PATH, ya que estos comandos solo aplican a la sesión actual de la consola.
