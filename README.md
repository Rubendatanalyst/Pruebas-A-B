# Selección de hipótesis mediante resultados de pruebas A/B.

__Contexto__

Para impulsar el crecimiento de un negocio digital se tienen a disposición una serie de hipótesis, propuestas innovadoras que podrían convertirse en el catalizador para aumentar los ingresos. Sin embargo, no todas las hipótesis son creadas iguales, y es fundamental priorizar aquellas que tienen mayor probabilidad de éxito.

El objetivo principal es seleccionar cuidadosamente una de estas hipótesis y someterla a una rigurosa prueba A/B. Esta metodología nos permitirá comparar dos versiones de un mismo elemento, con el fin de identificar cuál genera mejores resultados.

Al combinar el rigor científico de los tests A/B con la intuición y conocimiento del negocio, podremos tomar decisiones más inteligentes y optimizar continuamente el negocio.

__Descripción de los datos__

hypotheses_us.csv

•	Hypotheses: breves descripciones de las hipótesis.

•	Reach: alcance del usuario, en una escala del uno a diez.

•	Impact: impacto en los usuarios, en una escala del uno al diez.

•	Confidence: confianza en la hipótesis, en una escala del uno al diez.

•	Effort: los recursos necesarios para probar una hipótesis, en una escala del uno al diez. Cuanto mayor sea el valor Effort, más recursos requiere la prueba.

orders_us.csv
•	transactionId: identificador de pedido.
•	visitorId: identificador del usuario que realizó el pedido.
•	date: fecha del pedido.
•	revenue: ingresos del pedido.
•	group: el grupo del test A/B al que pertenece el usuario.

visits_us.csv
•	date: la fecha.
•	group: grupo de la prueba A/B.
•	visits: el número de visitas en la fecha especificada en el grupo de pruebas A/B especificado.

__Tabla de contenido__

En el archivo '__test_a_b.ipynb__' se encuentra el siguiente desarrollo: 

__Parte I__
- Carga de librerias y archivos.
- Priorización de hipótesis usando el framework ICE y RICE.

__Parte II - Análisis del Test A/B__
- Representación gráfica del ingreso acumulado por grupo.
- Representación gráfica del tamaño de pedido promedio acumulado por grupo.
- Representación gráfica de la diferencia relativa en el tamaño de pedido promedio acumulado para el grupo B en comparación con el grupo A.
- Cálculo de la tasa de conversión de cada grupo como la relación entre los pedidos y el número de visitas de cada día y Representación gráfica de las tasas de conversión diarias de los dos grupos.
- Gráfico de dispersión del número de pedidos por usuario.
- Cálculo de los percentiles 95 y 99 del número de pedidos por usuario.
- Gráfico de dispersión de los precios de los pedidos.
- Cálculo de los percentiles 95 y 99 de los precios de los pedidos.
- Significancia estadística de la diferencia en la conversión entre los grupos utilizando los datos en bruto.
- Significancia estadística de la diferencia en el tamaño promedio de pedido entre los grupos utilizando los datos en bruto.
- Significancia estadística de la diferencia en la conversión entre los grupos utilizando los datos filtrados.
- Significancia estadística de la diferencia en el tamaño promedio de pedido entre los grupos utilizando los datos filtrados.

__Conclusiones__  












