# Movilidad-urbana
### El objetivo de este trabajo es identificar en qué ciudades invertir en infraestructura de transporte para aumentar la productividad y el bienestar de la población. (Trabajo de práctica, los datos de este trabajo pueden, o no, ser ficticios).

Antes que nada, en cualquier trabajo se debe de leer, razonar y comprender los datos que se nos estan proporcionando. Ya sea que los tengamos la información en documentación fisica o de manera digital.
<img width="1518" height="182" alt="Captura de pantalla 2026-03-09 185844" src="https://github.com/user-attachments/assets/7a176cdd-6d31-422f-bae2-67ac4c2a8814" />
Pero al relacionarme con los datasets encontre datos erroneos, duplicados, así como información que no rea reelevante para lo que estaba buscando;  ¿qué relación existe entre la movilidad urbana y la productividad económica?
Para esto debía de:

- Crear un dataset único y limpio a partir de dos fuentes diferentes.
- Aplicar limpieza, estandarización y validación de tipos de datos.
- Filtrar y enfocar el análisis en ciudades latinoamericanas...

<img width="1707" height="195" alt="a" src="https://github.com/user-attachments/assets/0116e394-6607-4632-a4db-51ded1503b3e" />
<img width="1685" height="198" alt="b" src="https://github.com/user-attachments/assets/d021a994-9118-47ca-9eb1-9edef8289307" />

Una vez tuve todos los datos de una forma que fueran legibles, sin errores y con unos encabezados que son más entendibles procedi a comenzar a analizar la información, pero yo quiero obtener una vista consolidada del tráfico promedio por ciudad y año, para analizar patrones generales sin depender de datos diarios...
<img width="1715" height="515" alt="image" src="https://github.com/user-attachments/assets/ae9e18e2-01cf-44af-99ea-d582cbbfab57" />
Para analizar visualmente la distribución y la relación entre indicadores de tráfico y economía en 2024, para identificar posibles patrones o tendencias generales entre ambas variables debería de usar seaborn y matplotlib.pyplot para generar los gráficos. Ademas del uso de Boxplot para observar las estadisticas y detectar los valores atipicos...

<img width="877" height="527" alt="image" src="https://github.com/user-attachments/assets/50bb8de3-543d-4733-a598-1ece54d1c5bb" />
<img width="1311" height="602" alt="image" src="https://github.com/user-attachments/assets/ca9d2012-e6d7-4787-95c0-c7996e5abfa3" />

### ¿Qué relación existe entre la movilidad urbana y la PIB percapita?

De acuerdo al trabajo podemos concluir que, al menos en las ciudades Latinoamericanas existe una relacion inversa, no obstante existen ciudades con alto PIB y alta congestión, lo que nos indica que el tamaño poblacional y la estuctura urbana influyen además de el PIB, esto puede actuar como freno estructural del crecimiento si no es gestionado de una buena manera.

El PIB nos permite comparar el desempeño economico entre ciudades, nos ayuda a dectectar donde es necesario priorizar la inversión en infaestructura y el transporte público. Además de que el tiempo adicional entre viajes lo podemos traducir como el impacto en la calidad de vida y la eficiencia laboral.

### Cobertura de datos

Podemos encontrar catorce ciudades como lo son; Bogotá, Lima, Buenos Aires, Sao Paulo, Ciudad de México, Brasilia, Montevideo, etc. Los países incluidos encontramos a Brasil, México, Colombia, Perú, Uruguay, entre otros. Y el año que es de nuesto interes es el 2024.

### Metodología

LaLimpieza de datos se centro en la estandarización de los nombres de columnas, la conversión de fechas para evitar errores, así como la revisión de los datos y la verificacion de nulos, esto para tener una base solida para los puntos posteriores.

En la agregación ciudad/año se agruparon los datos de trafico por ciudad y año, promediamos el índice de congestión anual y de emparejo con el PIB per capita del mismo año (2024).

Para la integración de datos utilizamos la unión INNER para city y year. Asegurando que solo se analicen registros con información completa de trafico y economía. Los histogramas nos apoyan para la distribución, ademas de que se uso el boxplot y scatterplots para la detecciónd e outliers, ademas de detectar la tendencia en la congestion en las ciudades creando elementos para la revisión visual.

### Hallazgos iniciales

Tenemos ciudades con congestion alta pero un PIB relativamente bajo (Lima), otras que tienen PIB alto y con una gran congestion (Ciudad de México), y por ultimo, tenemos ciudades con un mejor balance como lo es Montevideo. Esos resultados nos hablan de ciudades con economia fuerte, pero con una infraestructura ineficiente, mientras que tenemos otras con una econimia fuerte y un posible modelo urbano eficiente pos su baja congestión.

### Recomendaciones

Cuidades como los son Bogotá y Lima tienen una alta congestión con poco nivel de PIB, esto lo podemos resumir en una alta dependencia en el transporte terrestre y una infraestructura limitada, puede ser debido a una carente planeación a un futuro o por la dificultad del terreno.

Uno de los puntos a tratar sería la invesrión en transporte sea; metros autobuses, nias que conecten de una forma más eficiente las ciudades, para que más persones opten por tomar el transporte debido a su accesibilidad y que realicen menos tiempo en sus recorridos diarios. Debemos de analizar la poblacion de estas ciudades y la densidad que tienen, además de tomar en cuenta que lugares serian los más optimos para las estaciones o posibles paradas del circuito, puede haber tambien un aumento por parte del sector privado con incentivos de la movilidad sostenible o tarjetas de pases recargables en transporte.

Esto puede ser aprovechado tanto en un aumento para generar trabajos como lo son la etapa de estructuración y construcción de losos sistemas de transporte, dar trabajo a los que operaran y manejaran la parte vial del sistema, así como una posible disminucion en tiempos, mayor eficiencia en los recorridos y un posible aumento en las contrataciones por los bonos o tarjetas de uso en transporte.
