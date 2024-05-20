![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Laboratorio | Limpieza de datos básicos y EDA

Para esta práctica de laboratorio, usaremos el conjunto de datos del Caso de Negocio de Análisis de Clientes. Este conjunto de datos se puede encontrar en la carpeta `files_for_lab`.

## Contexto

Una compañía de seguros de automóviles ha recopilado algunos datos sobre sus clientes, incluidos sus _demográficos_, _educación_, _empleo_, _detalles de la póliza_, _información del vehículo_ en la que se encuentra la póliza de seguro y los _montos de las reclamaciones_. Ayudará a la alta dirección con algunas preguntas comerciales que deberían ayudarles a comprender mejor a sus clientes, mejorar sus servicios y mejorar la rentabilidad.

**Algunos objetivos comerciales para el estudio de caso podrían ser**:

- Retener clientes,
- Analizar datos relevantes del cliente,
- Desarrollar programas enfocados en retención de clientes.

Con base en el análisis, tome acciones específicas para aumentar la respuesta, la retención y el crecimiento rentables de los clientes.

### Instrucciones

1. Importe las bibliotecas necesarias.
2. Cargue `we_fn_use_c_marketing_customer_value_analysis.csv` en la variable `customer_df` (es decir, `customer_df = pd.readcsv("")`)
3. Primero, observe sus características principales (`cabeza`, `forma`, `información`).
4. Cambie el nombre de las columnas para que sigan el PE8 (caso de serpiente).
5. Corrija los tipos de datos de cualquier otra columna/columnas según lo considere necesario. Tenga en cuenta que a veces hay algunas características que quizás desee utilizar como categóricas, pero Python las lee como numéricas (y viceversa). Por ejemplo, si hay una columna con valores de año como 2020, 2021, 2022, etc., Python puede leer esta columna como numérica, pero usted querrá usar esa columna como datos categóricos. **Sugerencia**: Una cosa que puedes intentar es cambiar la columna de fecha al formato de fecha y hora.
6. Traza una matriz de correlación y comenta lo que observas.
7. Traza cada variable continua. Comenta lo que puedes ver en las tramas.
8. Haga lo mismo con las variables categóricas (¡tenga cuidado, es posible que deba cambiar el tipo de gráfico a uno más adecuado para datos continuos!). Comenta lo que puedes ver en las tramas.
También debes eliminar la columna `customer_id` antes de poder intentar usar un bucle for en todas las columnas categóricas. Analice por qué es necesario eliminar la columna `customer_id`. **Sugerencia**: Utilice gráficos de barras para trazar datos categóricos, con cada categoría única en la columna en el eje x y una medida apropiada en el eje y.
9. Busque valores atípicos en las variables continuas. (**Pista**: ¡Hay una buena trama para hacer eso!). En caso de que encuentres valores atípicos, comenta qué harás con ellos.
10. Verifique todas las columnas para ver los valores *NaN*. Decide qué necesitarás hacer (si es que necesitas hacer algo) con ellos.