# Predicción de Fuga de Clientes — H&M Fashion

![Banner](https://www.vtiger.com/blog/wp-content/uploads/2021/01/8-Possibilities-of-CRM-that-will-Change-the-Way-1-e1609848202482-1.png)

## Autores
Santiago Suarez Magon · Esteban Aicardy Pacheco

## Objetivo
Predecir qué clientes tienen baja probabilidad de retorno usando su historial de compras, perfil RFM y comportamiento en la plataforma. Combina modelos supervisados de clasificación con análisis no supervisado de segmentación.

## Dataset
**H&M Personalized Fashion Recommendations**
Kaggle: https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations

Transacciones reales de H&M con historial de compras por cliente, catálogo de artículos y metadatos de producto. Se construyó un dataset RFM derivado con variables de recencia, frecuencia, gasto, edad, canal y estatus de membresía.

## Contenido del colab

**Sección 1 — Setup y datos**
Reconstrucción del dataset de modelado, ingeniería de variables RFM y codificación de variables categóricas.

**Sección 2 — Modelos supervisados**
Entrenamiento y comparativa de Random Forest, SVM y modelos previos (Regresión Logística, XGBoost). Métricas: accuracy, precision, recall, F1.

**Sección 3 — Análisis no supervisado**
- PCA para reducción de dimensiones y visualización de varianza explicada
- KMeans con selección de K por Elbow + Silhouette
- t-SNE para visualización 2D de clusters
- DBSCAN con estimación automática de eps (percentil 90 k-distancia)
- Clustering Jerárquico Ward con dendrograma
- Comparativa de algoritmos y perfil de segmentos vs churn

**Sección 4 — Conclusiones**
Vinculación entre segmentos no supervisados y predicción de churn supervisado.

## Modelos y técnicas
`Random Forest` `SVM` `KMeans` `DBSCAN` `Clustering Jerárquico` `PCA` `t-SNE` `Churn Prediction` `Feature Engineering` `RFM`

## Métricas usadas
| Métrica | Sección | Para qué sirve |
|---|---|---|
| Silhouette | Clustering | Qué tan separados están los clusters (−1 a +1) |
| Inercia / Elbow | KMeans | Elegir el K óptimo |
| Accuracy / F1 | Supervisado | Rendimiento del clasificador |

## Enlaces
- 🎥 **Video IA**: [Ver en Drive](https://drive.google.com/file/d/1EMMJbneSSfFj5awoFUP5GBSeMjDA7Sz4/view?usp=sharing)
- 📂 **Código (Colab)**: [Abrir notebook](https://colab.research.google.com/drive/1e5QQs63sUL82r9gU0xu7wJj7YmX0TrKp?usp=sharing)
- 🗂️ **Repositorio**: [GitHub](https://github.com/xteban23/prediccion-fuga-clientes)
- 🎨 **Presentación**: [Ver en Canva](https://canva.link/qmsm3ad6aqtm3bh)
