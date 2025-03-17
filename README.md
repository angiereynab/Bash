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

## Ejemplos de Ejecución

### 1. Respaldo básico con archivo de salida especificado

    $ ./LARB3-LuzAngelicaReynaBautista.sh -u root -d mysql -o /tmp/LARB3.sql

📌 Salida esperada:
    
    Introduce la contraseña para el usuario 'root': 
    Iniciando respaldo...
    Usuario: root
    Base de datos: mysql
    Archivo de salida: /tmp/LARB3.sql
    Backup exitoso: /tmp/LARB3.sql

### 2. Mostrar la ayuda del script

    $ ./LARB3-LuzAngelicaReynaBautista.sh -h

📌 Salida esperada:
    
    COMANDO ESPERADO:
    $ bash LARB3-LuzAngelicaReynaBautista.sh -u <USUARIO> -d <BASE_DE_DATOS> -o <RUTA_ARCHIVO_SALIDA>

    Opciones:
    - u Usuario de la base de datos (OBLIGATORIO)
    - d Nombre de la base de datos (OBLIGATORIO)
    - o Ruta y nombre del archivo de respaldo (OBLIGATORIO)
    - h Mostrar esta ayuda
    
    Ejemplo: 
    $ bash LARB3-LuzAngelicaReynaBautista.sh -u root -d mysql -o /tmp/LARB3.sql

    Nota:
    Si deseas ejecutar el comando con './LARB3-LuzAngelicaReynaBautista.sh' en lugar de 'bash LARB3-LuzAneglicaReynaBautista.sh" necesitas permisos de ejecución.
    
    Comando para permisos:
    $ chmod +x LARB3-LuzAngelicaReynaBautista.sh
