# Aprendizaje Autónomo 1 - Principios de Sistemas de Software Distribuido

**Estudiante:** Darwin Homero Palacios Contreras  
**Cedula:** 1750966929  
**Universidad:** Universidad Internacional del Ecuador (UIDE)  

## Descripción del Proyecto
Este repositorio contiene los archivos, ejemplos y configuraciones desarrollados para el proyecto de Aprendizaje Autónomo 1. El objetivo principal es demostrar la comprensión práctica de los sistemas distribuidos mediante el uso de herramientas de línea de comandos, gestores de construcción de proyectos (Gradle) y comunicación en red mediante Sockets (Cliente-Servidor).

El proyecto fue desarrollado utilizando un entorno heterogéneo con dos nodos (máquinas físicas):
*   **Nodo Cliente:** Laptop con Ubuntu Linux.
*   **Nodo Servidor:** PC de escritorio con Windows.

## Estructura y Fases del Proyecto

### Parte 1: Entorno de Línea de Comandos (Linux)
Uso de la terminal de Ubuntu para la administración y procesamiento de datos simulando un entorno de servidor sin interfaz gráfica.
*   Creación de directorios y manipulación de permisos (`chmod`, `mv`, `cp`).
*   Uso de operadores de redirección (`>`, `>>`, `|`).
*   Procesamiento de archivos CSV (`marks.csv`) utilizando comandos de filtrado como `awk`, `cut`, `grep`, `sort`, `head` y `tail`.

### Parte 2: Control de Versiones y Construcción (Gradle)
Implementación de herramientas estándar de la industria para el desarrollo colaborativo y la construcción de software en Java.
*   Configuración de control de versiones local con **Git** y conexión a este repositorio remoto en **GitHub**.
*   Configuración del gestor de dependencias **Gradle**.
*   Ejecución del código `SimpleGrabHttpURL` modificando el archivo `build.gradle` para realizar una petición HTTP a `www.google.com` y descargar su estructura HTML.

### Parte 3: Comunicación Cliente-Servidor (Sockets en Java)
Prueba de comunicación distribuida en una red de área local (LAN) utilizando el código base del repositorio `ser321examples` del profesor.
*   **Servidor:** Ejecución de `SockServer.java` en el entorno Windows, escuchando en el puerto designado.
*   **Cliente:** Ejecución de `SockClient.java` desde el entorno Ubuntu Linux, apuntando a la dirección IP local del servidor (`10.42.0.50`).
*   **Resultado:** Envío exitoso de cadenas de texto (Strings) y enteros (Integers) por la red, validado mediante la recepción del mensaje `"Got it!"` por parte del servidor.

## Requisitos del Entorno
Para ejecutar los códigos de este repositorio se requiere:
*   Java Development Kit (JDK 17 o superior).
*   Gradle (versión 8+ recomendada).
*   Git.
