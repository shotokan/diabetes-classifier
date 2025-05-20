# Proyecto de Análisis y Clasificación de Diabetes

Este proyecto tiene como objetivo explorar un conjunto de datos de salud con el fin de identificar patrones asociados al desarrollo de diabetes, así como entrenar modelos de clasificación para predecir su presencia.

---

## 📌 Hipótesis planteadas

1. Las personas con obesidad (alto BMI) tienen mayor probabilidad de diabetes.
2. No hay diferencia en la proporción de personas con diabetes entre quienes consumen fruta y quienes no.
3. El consumo diario de fruta se asocia a una menor prevalencia de diabetes.
4. La inactividad física está relacionada con mayor prevalencia de diabetes.
5. Las personas con menor nivel educativo tienen mayor probabilidad de sufrir diabetes.
6. Las personas con colesterol alto o presión alta tienen más riesgo de desarrollar diabetes.
7. El consumo diario de frutas y verduras se relaciona con menor presencia de diabetes.
8. El acceso a atención médica reduce la probabilidad de complicaciones como ataque cardíaco o stroke.
9. La diabetes es más prevalente en adultos mayores.

---

## ❓ Preguntas de investigación

- ¿Cuál es la proporción de personas con diabetes (clases 0, 1, 2)?
- ¿Cuál es el promedio de BMI por grupo de diabetes?
- ¿Cómo varía la prevalencia de diabetes por edad?
- ¿Existe diferencia en diabetes entre hombres y mujeres?
- ¿El nivel de ingreso o educación afecta la presencia de diabetes?
- ¿Hay relación entre salud general percibida y diabetes?
- ¿Qué factores (como fumar, alcohol, presión, colesterol) aparecen con más frecuencia en personas con diabetes?

---

## 🧪 Fases del proyecto

### 1. Análisis exploratorio de datos (EDA)

- Visualización de la distribución de diabetes según variables relevantes.
- Identificación de valores faltantes.
- Pruebas estadísticas (como Chi-cuadrado) para validar relaciones.

### 2. Selección de características

- Se utilizó `SelectKBest` con la prueba `chi2` para identificar las variables más predictivas.
- Se probaron diferentes valores de `k` (como 8, 10, 12) para optimizar rendimiento.

### 3. Modelos entrenados

- `RandomForestClassifier` con y sin `class_weight='balanced'`
- `LogisticRegression` con y sin balanceo
- Evaluación con métricas: accuracy, precision, recall, f1-score y matriz de confusión.
