# Data Automation Template

Este proyecto automatiza la limpieza, análisis y envío de reportes utilizando datos de móviles del año 2025.

## Estructura

- `data/`: Contiene los archivos de datos.
- `reports/`: Almacena los reportes generados.
- `src/`: Scripts de procesamiento y automatización.
- `.env`: Variables de entorno para configuración de correo.
- `requirements.txt`: Dependencias del proyecto.

## Uso

1. Instala las dependencias:
   
!pip install -r requirements.txt

3. Configura tus credenciales en el archivo `.env`.

4. Ejecuta el script maestro:
python src/run_all.py

El script se ejecutará diariamente a las 08:00 AM, generando y enviando el reporte automáticamente.


data-automation-template/
│
├── data/
│   └── raw_data.csv           # Archivo de datos de entrada
│
├── reports/
│   └── report.html            # Reporte generado automáticamente
│
├── src/
│   ├── clean_data.py          # Limpieza de datos
│   ├── analyze_data.py        # Análisis y visualización
│   ├── send_email.py          # Envío del reporte por correo
│   └── run_all.py             # Script maestro que ejecuta todo
│
├── .env                       # Variables de entorno (correo, clave, etc.)
├── requirements.txt           # Librerías necesarias
├── README.md                  # Instrucciones del proyecto
└── .gitignore                 # Ignorar datos sensibles


##########################
🧪 ¿Qué hace?
##########################
	•	Limpia un CSV que pongas en /data/
	•	Genera visualizaciones automáticas (gráficos con Plotly o Matplotlib)
	•	Crea un HTML con el análisis
	•	Lo envía por correo automáticamente
	•	Puedes programarlo con schedule para que corra cada mañana

##########################
🧪 Descripción del Proyecto
##########################
Este proyecto automatiza las siguientes tareas:
	1.	Limpieza de datos: Procesa el conjunto de datos de móviles 2025, eliminando valores nulos y estandarizando nombres de columnas.
	2.	Análisis y visualización: Genera gráficos interactivos para visualizar tendencias en precios y especificaciones de los dispositivos.
	3.	Generación de reporte: Crea un archivo HTML con los resultados del análisis.
	4.	Envío por correo: Envía automáticamente el reporte generado a una dirección de correo especificada.
	5.	Automatización diaria: Programa la ejecución diaria del script maestro para mantener los reportes actualizados.
