# Trabajo Práctico Nº1 – Introducción a Java (Consola)

---

##  Objetivo del trabajo práctico
Que el estudiante sea capaz de:
- Verificar la instalación de Java
- Ejecutar programas Java desde la consola
- Comprender el flujo de compilación y ejecución
- Identificar y analizar errores comunes de compilación y ejecución

 #### ⚠️Importante 
 Las capturas se deben realizar en code block del formato markdown - **sin imagenes**,  solo el codigo formateado

##  Ejercicio 1 – Verificación del entorno

### Consigna
1. Abra una terminal o símbolo del sistema.
2. Ejecute el comando correspondiente para verificar la versión de Java instalada.
3. Registre la salida obtenida.

### Evidencia a entregar
- Captura de pantalla del comando ejecutado. 
- Versión de Java instalada.

### Preguntas
- ¿Qué indica que Java está correctamente instalado?
- ¿Por qué es importante la variable `PATH`?

---

##  Ejercicio 2 – Organización del proyecto

### Consigna
1. Cree una carpeta llamada `java-intro`.
2. Dentro de la carpeta, cree el archivo `MyFirstJavaApp.java`. y agreguele codigo simple
3. Desde la terminal, navegue hasta dicha carpeta.
4. Liste los archivos del directorio.

### Evidencia a entregar
- Captura del directorio con el archivo creado. (opcional)
- Comandos utilizados.

### Preguntas
- ¿Por qué los archivos fuente Java terminan en `.java`?
- ¿Qué función cumple el directorio de trabajo?

---

##  Ejercicio 3 – Primera ejecución

### Consigna
1. Ejecute el programa Java desde la terminal.
2. Observe el resultado obtenido.
3. Registre el comportamiento del sistema.

### Evidencia a entregar
- Captura de la ejecución.
- Resultado mostrado en consola.

### Preguntas
- ¿Qué diferencia existe entre compilar y ejecutar?
- ¿Qué ocurre si el archivo no existe?

---

##  Ejercicio 4 – Programa interactivo

### Consigna
Modifique el programa para que:
1. Muestre un mensaje inicial.
2. Solicite el nombre del usuario.
3. Muestre un saludo personalizado.

Ejecute el programa al menos dos veces con nombres distintos.

### Evidencia a entregar
- Capturas de las ejecuciones.
- Breve descripción del funcionamiento.

### Preguntas
- ¿Qué tipo de dato se utiliza para almacenar el nombre?
- ¿El programa se comporta igual con distintos valores?

---

##  Ejercicio 5 – Errores de compilación

### Consigna
1. Ejecute un programa con errores provisto por el docente.
2. Analice el mensaje del compilador.
3. Identifique:
   - Tipo de error
   - Línea donde ocurre
   - Posible causa
```java
public class ErroresCompilacion {

    public static void main(String[] args) {

        int numero = "10";

        System.out.println("El número es: " + numero)

        if (numero > 5) {
            System.out.println("Número mayor que 5");
        else
            System.out.println("Número menor o igual a 5");
        }

        suma = numero + 5;

        mostrarResultado(suma);
    }

    public static void mostrarResultado(int resultado) {
        System.out.println("Resultado final: " + resultadoo);
    }
}

```

### Evidencia a entregar
- Copia del mensaje de error.
- Explicación del problema.

### Preguntas
- ¿El error es sintáctico o semántico?
- ¿Se generó el archivo `.class`?

---

##  Ejercicio 6 – Errores de ejecución

### Consigna
Intente ejecutar un programa:
1. Desde un directorio incorrecto.
2. Usando el nombre del archivo `.class`.
3. Sin un método `main` válido.

### Evidencia a entregar
- Mensajes de error obtenidos.
- Explicación de cada caso.

### Preguntas
- ¿Qué busca la JVM al iniciar un programa?
- ¿Por qué el método `main` es obligatorio?

---

##  Ejercicio 7 – Reflexión final

### Consigna
Responda brevemente:
- Describa los pasos para ejecutar un programa Java desde cero.
- ¿Qué error le resultó más difícil de comprender?
- ¿Qué ventajas cree que ofrecen los IDE frente a la consola?

---

##  Forma de entrega
- Un único archivo `README.md` o `TP1-Java.md`
- Repositorio Git
- Capturas correctamente rotuladas



---


