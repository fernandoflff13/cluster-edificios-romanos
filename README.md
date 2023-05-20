# Análisis de Cluster Jerárquico de Edificios Romanos

Este proyecto tiene como objetivo realizar un análisis de cluster jerárquico para agrupar edificios romanos en función de sus características. A continuación, se presenta una descripción del proceso realizado y los resultados obtenidos.

## Carga de Datos

Se cargaron los datos de los edificios romanos desde el archivo "data_edificios_ludicos_romanos.xlsx" y se eliminó la columna de identificación. A continuación, se muestra una vista previa de los datos cargados.

## Exploración y Preprocesado de Datos

Se realizó una exploración de los datos y se identificó la presencia de outliers que podrían afectar el rendimiento de los algoritmos de clustering. Para abordar este problema, se aplicó una transformación logarítmica a las columnas numéricas. Además, se normalizaron las variables para que tuvieran una media de 0 y una desviación estándar de 1.

## Distancia Euclídea

Se calculó la matriz de distancias euclídeas entre todas las combinaciones de edificios y se visualizó mediante un gráfico de calor. Esta matriz de distancias es utilizada por los algoritmos de clustering jerárquico para agrupar los edificios en clusters.

## Comparación de Dendrogramas

Se compararon los dendrogramas generados utilizando el método de "Average Linkage" y el método de "Ward Linkage". Se observó que el dendrograma generado con el método de "Ward Linkage" presentaba una estructura más clara y separada, por lo que se seleccionó este método como el más adecuado para el análisis.

## Selección del Número Óptimo de Clusters

Se utilizó el método del codo para determinar el número óptimo de clusters. Se observó que tanto con el método de "Average Linkage" como con el método de "Ward Linkage", el número óptimo de clusters parecía ser alrededor de 3. Se decidió utilizar 3 clusters para el análisis.

## Conclusiones del Mejor Modelo

Se realizó el clustering jerárquico utilizando el método de "Ward Linkage" y se agruparon los edificios romanos en 3 clusters. Se realizó una visualización de los puntos en el espacio y se mostraron las características más significativas de cada cluster. Se observó que los edificios se agrupaban principalmente en función de su tipo y dimensiones.

## Visualización de Dendrogramas

Se presentaron diferentes visualizaciones de los dendrogramas generados. Se destacó la estructura de los clusters y se utilizó la coloración para distinguir los diferentes grupos.

## Referencias

1. Análisis jerárquico de cluster: https://rquer.netlify.app/clustering/
2. Transformación logarítmica: https://rpubs.com/marvinlemos/log-transformation
3. Número óptimo de clusters: http://www.sthda.com/english/articles/29-cluster-validation-essentials/96-determiningthe-optimal-number-of-clusters-3-must-know-methods/