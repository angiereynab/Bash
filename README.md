# Script de Respaldo Seguro de MySQL en BASH

Este script realiza un respaldo seguro de una base de datos MySQL utilizando "mysqldump". Se ha diseñado para ser seguro, fácil de usar y configurable a través de opciones de línea de comandos.

## Características 
    ✓ Evita exponer la contraseña en la línea de comandos o en procesos del sistema.
    ✓ Usa "mysqldump" para generar un respaldo en la ruta especificada.
    ✓ Muestra mensajes claros de inicio, éxito o error.
    ✓ Valida la entrada de usuario para evitar errores comunes.
    ✓ Compatible con MySQL

## Requisitos 

Antes de ejecutar el script, asegurese de cumplir con los siguientes requisitos:

    - Tener acceso a una base de datos MySQL local o remota.
    - Tener instalado "mysqldump" en tu entorno de desarrollo.
    - Tener permisos suficientes para acceder y exportar la base de datos.

Puedes verificar si "mysqldump" esta instalado ejecutando:
    $ mysqldump --version

Sino esta instalado, puedes instalarlo con:
    # Debian/Ubuntu
    $ sudo apt update
    $ sudo apt install mysql-client

    # CentOS/RHEL
    $ sudo yum install mysql

## Instalación
    
    1- Descarga el script y guárdalo en tu sistema.
    2- Concede permisos de ejecución:
        $ chmod +x LARB3-LuzAngelicaReynaBautista.sh
    3- Ejecuta el script con lo parámetros adecuados.

## Uso

Ejecuta el script con las siguientes opciones obligatorias y opcionales.
    $ ./LARB3-LuzAngelicaReynaBautista.sh -u <usuario> -d <base_de_datos> -o <arhivo_de_salida>

◈ Parámetros Obligatorios
    • -u → Usuario de la base de datos.
    • -d → Nombre de la base de datos a respaldar.
    • -o → Ruta y nombre del archivo de respaldo.

◈ Parámetros Opcionales
    • -h → Muestra la ayuda del script.




