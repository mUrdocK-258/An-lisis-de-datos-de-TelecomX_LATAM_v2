# 📊 Análisis de Cancelación de Clientes - TelecomX LATAM

## 📌 Resumen Ejecutivo
Este proyecto busca identificar los principales factores que influyen en la **cancelación de clientes (churn)** dentro de TelecomX LATAM y evaluar modelos de machine learning que permitan predecirla.  
Los hallazgos permiten establecer estrategias de retención basadas en datos.

---

## 🔎 Metodología

1. **Preparación de datos**
   - Eliminación de columnas irrelevantes (ej. `CustomerID`).
   - Transformación de variables categóricas a numéricas mediante *one-hot encoding*.
   - Evaluación de balance de clases → análisis de proporción de clientes que cancelaron vs. permanecieron.
   - Consideración de normalización para modelos basados en distancia.

2. **Modelos probados**
   - **Regresión Logística** (requiere normalización).
   - **K-Nearest Neighbors (KNN)** (requiere normalización).
   - **Random Forest** (no requiere normalización).
   - **Support Vector Machine (SVM)** (requiere normalización).

3. **Evaluación**
   - Accuracy
   - Precisión
   - Recall
   - F1-score
   - Matriz de confusión

---

## 📈 Resultados de los Modelos

| Modelo              | Accuracy | Precisión | Recall | F1-score |
|---------------------|----------|-----------|--------|----------|
| Regresión Logística | **(insertar)** | **(insertar)** | **(insertar)** | **(insertar)** |
| KNN                 | **(insertar)** | **(insertar)** | **(insertar)** | **(insertar)** |
| Random Forest       | **(insertar)** | **(insertar)** | **(insertar)** | **(insertar)** |
| SVM                 | **(insertar)** | **(insertar)** | **(insertar)** | **(insertar)** |

---

## 🔑 Variables más Relevantes

- **Regresión Logística**: coeficientes más altos relacionados con cancelación →  
  *Ejemplo: clientes con contrato mensual, cargos mensuales altos.*

- **KNN**: proximidad entre clientes influida por →  
  *Ejemplo: tiempo de contrato, métodos de pago.*

- **Random Forest**: variables más importantes según importancia de características →  
  *Ejemplo: `Tiempo de Contrato`, `Cargo Mensual`, `Método de Pago`.*

- **SVM**: variables que más impactan en la frontera de decisión →  
  *Ejemplo: `Servicio de Internet`, `Soporte Técnico`, `Streaming TV`.*

---

## 📊 Factores Clave de Cancelación

1. **Clientes con contrato mensual** → Mayor propensión a cancelar frente a contratos anuales.
2. **Altos cargos mensuales** → Clientes sensibles al precio tienden a abandonar.
3. **Falta de servicios complementarios** (ej. seguridad online, soporte técnico) → Relación con mayor churn.
4. **Método de pago automático vs. manual** → Los pagos manuales presentan mayor tasa de cancelación.

---

## 🎯 Estrategias de Retención

- **Incentivar contratos de mayor plazo**: descuentos o beneficios por cambiar de mensual a anual.
- **Segmentación de clientes sensibles al precio**: ofrecer planes más flexibles o personalizados.
- **Mejorar percepción de valor en servicios complementarios**: reforzar marketing de seguridad online, soporte técnico y respaldo en la nube.
- **Fomentar métodos de pago automáticos**: bonificaciones por débito automático o tarjetas.

---

## ✅ Conclusiones

- El **Random Forest** resultó ser el modelo más robusto frente a la variabilidad y sin necesidad de normalización.  
- La **Regresión Logística** mostró buena interpretabilidad al identificar las variables con mayor impacto.  
- El churn se explica principalmente por **precio**, **tipo de contrato** y **servicios adicionales contratados**.  

---

## 📂 Próximos Pasos

- Ajustar hiperparámetros en Random Forest y SVM para mejorar recall.  
- Probar modelos de boosting como **XGBoost** o **LightGBM**.  
- Implementar un sistema de alerta temprana de clientes en riesgo de cancelar.

---

✍️ **Autores**: Equipo de Ciencia de Datos - Especialización en Alura LATAM

