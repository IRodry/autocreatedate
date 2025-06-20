#Generador de Estructura de Carpetas para Fondos

Este script en Python crea automáticamente la estructura de carpetas para organizar archivos por año, trimestres y meses en una carpeta principal llamada "Fondos".

##Estructura que se genera

Cuando ejecutas el script, se te pide un año (por ejemplo, `2025`) y se genera la siguiente estructura:

Fondos/
└── 2025/
├── Q1/
│ ├── 01.Enero
│ ├── 02.Febrero
│ └── 03.Marzo
├── Q2/
│ ├── 04.Abril
│ ├── 05.Mayo
│ └── 06.Junio
├── Q3/
│ ├── 07.Julio
│ ├── 08.Agosto
│ └── 09.Septiembre
└── Q4/
├── 10.Octubre
├── 11.Noviembre
└── 12.Diciembre


##Cómo usar

1. Asegúrate de tener Python instalado.
2. Descarga el script `crear_estructura_fondos.py`.
3. Abre una terminal en la misma carpeta del script.
4. Ejecuta el script con:

```bash
python crear_estructura_fondos.py

Introduce el año cuando se te solicite.

**Verificación de existencia**

Si la carpeta para el año ingresado ya existe, el script te preguntará si deseas continuar.
Solo si respondes yes (en minúsculas), se procederá a crear las subcarpetas que falten.
Cualquier otra respuesta cancelará la operación.

**Personalización**

Puedes cambiar el nombre de la carpeta raíz (Fondos) modificando el valor de ruta_base en el script.
Puedes automatizar el año actual importando datetime y usando:

from datetime import datetime
año_nuevo = str(datetime.now().year)

