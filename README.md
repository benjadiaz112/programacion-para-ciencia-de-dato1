# programacion-para-ciencia-de-dato1
guia 2
Proyecto: Procesamiento de Notas de Estudiantes (Duoc UC)
Este proyecto nace de la necesidad de enfrentar un problema común en el mundo del análisis de datos: la información "sucia". Trabajé con un dataset de registros académicos que presentaba inconsistencias de formato, espacios innecesarios y valores no numéricos, con el objetivo de transformarlo en un reporte de rendimiento limpio y funcional.

El Proceso de Desarrollo
Para cumplir con los objetivos de la Guía 2, estructuré el código de manera modular, enfocándome en la reutilización de funciones y el manejo eficiente de errores en los datos.

1. Diagnóstico y Carga
El primer paso fue importar la librería Pandas y realizar una inspección del archivo notasdeestudiantes.csv. Detecté que las columnas de notas necesitaban una transformación profunda antes de poder realizar cualquier cálculo matemático, debido al uso de comas y etiquetas de texto como "NR".

2. Limpieza de Datos (Función: limpiar_estudiantes)
En lugar de limpiar celda por celda, diseñé una función que automatiza el trabajo pesado:

Normalización de texto: Utilicé .strip() para eliminar espacios invisibles que suelen causar errores al agrupar por carrera o buscar nombres.

Procesamiento con Bucles: Implementé un ciclo for para recorrer las columnas de notas, reemplazando comas por puntos y convirtiendo todo a tipo flotante.

Manejo de Excepciones: Configuré el proceso para que los valores no válidos (como ausencias) se trataran de forma que no interrumpieran el cálculo del promedio final.

3. Análisis de Métricas (Función: resumen_general)
Una vez con los datos limpios, generé un resumen estadístico para obtener una visión global del curso:

Conteo total de alumnos procesados.

Promedio general del grupo.

Identificación de los extremos: la nota más alta y la más baja obtenida.

4. Segmentación Académica (Función: promedio_por_carrera)
Para finalizar, utilicé operaciones de agrupación (groupby) para comparar el rendimiento entre las distintas carreras. Esto permite identificar rápidamente qué programas académicos están teniendo un mejor desempeño o cuáles requieren mayor apoyo.

Tecnologías Utilizadas
Python 3 como lenguaje principal.

Pandas para la estructuración y limpieza de tablas.

NumPy para la lógica de estados y manejo de nulos.

Google Colab como entorno de desarrollo y ejecución.

Conclusión Personal
Este ejercicio me permitió entender que la calidad de cualquier análisis o modelo de IA depende enteramente de la etapa de pre-procesamiento. Dominar herramientas como los bucles para limpieza y las funciones de agregación es clave para cualquier desarrollador que trabaje con datos.
