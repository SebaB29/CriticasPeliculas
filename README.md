# 🎬 Críticas de Películas

Trabajo Práctico para la materia **Organización de Datos** (95.58)

---

## 👥 Integrantes

| Nombre                         | GitHub                                   |
|--------------------------------|------------------------------------------|
| Sebastián Brizuela             |                                          |
| Lucía Agha Zadeh Dehdeh        | [Lucia-azd](https://github.com/Lucia-azd)|
| Juan Sebastián Del Río         | [S2JuanS2](https://github.com/S2JuanS2)  |

---

## 📝 Descripción

El objetivo de este trabajo es predecir si una crítica cinematográfica es positiva o negativa utilizando diferentes modelos de clasificación.

### Análisis Exploratorio

Se trabajó con un DataFrame de **50,000 filas** y **3 columnas** que incluye el ID, las críticas (en español) y el sentimiento asociado.

### Preprocesamiento

- Se eliminaron críticas en inglés, quedando **48,183 críticas** en español.
- Se limpiaron caracteres especiales y se transformaron las etiquetas de sentimiento a **1** (positivo) y **0** (negativo).
- Se utilizó **TfidfVectorizer** para ponderar la frecuencia de palabras, eliminando stopwords en español.

### Modelos Utilizados

- **Bayes Naive**
- **Random Forest**
- **XGBoost**
- **Redes Neuronales**
- **Stacking**

---

## 📊 Resultados

| Modelo                 | F1      | Precisión | Recall   | Accuracy | Kaggle   |
|------------------------|---------|-----------|----------|----------|----------|
| Bayes Naive (Mejor)    | 0.86911 | 0.85916   | 0.87930  | 0.86748  | 0.75033  |
| Random Forest          | 0.85331 | 0.83575   | 0.87163  | 0.85005  | 0.72281  |
| XGBoost                | 0.86025 | 0.85134   | 0.86934  | 0.85866  | 0.70478  |
| Red Neuronal           | 0.87670 | 0.87670   | 0.87670  | 0.87670  | 0.74471  |
| Stacking               | 0.86764 | 0.84533   | 0.89116  | 0.86293  | 0.74626  |

---

## 📌 Conclusiones Generales

- El análisis exploratorio fue limitado, ya que solo había una característica a analizar (críticas).
- Las tareas de preprocesamiento resultaron útiles para agilizar y mejorar las predicciones; la eliminación de críticas en inglés tuvo un impacto significativo.
- El mejor modelo resultó ser **Bayes Naive**, el más sencillo y rápido de entrenar, además de ser el que mejor desempeño tuvo en Kaggle.

---

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más información.
