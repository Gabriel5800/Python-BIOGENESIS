# Python-BIOGENESIS
El trabajo consistia en analizar una base de datos +12.000.000 millones de registros para extraer información del Covid-19 e identificar a cuáles paises de la región deberia la empresa BYOGENESIS extenderse con el fin de brindar mayor cobertura.
A continuación documentaré todo el proceso del trabajo realizado. )
1. Carga, limpieza, filtros y normalización de datos:
Se hace lectura del documento CSV, conteo de nulos filtrado por países seleccionados y por fechas mayores a 2021-01-01, además para la normalización de los datos se usa el promedio de datos para reemplazar los datos nulos. Esto lo guardamos en un nuevo documento limpio para su posterior análisis.

2. Graficación de Matplotlib: Se realizaron diversos gráficos para obtener información general de casos confirmados, nuevos casos, total población, muertes y vacunación por país. Tasa de mortalidad por genero y matriz de correlació. De estos gráficos podemos obtener los siguientes insights:

-Los países más afectados por el covid-19 en aspectos de casos, nuevos casos, muertes son Brasil, Mexico, Colombia y Argentina.
- Colombia es el país con menos tasa de vacunación en toda latinoamerica, superado por país con menor densidad población.
- Existe una correlación positiva moderada de diabetes y tabaquismo (0.74) (0.89), lo que sugiere que áreas con mayor densidad de población podrían tener una mayor prevalencia de diabetes.
- Se nota una correlación negativa moderada en desarrollo humano vs tabaquismo (-0.44), lo que sugiere que áreas con mayor desarrollo humano podrían tener una menor cantidad de fallecidos acumulados.
- Hay una correlación negativa moderada (-0.52) entre tabaquismo vs desarrollo humano, lo que podría indicar que áreas con mayor desarrollo humano tienden a tener una menor prevalencia de tabaquismo.

Importante para futuros análisis investigar el motivo por el cual hay más fallecidos hombres que mujeres ¿tienen mayor exposición en centros medicos?¿Mayor densidad poblacional? Es un interesante rubro a investigar con una base de datos complementaria.

3. Analisis del comportamiento semanal y anual de datos agrupados con Matplotlib y Seaborn: Graficación temporales de casos nuevos por semana a lo largo del año, relación de la temperatura y los casos nuevos generados, distribución de la tasa de mortalidad entre los diferentes paises. A partir de ellos, se encuentran los siguientes insights:

- Brasil y Mexico lideran las tasas de mortalidad por Covid-19, esto se puede atribuir a su densidad poblacional, sin embargo Colombia, un país con menor densidad que Argentina tiene mayor tasa de mortalidad.
- Se encuentra una relación estrecha entre las temperaturas promedio y el aumento de casos de COVID-19 siendo directamente proporcional a medida que una variable aumenta la otra lo hace en similar proporción.

Por último, se recomienda a la empresa BYOGENESIS expandirse a los siguientes países:

1. Brasil: Dada su alta densidad poblacional, mantiene una cifra de casos nuevos confirmados importantes.

2. Mexico: Es el país en promedio con nuevos casos confirmados y tasas de mortalidad altas. se deberá hacer su presencia para evitar un aumento similar al de Brasil.

3. Colombia: Si bien no posee gran cantidad de nuevos casos confirmados, es el país con menos vacunados a nivel de la región, superando en tasa de mortalidad a países con mayor densidad poblacional como Argentina.

