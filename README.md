# Proyecto2-SegundaParte
Segunda parte del segundo proyecto de Python Avanzado

# Regresión Lineal Múltiple – Proyecto 2

### Tecnicatura Universitaria en Tecnologías de Programación  
**Materia:** Programación Python Avanzada  
**Integrantes:** Amezaga Estefanía, Figueroa Cynthia, Pizarro Sol.

## Conclusiones – Segunda Parte: Regresión Lineal Múltiple

El análisis realizado sobre el dataset de autos usados permitió construir y evaluar un modelo de regresión lineal múltiple con el objetivo de predecir el precio a partir de distintas características del vehículo. La exploración inicial mostró que los datos no presentaban valores faltantes y que existía una amplia variabilidad en kilómetros recorridos, edad del auto y precio, lo que hacía necesario un modelo capaz de capturar relaciones lineales entre múltiples variables.

La matriz de correlación indicó que edad_auto y km_recorridos tienen una correlación negativa con el precio, lo que coincide con el comportamiento habitual del mercado: autos más viejos o con mayor uso tienden a valer menos. La variable tipo, pese a ser binaria, mostró una correlación positiva moderada y terminó siendo la que mayor peso tuvo en el modelo. Por el contrario, edad_vendedor y reparaciones evidenciaron menor relevancia estadística.

Tras dividir los datos en entrenamiento y prueba, se entrenó el modelo de regresión lineal. Las métricas obtenidas fueron consistentes en ambos conjuntos, con un R² cercano al 60%, lo que indica que el modelo logra explicar una parte importante de la variabilidad del precio sin mostrar señales de overfitting. Los valores de MAE y RMSE se mantuvieron en rangos similares entre Train y Test, demostrando que el modelo generaliza correctamente.

El análisis de los coeficientes permitió identificar que la variable tipo fue la más influyente en el precio, seguida por factores relacionados con desgaste, como edad_auto, km_recorridos y reparaciones, los cuales generaron un impacto negativo. Esto confirma la lógica del mercado: el tipo de vehículo define un valor base, mientras que el uso y la antigüedad reducen ese valor.

En conjunto, el modelo desarrollado resulta estable, interpretativo y útil para estimar el precio de autos usados empleando un conjunto reducido de variables. Aunque no captura la totalidad de la variabilidad del precio, brinda una aproximación razonable y consistente, adecuada para fines exploratorios o como base para modelos más complejos.
