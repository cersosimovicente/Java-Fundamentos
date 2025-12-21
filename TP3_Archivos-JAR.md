# Ejercicios – Ficheros JAR en Java

## Objetivo general
Que el estudiante comprenda y practique el uso de ficheros JAR para empaquetar, inspeccionar, modificar y ejecutar aplicaciones Java desde la línea de comandos.

---

## Ejercicio 1 – Conceptos básicos (teórico)

Responder con sus propias palabras:

1. ¿Qué es un fichero JAR?
2. ¿Qué ventajas tiene usar un JAR frente a distribuir archivos `.class` sueltos?
3. ¿En qué se parece y en qué se diferencia un JAR de un archivo `.zip`?
4. ¿Qué comando de Java se utiliza para trabajar con ficheros JAR?

---

## Ejercicio 2 – Identificación de opciones del comando `jar`

Dado el siguiente comando:

```bash
jar -cf programa.jar *.class
```

Indicar:
1. ¿Qué hace la opción `c`?
2. ¿Qué hace la opción `f`?
3. ¿Qué archivos se incluyen dentro del JAR?
4. ¿Qué ocurre si `programa.jar` ya existía?

---

## Ejercicio 3 – Creación de un JAR sin paquetes

1. Crear una clase Java simple llamada `Saludo` con un método `main`.
2. Compilar la clase.
3. Crear un fichero JAR que contenga el archivo `.class`.
4. Listar el contenido del JAR creado.
5. Explicar qué información muestra el listado.

> **Entrega:** captura de pantalla de los comandos utilizados y breve explicación.

---

## Ejercicio 4 – Creación de un JAR con paquetes

Se tiene la siguiente estructura:

```
src/
 └── escuela/
     └── Alumno.java
```

1. Compilar la clase respetando la estructura de paquetes.
2. Indicar desde qué directorio debe ejecutarse el comando `jar`.
3. Crear un JAR que incluya correctamente el paquete.
4. Verificar el contenido del JAR.
5. Explicar por qué es importante respetar la estructura de directorios.

---

## Ejercicio 5 – Inspección de un JAR

Dado un fichero `app.jar`:

1. Ejecutar el comando para listar su contenido.
2. Identificar:
   - paquetes
   - clases
   - otros recursos (si los hubiera)
3. Explicar cómo se representan los paquetes dentro del JAR.

---

## Ejercicio 6 – Modificación de un JAR

1. Realizar un cambio en una clase existente de un proyecto.
2. Recompilar la clase.
3. Actualizar únicamente ese archivo dentro del JAR.
4. Verificar que el cambio fue aplicado.

Responder:
- ¿Qué opción del comando `jar` se utilizó?
- ¿Qué sucede si el archivo no existía previamente en el JAR?

---

## Ejercicio 7 – Ejecución de un JAR sin manifiesto

1. Ejecutar una clase contenida en un JAR usando `-cp`.
2. Escribir el comando completo.
3. Explicar:
   - por qué se indica el archivo `.jar`
   - por qué se usa el nombre completo de la clase (paquete.clase)

---

## Ejercicio 8 – Fichero de manifiesto

1. Crear un fichero de texto que defina una clase principal.
2. Indicar el nombre correcto del atributo utilizado.
3. Construir un JAR incluyendo dicho manifiesto.
4. Ejecutar el JAR usando una única instrucción.

Responder:
- ¿Qué ventaja aporta el fichero de manifiesto?
- ¿Qué problema resuelve frente al uso de `-cp`?

---

## Ejercicio 9 – Comparación de métodos de ejecución

Completar la siguiente tabla:

| Método | Comando | Ventajas | Desventajas |
|------|--------|----------|-------------|
| Con `-cp` | | | |
| Con `-jar` | | | |

---

## Ejercicio 10 – Caso práctico integrador

Un compañero necesita ejecutar tu programa Java en otro equipo.

1. ¿Qué archivos deberías entregarle?
2. ¿Qué instrucciones mínimas le darías para ejecutarlo?
3. ¿Qué cambios harías si el programa tuviera múltiples dependencias?

---

 **Nota:** No se permite el uso de IDEs para generar el JAR. Todo debe realizarse desde consola.

