# programacion-para-ciencia-de-dato1
guia 3


🏅 Proyecto de Limpieza y Análisis de Datos Deportivos (2281 Registros)
Este proyecto aplica técnicas avanzadas de Data Cleaning 🧹 y Data Analysis 📊 sobre un dataset extenso de más de 2000 registros de deportistas. El objetivo principal fue automatizar el procesamiento de una base de datos de gran volumen para obtener estadísticas confiables y precisas. 🎯

📁 Estructura del Proyecto
El proyecto está organizado de forma modular para facilitar la escalabilidad y el orden: 🏗️

📂 data/: Contiene el dataset original (deportistas.csv). 📄

📂 src/: Módulos de Python con la lógica del negocio. 🧠

🐍 limpieza.py: Algoritmos de limpieza y tratamiento de outliers.

🐍 analisis.py: Funciones de agregación y cálculo estadístico.

📂 notebooks/: Cuaderno analisis.ipynb que actúa como orquestador del proceso. 📓

📂 outputs/: Resultados finales listos para presentación. 📤

🛠️ Procesos Realizados para el Big Data
1. Limpieza de Datos Masiva 🧹
Dado el volumen de 2281 datos, se implementaron procesos automáticos para:

Normalización de columnas: 📋 Transformación de encabezados para asegurar la compatibilidad en las consultas.

Imputación de Nulos: 🧮 Se detectaron y rellenaron valores faltantes en las métricas de rendimiento y salud utilizando promedios calculados.

Deduplicación: 🚫 Identificación y eliminación de registros redundantes en la base de datos.

Tratamiento de Errores de Formato: 🔄 Conversión masiva de datos tipo string (con comas) a float (con puntos) para permitir operaciones aritméticas.

Filtrado de Outliers (IQR): 📉 Se aplicó el método del Rango Intercuartílico para descartar datos ruidosos en peso y entrenamiento, garantizando promedios reales.

2. Análisis de Rendimiento 📈
Agrupación Estadística: 🔢 Se procesaron las filas para calcular el rendimiento promedio por cada disciplina deportiva.

Detección de Atletas de Elite: ⭐ Filtrado automático de los deportistas con puntajes superiores a la media.

📊 Resultados Exportados
El flujo de trabajo genera dos archivos clave en la carpeta outputs/: 🏁

✨ deportistas_limpios.csv: La base de datos depurada, sin nulos y con formatos corregidos.

📊 analisis_por_deporte.csv: Tabla comparativa con los promedios de rendimiento de todas las categorías analizadas.

💻 Tecnologías Utilizadas
Python 3.x 🐍

Pandas 🐼 (Procesamiento de grandes volúmenes de datos)

NumPy 🔢

Jupyter Notebooks 📓

👤 Autor: Benjamin Diaz

📅 Fecha: Marzo 2026

🌟 Estado: Completado
