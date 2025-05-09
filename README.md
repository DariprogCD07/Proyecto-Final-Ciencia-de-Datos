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
