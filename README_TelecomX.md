
# 📊 Proyecto: Predicción de Cancelación de Clientes - TelecomX

Este proyecto aplica técnicas de Machine Learning para predecir la cancelación de clientes (churn) en una empresa de telecomunicaciones ficticia, **TelecomX**.

## 🧠 Objetivo del Proyecto

El objetivo principal es identificar qué clientes tienen más probabilidad de cancelar el servicio y proponer estrategias de retención basadas en los factores detectados.

---

## 🔧 Tecnologías utilizadas

- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)
- Machine Learning: Logistic Regression, Random Forest
- Balanceo con SMOTE
- Evaluación con métricas clásicas (Accuracy, Recall, F1-score)
- Visualización de importancia de variables
- Ajuste de umbral de decisión

---

## 📈 Flujo de trabajo

1. **Preparación de Datos**
   - Limpieza, codificación y escalado de variables
   - División del dataset en entrenamiento (75%) y prueba (25%)
   - Balanceo con SMOTE

2. **Entrenamiento de Modelos**
   - Regresión Logística (requiere normalización)
   - Random Forest (no requiere normalización)

3. **Evaluación**
   - Métricas: Accuracy, Precision, Recall, F1-score
   - Ajuste de umbral para maximizar el Recall

4. **Análisis de Importancia de Variables**
   - Importancia por reducción de impureza (Random Forest)
   - Coeficientes interpretables (Regresión Logística)

5. **Selección del Modelo Champion**
   - Random Forest con umbral ajustado a `0.4` → mejor Recall (`0.679`)
   - Balance entre detección de clientes propensos a cancelar y minimización de falsos negativos

---

## 🏆 Conclusiones

- Las variables más influyentes fueron: tipo de contrato, tiempo como cliente, método de pago, y servicios como soporte técnico y seguridad online.
- Contratos de tipo mes a mes y clientes nuevos presentaron mayor probabilidad de churn.
- Se recomienda incentivar contratos largos y automatización de pagos.

---

## 📂 Archivos incluidos

- `Proyecto_TelecomX_Notebook_Final.ipynb` → Notebook completo del flujo de trabajo
- `Presentacion_Final_TelecomX.pdf` → Presentación ejecutiva con gráficos e insights
- `modelo_champion_rf.pkl`, `umbral_champion.pkl` → Artefactos del modelo

---

## 👤 Autor

Desarrollado como parte de una práctica de ciencia de datos aplicada.
