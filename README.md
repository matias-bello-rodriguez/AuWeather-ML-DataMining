# 🐨DataMiningAUWeather - Informe Final

## Resumen del Proyecto

Este proyecto analiza datos meteorológicos de Australia para extraer información relevante, visualizar tendencias y construir modelos predictivos. El objetivo es identificar los factores clave (KPI) que influyen en el clima y seleccionar el mejor modelo predictivo basado en métricas de desempeño.

<img width="739" height="577" alt="Captura de pantalla 2025-08-12 215046" src="https://github.com/user-attachments/assets/152e7606-a257-4020-843a-86b5c5ec4c10" />
<img width="938" height="371" alt="Captura de pantalla 2025-08-12 215059" src="https://github.com/user-attachments/assets/59839a01-f599-424b-87b9-06bc5054887c" />


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

## Impacto de Negocio para Aerostáticos Aventura

### 💰 Impacto Financiero:
- Reducción del 40% en cancelaciones de último momento
- Ahorro proyectado: $96M CLP anuales
- ROI del 225% en el primer año

### 📊 KPIs Propuestos:
- Tasa de vuelos recalendarizados: <15%
- Precisión de predicción: >85%
- Anticipación de cancelación: >24 horas

### 🚀 Estrategias de Implementación:
- Sistema de Alerta Temprana automatizado
- Optimización de horarios hacia ventanas matutinas
- Capacitación especializada del personal

### 📈 Beneficios Esperados:
- Aumento del 30% en vuelos completados
- Mejora del 25% en satisfacción del cliente
- Reducción del 50% en quejas por cancelaciones

---

**Autor:** Matías Bello
**Fecha:** Junio 2024
