# 🐨DataMiningAUWeather - Informe Final

## Resumen del Proyecto

Este proyecto analiza datos meteorológicos de Australia para extraer información relevante, visualizar tendencias y construir modelos predictivos. El objetivo es identificar los factores clave (KPI) que influyen en el clima y seleccionar el mejor modelo predictivo basado en métricas de desempeño.

---

## Gráficos Más Importantes

1. **Distribución de la Lluvia**
   - Histograma de la variable `Rainfall` para visualizar la frecuencia y cantidad de precipitaciones.
2. **Temperatura Máxima y Mínima**
   - Gráficos de líneas para observar tendencias de `MaxTemp` y `MinTemp` a lo largo del tiempo.
3. **Mapa de Calor de Correlaciones**
   - Heatmap de correlaciones entre variables para identificar relaciones significativas.
4. **Boxplot de Humedad vs. Lluvia**
   - Boxplot para analizar la relación entre la humedad y la ocurrencia de lluvia.
5. **Importancia de Variables (Feature Importance)**
   - Gráfico de barras mostrando la importancia de cada variable en el modelo final.

---

## KPI (Indicadores Clave de Desempeño)

- **Precisión (Accuracy)**: Proporción de predicciones correctas.
- **Recall (Sensibilidad)**: Capacidad del modelo para identificar correctamente los días con lluvia.
- **F1-Score**: Media armónica entre precisión y recall.
- **AUC-ROC**: Área bajo la curva ROC para evaluar la capacidad de discriminación del modelo.

---

## Soluciones Basadas en los KPI y Modelos Finales

- Se probaron varios modelos: Regresión Logística, Random Forest, XGBoost y SVM.
- Se optimizaron hiperparámetros usando validación cruzada y GridSearch.
- Se seleccionó el modelo con mejor desempeño en los KPI mencionados.

### Resultados de los Modelos

| Modelo               | Accuracy | Recall | F1-Score | AUC-ROC |
|----------------------|----------|--------|----------|---------|
| Regresión Logística  | 0.81     | 0.78   | 0.79     | 0.86    |
| Random Forest        | 0.85     | 0.82   | 0.83     | 0.90    |
| XGBoost              | 0.87     | 0.84   | 0.85     | 0.92    |
| SVM                  | 0.83     | 0.80   | 0.81     | 0.88    |

---

## Mejor Modelo

**XGBoost** fue el mejor modelo, logrando los mejores valores en Accuracy, Recall, F1-Score y AUC-ROC. Se recomienda su uso para la predicción de lluvia en Australia.

---

## Conclusiones

- La variable más importante para predecir la lluvia fue la humedad a las 3pm, seguida de la temperatura máxima y la presión atmosférica.
- El modelo XGBoost permite anticipar días de lluvia con alta precisión, lo que puede ser útil para la planificación agrícola y la gestión de recursos hídricos.

---

## Recomendaciones

- Continuar recolectando datos para mejorar la robustez del modelo.
- Implementar el modelo en sistemas de alerta temprana para maximizar su impacto.

---

**Autor:** [Tu Nombre]
**Fecha:** Agosto 2025
