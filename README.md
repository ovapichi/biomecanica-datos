

# Procesamiento de datos de biomecánica deportiva con python

Aquí dejo los scripts que fui utilizando dentro del laboratorio de biomecánica para procesar los datos exportados de las plataformas de fuerza y dinamómetros de la marca WinLaborat

</header>



## Archivo Celda_individual
Colocando los valores máximos de fuerza de cuadriceps e isquios de cada pierna obtenidos con celdas de cargas, el script aplica formulas y entrega el porcentaje de simetria de MMII para poder saber que grupo muscular entrenar, reducir el riesgo lesiones y potenciar el rendimiento deportivo. 

Los valores de asimetria entre piernas mayores al 10% son leves y mayores al 30% graves.
Los valores de asimetría inter pierna mayores al 6% de fuerza total de la pierna es leve y mayores al 30% es grave.

Mientras más acentuada esté la asimetría mayor es el riesgo de lesiones en los muslos.

## Archivo McGill_individual
Colocando los valores obtenidos con la prueba de fuerza resistencia de zona media de McGill, el script aplica formulas y entrega el porcentaje de simetría de los músculos de la zona media para poder saber que grupo muscular trabajar, reducir el riesgo de lesiones y potenciar el rendimiento deportivo.

## Archivo Plataformas WL Armado Tabla
Es un script para procesar los datos obtenidos desde las plataformas de fuerza Win Laborat, exportados en 3 archivos por cada jugador en formato .dat, transformarlo en un .txt para luego genrear un .csv de la prueba de saltos de Bosco, de los cuales genera un solo archivo con los datos ordenados de los saltos y luego a través de las fórmulas de la bibliografía de Bosco se obtienen  indices de utilización de brazos, de elastididad y de riesgo de lesión, para de esta forma poder orientar el entrenamiento de los deportistas y mejorar su rendimiento deportivo. Puede utilizarse con todo un equipo completo y arma un .csv de cada jugador.

## Archivo Informa Plataformas WL
Desde los archivos .csv generados por el Archivo Plataformas WL Armado Tabla, toma los datos y los procesa a través de fórmulas, y genera un .pdf agrupado con los deportistas según sus resultados lo cual le sirve al preparador físico para agrupar a los deportistas en los ejercicios especificos que tiene que realizar.

## Archivo McGill_y_Celda_Sinforniif
Desde los .csv generados en los archivos anteriores se toman para armar un informe en .pdf para entrenadores con pandas, fue un desafío para mejorar el rendimiento del script para no tener que recurrir a sucesivas iteraciones y condicionantes.
