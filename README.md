# Practica GIT VERSIONES (TAGs)


## Getting Started

Este proyecto es una práctica de cómo usar Git para control de versiones en un entorno de desarrollo Java. El proyecto incluye ejemplos simples de código Java y demuestra cómo manejar diferentes versiones usando tags anotados en Git.

## Requisitos
- Java JDK 11 o superior
- Git 2.20 o superior


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
   git tag -a v1.0.1 -m "App v1.0.1"
   git push origin v1.0.1
   ```

### Paso 5: Repetir para Versiones Adicionales

Recuerada que adicional a la descripción especifica se debera modificar el `README.md` adicionando la informacion de la version 

   ```markdown
   # Mi Proyecto Java
   Este es un proyecto Java simple para demostrar el manejo de versiones con Git.

   ## Version 1.0.0
   - Versión inicial del proyecto.

   ## Version X.X.X
   - [Descripcion de la version ]
   ```

#### Versión v1.0.2: Estructura MVC y Clase de Modelo

1. **Descripción:**
   - Crea la estructura de carpetas MVC (Model-View-Controller).
   - Añade una clase de tipo objeto (como `Persona`) en la carpeta de modelos con los métodos y atributos necesarios. No se permite Objetos `Persona`, `Vehiculo o Carro`

2. **Comandos de Git:**
   ```bash
   git add .
   git commit -m "Agregada estructura MVC y clase modelo Object"
   git tag -a v1.0.2 -m "Versión 1.0.2: Estructura MVC y modelo Object implementados"
   git push 
   git push origin --tags
   ```


#### Versión v1.0.3: Implementación de Arreglo de Objetos

1. **Descripción:**
   - Modifica la clase principal para incluir un arreglo de objetos `Object`, inicializando varios objetos con diferentes valores.

2. **Comandos de Git:**
   ```bash
   git add Main.java
   git commit -m "[Mensaje adecuado]"
   git tag -a v1.0.3 -m "Mensaje adecuado"
   git push origin --tags
   ```



#### Versión v1.0.4: Funcionalidad en Controladores y Vistas
Realizar dos commits antes de realizar el TAG
1. **Descripción:**
   - Crea una clase `ObjectController` con un método de búsqueda secuencial el cual reciba el arreglo, y el valor a buscar, es decir por algun valor de uno de los atributos del objeto.

2. **Comandos de Git:**
   ```bash
   git add .
   git commit -m "[Mensaje adecuado]"
   git push
   ```

3. **Descripción:**
   - Añade una clase `ObjectView` para manejar la visualización de objetos `Object`.


4. **Comandos de Git:**
   ```bash 
   git add .
   git commit -m "[Mensaje adecuado]"
   git tag -a v1.0.4 -m "[Mensaje adecuado]"
   git push
   git push --tags
   ```

#### Versión v2.0.0: Integración y Pruebas Finales

1. **Descripción:**
   - Modifica la clase `Main` para integrar y probar las llamadas a los métodos de las clases `ObjectController` y `ObjectView`.
   - Verifica que todo el sistema funcione correctamente.

2. **Comandos de Git:**
   ```bash
   git add .
   git commit -m "[Mensaje adecuado]"
   git tag -a v2.0.0 -m "[Mensaje adecuado]"
   git push
   git push origin v2.0.0
   ```

## Contribuir

Para contribuir a este proyecto, por favor crea un fork y envía un pull request, o simplemente abre un issue con tus comentarios y sugerencias.

## Autores

- [PABLO TORRES] - Desarrollo inicial