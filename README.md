# Proyecto Final - Ciencia de Datos 📊  
### Predicción de Incumplimiento de Pago  
**Autor:** Ángel Dario Cortes  
**Fecha de entrega:** 12/05/2025

---

## 📌 Descripción del proyecto

Este proyecto tiene como objetivo predecir si un cliente incurrirá en incumplimiento de pago el siguiente mes, utilizando algoritmos de machine learning aplicados sobre un conjunto de datos financieros y demográficos. Se entrenaron dos modelos supervisados: **regresión logística** y una **red neuronal multicapa (MLPClassifier)**.

---

## 🧠 Algoritmos utilizados

- **Regresión Logística:** modelo base e interpretativo.
- **MLPClassifier (Red Neuronal):** modelo más complejo, capaz de capturar relaciones no lineales.

Se usó **ROC-AUC** como métrica principal de evaluación, dada la naturaleza desbalanceada del problema.

---

## 🔍 Análisis Exploratorio de Datos

Antes de construir los modelos, se realizó un análisis detallado de la distribución de los datos y sus relaciones con la variable objetivo (`default.payment.next.month`).

- **Distribución por género:** El 60.4% de los clientes son mujeres y el 39.6% son hombres. Las tasas de incumplimiento son similares entre ambos grupos.
- **Variables más relevantes:** Las variables más correlacionadas con el incumplimiento son los estados de pago anteriores (`PAY_0`, `PAY_2`, etc.), lo que tiene sentido desde un punto de vista financiero.
- **Correlación entre variables:** Se identificaron grupos de variables altamente correlacionadas, como las facturaciones mensuales (`BILL_AMT1` a `BILL_AMT6`), lo que sugiere que podrían ser simplificadas o reducidas.
- **No se aplicó PCA** porque las correlaciones no justifican una reducción de dimensiones, aunque se sugiere para futuras versiones.

Este análisis ayuda a comprender mejor el dataset y a construir modelos más informados.

---

## 📁 Estructura del repositorio

```bash
/Proyecto-Final-Ciencia-de-Datos
├── README.md
├── /notebook/
│   └── proyecto_prediccion_incumplimiento.ipynb
├── /data/
│   └── data.csv
└── /images/
    └── curva_roc.png (opcional)
