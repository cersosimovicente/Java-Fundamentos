# Ejercicios – Paquetes en Java

Estos ejercicios están basados en el documento **“Hola Mundo con paquetes en Java”** y están pensados para practicar **organización de código, compilación y ejecución desde consola**, sin usar IDE.

---

## Ejercicio 1 – Hola Mundo en un paquete

### Objetivo
Comprender cómo declarar un paquete y su relación con la estructura de directorios.

### Consigna
1. Crear un proyecto llamado `hola_paquetes`.
2. Dentro del proyecto, crear un paquete llamado `prueba`.
3. Crear la clase `HolaMundo` dentro del paquete `prueba`.
4. El programa debe mostrar por pantalla:

```text
Hola mundo desde paquetes
```

### Requisitos
- Usar consola para compilar y ejecutar.
- No usar IDE.

### Preguntas teóricas
- ¿Qué ocurre si el nombre del paquete no coincide con el nombre del directorio?
- ¿Por qué la línea `package` debe ir al comienzo del archivo?

---

## Ejercicio 2 – Estructura de directorios

### Objetivo
Reconocer la relación entre paquetes y carpetas.

### Consigna
Dada la siguiente declaración de paquete:

```java
package escuela.programacion.java;
```

1. Crear la estructura de directorios correspondiente.
2. Indicar dónde debe ubicarse el archivo `Main.java`.

### Preguntas
- ¿Desde qué directorio se debe ejecutar el comando `javac`?
- ¿Cuál sería el nombre completo de la clase al ejecutarla?

---

## Ejercicio 3 – Compilación manual

### Objetivo
Practicar la compilación de clases dentro de paquetes.

### Consigna
1. Crear el paquete `utilidades`.
2. Crear la clase `Saludador` con un método `main` que muestre:

```text
Hola desde utilidades
```

3. Compilar la clase desde el directorio raíz del proyecto.

### Preguntas
- ¿Dónde se genera el archivo `.class`?
- ¿Qué error aparece si se intenta compilar desde el directorio incorrecto?

---

## Ejercicio 4 – Ejecución con CLASSPATH

### Objetivo
Comprender el uso del `CLASSPATH`.

### Consigna
1. Usar el ejercicio anterior.
2. Ejecutar la clase `Saludador`:
   - Sin definir `CLASSPATH`.
   - Definiendo `CLASSPATH` como variable de entorno.
   - Usando la opción `-cp`.

### Preguntas
- ¿A qué directorio debe apuntar el `CLASSPATH`?
- ¿Por qué no debe apuntar directamente al paquete?

---

## Ejercicio 5 – Paquetes anidados

### Objetivo
Trabajar con subpaquetes.

### Consigna
1. Crear el paquete `empresa.empleados`.
2. Dentro del paquete, crear la clase `EmpleadoApp`.
3. El programa debe mostrar:

```text
Gestión de empleados
```

4. Compilar y ejecutar correctamente desde consola.

### Preguntas
- ¿Cómo se representa este paquete en el sistema de archivos?
- ¿Cuál es el nombre completo de la clase?

---

## Ejercicio 6 – Análisis de errores

### Objetivo
Identificar errores comunes relacionados con paquetes.

### Consigna
Indicar qué error se produce y cómo solucionarlo en cada caso:

1. El paquete declarado es `package prueba;` pero el archivo está en la carpeta `test`.
2. Se ejecuta el comando:

```bash
java HolaMundo
```

cuando la clase pertenece al paquete `prueba`.
3. El `CLASSPATH` apunta al directorio del paquete y no al raíz del proyecto.

---

## Ejercicio 7 – Integrador

### Objetivo
Aplicar todos los conceptos vistos.

### Consigna
Crear un proyecto llamado `sistema_pruebas` con la siguiente estructura:

- `app.inicio` → clase `Main`
- `app.mensajes` → clase `Mensaje`

La clase `Mensaje` debe tener un método estático que retorne un texto.
La clase `Main` debe mostrar ese mensaje por pantalla.

### Requisitos
- Compilar todo desde consola.
- Ejecutar usando el nombre completo de la clase.

### Preguntas finales
- ¿Qué ventajas aportan los paquetes en proyectos grandes?
- ¿Qué problemas aparecen si no se usan paquetes?

---


