# Portfolio Overview - MA2003B Métodos Multivariados

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5** - Tecnológico de Monterrey

---

## 📊 Resumen Ejecutivo

Este portfolio presenta la aplicación práctica de tres técnicas estadísticas multivariadas fundamentales para el análisis de datos empresariales. Cada caso aborda un problema real de negocio, demostrando cómo estas metodologías pueden generar valor y apoyar la toma de decisiones.

---

## 🔗 ¿Cómo se Relacionan los Tres Métodos?

Los tres métodos multivariados presentados en este portfolio comparten un objetivo común: **extraer información significativa de datos complejos con múltiples variables**. Sin embargo, cada uno aborda este objetivo desde una perspectiva diferente:

```
                    DATOS MULTIVARIADOS
                           │
           ┌───────────────┼───────────────┐
           ▼               ▼               ▼
    ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
    │   FACTOR    │ │DISCRIMINANT │ │   CLUSTER   │
    │  ANALYSIS   │ │  ANALYSIS   │ │  ANALYSIS   │
    └─────────────┘ └─────────────┘ └─────────────┘
           │               │               │
           ▼               ▼               ▼
    ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
    │  Reducir    │ │ Clasificar  │ │  Agrupar    │
    │ Dimensiones │ │ en Grupos   │ │ Naturales   │
    │  Latentes   │ │  Conocidos  │ │Descubiertos │
    └─────────────┘ └─────────────┘ └─────────────┘
```

### Conexiones Clave

1. **Factor Analysis → Cluster Analysis:** Los scores factoriales pueden usarse como input para clustering, reduciendo ruido y mejorando la segmentación.

2. **Cluster Analysis → Discriminant Analysis:** Una vez identificados clusters, el análisis discriminante puede crear reglas para clasificar nuevas observaciones.

3. **Factor Analysis → Discriminant Analysis:** Los factores latentes pueden ser mejores predictores que las variables originales, mejorando la clasificación.

---

## ❓ ¿Qué Tipos de Preguntas Responde Cada Método?

| Método | Pregunta Principal | Ejemplos de Aplicación |
|--------|-------------------|------------------------|
| **Factor Analysis** | ¿Cuáles son las dimensiones subyacentes en mis datos? | Identificar factores de satisfacción, construir índices compuestos, reducir cuestionarios |
| **Discriminant Analysis** | ¿Cómo puedo clasificar nuevas observaciones en grupos conocidos? | Scoring crediticio, diagnóstico médico, detección de fraude |
| **Cluster Analysis** | ¿Qué grupos naturales existen en mis datos? | Segmentación de mercado, tipología de clientes, agrupación de productos |

---

## 🧭 ¿Cuándo Usar Cada Técnica?

### Usa Factor Analysis cuando:

- ✅ Tienes muchas variables correlacionadas entre sí
- ✅ Quieres identificar constructos latentes no observables
- ✅ Necesitas reducir dimensionalidad antes de otros análisis
- ✅ Buscas simplificar instrumentos de medición (encuestas)

### Usa Discriminant Analysis cuando:

- ✅ Ya conoces los grupos a los que pertenecen las observaciones
- ✅ Quieres crear una regla para clasificar nuevos casos
- ✅ Necesitas identificar qué variables mejor separan grupos
- ✅ Requieres un modelo interpretable (no caja negra)

### Usa Cluster Analysis cuando:

- ✅ No tienes etiquetas predefinidas de grupos
- ✅ Quieres descubrir estructura natural en los datos
- ✅ Buscas segmentar clientes, productos o entidades
- ✅ Necesitas crear tipologías o taxonomías

---

## 🔍 Casos de Estudio

### Caso 1: Análisis Factorial

**Objetivo:** Reducción de dimensionalidad en datos de satisfacción del cliente

| Aspecto | Detalle |
|---------|---------|
| **Empresa** | TechnoServe Solutions |
| **Dataset** | 3,400 respuestas de 850 clientes |
| **Variables** | 23 ítems de satisfacción (escala Likert) |
| **Método** | Análisis Factorial Exploratorio |
| **Resultado** | Identificación de factores latentes clave |

**Hallazgos principales:**

- Reducción de 23 variables a factores interpretables
- Identificación de dimensiones clave de satisfacción
- Recomendaciones accionables para mejora del servicio

---

### Caso 2: Análisis Discriminante

**Objetivo:** Clasificación de riesgo crediticio

| Aspecto | Detalle |
|---------|---------|
| **Contexto** | Evaluación de préstamos |
| **Dataset** | Datos de solicitudes de crédito |
| **Métodos** | LDA y QDA |
| **Resultado** | Modelo de clasificación de riesgo |

**Hallazgos principales:**

- Identificación de variables predictoras clave
- Comparación de rendimiento entre LDA y QDA
- Evaluación de precisión con matrices de confusión y curvas ROC

---

### Caso 3: Análisis de Clusters

**Objetivo:** Segmentación de clientes retail

| Aspecto | Detalle |
|---------|---------|
| **Empresa** | MegaMart |
| **Dataset** | Datos de comportamiento de clientes |
| **Métodos** | K-means y Clustering Jerárquico |
| **Resultado** | Segmentos de clientes diferenciados |

**Hallazgos principales:**

- Identificación de grupos de clientes con comportamientos similares
- Perfiles detallados de cada segmento
- Estrategias de marketing personalizadas por segmento

---

## 🎯 Competencias Demostradas

1. **Análisis Exploratorio de Datos (EDA)**
   - Visualización efectiva de datos multivariados
   - Detección de patrones y anomalías
   - Preparación y limpieza de datos

2. **Aplicación de Técnicas Multivariadas**
   - Selección apropiada de métodos según el problema
   - Validación de supuestos estadísticos
   - Interpretación correcta de resultados

3. **Comunicación de Resultados**
   - Traducción de hallazgos técnicos a insights de negocio
   - Visualizaciones claras y profesionales
   - Recomendaciones accionables

---

## 🛠️ Herramientas Utilizadas

- **Python** como lenguaje principal
- **Jupyter Notebooks** para análisis interactivo
- **Bibliotecas:** pandas, numpy, scikit-learn, scipy, matplotlib, seaborn, factor-analyzer, pingouin

---

## 📈 Valor Agregado

Cada caso demuestra cómo los métodos multivariados pueden:

- Simplificar datos complejos manteniendo información relevante
- Predecir comportamientos y clasificar observaciones
- Descubrir patrones ocultos en grandes conjuntos de datos
- Apoyar decisiones empresariales basadas en evidencia
