# Comparación de Metodologías

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5** - Tecnológico de Monterrey

---

## 📊 Resumen Comparativo

| Aspecto | Análisis Factorial | Análisis Discriminante | Análisis de Clusters |
|---------|-------------------|----------------------|---------------------|
| **Objetivo** | Reducir dimensionalidad | Clasificar observaciones | Agrupar observaciones |
| **Tipo** | No supervisado | Supervisado | No supervisado |
| **Variable dependiente** | No | Sí (categórica) | No |
| **Output** | Factores latentes | Regla de clasificación | Grupos/segmentos |
| **Supuestos clave** | Correlación entre variables | Normalidad, homogeneidad | Distancia significativa |

---

## 🔍 Análisis Detallado

### Análisis Factorial

**¿Cuándo usarlo?**
- Cuando hay muchas variables correlacionadas
- Para identificar estructuras subyacentes en los datos
- Para reducir dimensionalidad antes de otros análisis
- Para crear índices o scores compuestos

**Supuestos principales:**
- Correlación suficiente entre variables (KMO > 0.6)
- Significancia de correlaciones (Test de Bartlett)
- Tamaño de muestra adecuado (≥5 observaciones por variable)

**Métricas de evaluación:**
- KMO (Kaiser-Meyer-Olkin)
- Varianza explicada
- Comunalidades
- Cargas factoriales

**Ventajas:**
- Simplifica datos complejos
- Revela patrones ocultos
- Reduce ruido en los datos

**Limitaciones:**
- Subjetividad en número de factores
- Requiere interpretación del analista
- Sensible a la selección de variables

---

### Análisis Discriminante

**¿Cuándo usarlo?**
- Para clasificar nuevas observaciones en grupos conocidos
- Cuando la variable dependiente es categórica
- Para identificar variables que mejor separan grupos
- Cuando se requiere interpretabilidad del modelo

**Supuestos principales:**
- Normalidad multivariada (especialmente para QDA)
- Homogeneidad de covarianzas (para LDA)
- Independencia de observaciones

**Métricas de evaluación:**
- Accuracy
- Precisión, Recall, F1-Score
- Curva ROC y AUC
- Matriz de confusión

**LDA vs QDA:**
| Aspecto | LDA | QDA |
|---------|-----|-----|
| Frontera de decisión | Lineal | Cuadrática |
| Supuesto de covarianza | Iguales entre grupos | Pueden ser diferentes |
| Complejidad | Menor | Mayor |
| Riesgo de overfitting | Menor | Mayor |

**Ventajas:**
- Modelo interpretable
- Funciona bien con pocos datos
- Identifica importancia de variables

**Limitaciones:**
- Sensible a violaciones de supuestos
- Limitado a fronteras lineales/cuadráticas
- Requiere variable dependiente definida

---

### Análisis de Clusters

**¿Cuándo usarlo?**
- Para descubrir grupos naturales en los datos
- Cuando no hay etiquetas predefinidas
- Para segmentación de mercado
- Para identificar patrones de comportamiento

**Métodos principales:**

| Método | Características |
|--------|----------------|
| **K-means** | Rápido, escalable, requiere k predefinido |
| **Jerárquico** | Dendrograma visual, no requiere k inicial |
| **DBSCAN** | Detecta formas arbitrarias, maneja outliers |

**Métricas de evaluación:**
- Coeficiente de Silueta
- Índice de Davies-Bouldin
- Inercia (within-cluster sum of squares)
- Método del codo

**Ventajas:**
- No requiere etiquetas previas
- Descubre estructura en los datos
- Flexible en aplicaciones

**Limitaciones:**
- Difícil determinar número óptimo de clusters
- Sensible a outliers y escala
- Resultados pueden variar con inicialización

---

## 🔗 Conexiones entre Métodos

```
┌─────────────────┐
│ Datos Originales │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Análisis        │  ← Reduce dimensionalidad
│ Factorial       │  ← Crea scores factoriales
└────────┬────────┘
         │
    ┌────┴────┐
    ▼         ▼
┌───────┐  ┌───────────┐
│Cluster│  │Discriminante│
│Analysis│  │Analysis    │
└───────┘  └───────────┘
    │            │
    ▼            ▼
Segmentos   Clasificación
sin etiquetar  supervisada
```

**Uso combinado:**
1. Usar **Análisis Factorial** para reducir variables
2. Aplicar **Clustering** sobre los factores para segmentar
3. Usar **Discriminante** para clasificar nuevos casos en segmentos

---

## 📋 Guía de Selección

```
¿Tienes variable dependiente categórica?
    │
    ├── SÍ → ¿Quieres clasificar nuevas observaciones?
    │         │
    │         ├── SÍ → ANÁLISIS DISCRIMINANTE
    │         │
    │         └── NO → ¿Muchas variables correlacionadas?
    │                   │
    │                   └── SÍ → ANÁLISIS FACTORIAL
    │
    └── NO → ¿Quieres encontrar grupos naturales?
              │
              ├── SÍ → ANÁLISIS DE CLUSTERS
              │
              └── NO → ¿Reducir dimensionalidad?
                        │
                        └── SÍ → ANÁLISIS FACTORIAL
```

---

## 📚 Referencias Clave

- Hair, J. F., et al. (2019). *Multivariate Data Analysis*
- James, G., et al. (2021). *An Introduction to Statistical Learning*
- Scikit-learn Documentation: https://scikit-learn.org/
