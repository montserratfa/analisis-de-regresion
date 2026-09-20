Análisis de Regresión Lineal: Predicción de Productividad

El notebook `analis_de_regresion.ipynb` ejecuta el flujo completo de análisis estadístico:

1. **Ajuste de Modelos:** Construcción de modelos iniciales, modelos transformados (usando $\log(\text{training})$ y términos cuadráticos para edad y tiempo de traslado) y selección de variables mediante métodos automatizados (*Forward*, *Backward*, *Stepwise*).
2. **Diagnóstico de Supuestos:**
   * **Linealidad:** Verificación de residuales parciales (`crPlots`).
   * **Independencia:** Pruebas de Rachas y Durbin-Watson.
   * **Homocedasticidad:** Pruebas de Bartlett y Levene.
   * **Normalidad:** Pruebas de Shapiro-Wilk, Anderson-Darling, Lilliefors y Cramer-von Mises.
   * **Colinealidad e Influencia:** Evaluación de VIF, Leverage, Distancia de Cook y residuales jackknife.
3. **Predicción:** Generación del archivo final `predicciones.csv` evaluado en el conjunto de prueba (`test_public.csv`).

## Archivos
* `analis_de_regresion.ipynb`: Notebook con el código y análisis.
* `predicciones.csv`: Archivo con los resultados predictivos finales.
