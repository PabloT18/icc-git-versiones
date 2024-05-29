# Practica GIT VERSIONES (TAGs)


## Getting Started

Este proyecto es una práctica de cómo usar Git para control de versiones en un entorno de desarrollo Java. El proyecto incluye ejemplos simples de código Java y demuestra cómo manejar diferentes versiones usando tags anotados en Git.



### Paso 1: Crear un Proyecto Simple de Java

1. **Crear un directorio para tu proyecto:**
   ```bash
   mkdir MiProyectoJava
   cd MiProyectoJava
   ```

2. **Crear un archivo Java simple:**
   Abre un editor de texto y crea un archivo llamado `Main.java`. Escribe el siguiente contenido en el archivo:
   ```java
   public class Main {
       public static void main(String[] args) {
           System.out.println("Hola, mundo!");
       }
   }
   ```

3. **Compilar y ejecutar el programa Java:**
   ```bash
   javac Main.java
   java Main
   ```

Se puede crear el proyecto directamente con VSCode

### Paso 2: Inicializar Git y Crear README

1. **Inicializa el repositorio Git:**
   ```bash
   git init
   ```

2. **Crear un archivo README:**
   Abre otro archivo de texto y nómbralo `README.md`. Agrega información inicial sobre tu proyecto. Por ejemplo:
   ```markdown
   # Mi Proyecto Java
   Este es un proyecto Java simple para demostrar el manejo de versiones con Git.
   ```

3. **Añadir archivos al repositorio y hacer el primer commit:**
   ```bash
   git add Main.java README.md
   git commit -m "Proyecto inicial con README"
   ```

### Paso 3: Subir el Proyecto a un Repositorio Remoto

1. **Crear un repositorio en GitHub** (o cualquier otro servicio de hosting Git). Debes tener una cuenta y luego crear un nuevo repositorio.

2. **Conectar tu repositorio local con el remoto:**
   ```bash
   git remote add origin <URL_DEL_REPOSITORIO_REMOTO>
   ```

3. **Subir tu proyecto al repositorio remoto:**
   ```bash
   git push -u origin master
   ```

### Paso 4: Modificaciones y Manejo de Versiones

1. **Modificar el `README.md` y preparar para la versión v1.0.0:**
   ```markdown
   # Mi Proyecto Java
   Este es un proyecto Java simple para demostrar el manejo de versiones con Git.

   ## Version 1.0.0
   - Versión inicial del proyecto.
   ```

2. **Hacer commit de los cambios:**
   ```bash
   git add README.md
   git commit -m "Preparación para la versión 1.0.0"
   ```

3. **Crear un tag anotado y subirlo:**
   ```bash
   git tag -a v1.0.0 -m "Versión 1.0.0"
   git push origin v1.0.0
   ```

### Paso 5: Repetir para Versiones Adicionales

Repite el paso 4 para las versiones adicionales (por ejemplo, v1.1.0, v1.2.0, v1.3.0), modificando el `README.md` y el código de ser necesario, actualizando el mensaje de commit y el tag según corresponda.

Estos pasos cubren la creación de un proyecto simple, el manejo de control de versiones con Git, y el uso de tags anotados para manejar releases. Es importante familiarizarse con más comandos y opciones de Git para poder adaptarse a diferentes flujos de trabajo y necesidades del proyecto.