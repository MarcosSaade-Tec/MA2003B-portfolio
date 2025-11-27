# Caso 03 — Análisis de Clusters

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5**

---

## 🏢 Contexto del Negocio

**Cliente:** MegaMart - Cadena de retail

**Problema:** La empresa tiene una base de clientes diversa pero trata a todos de manera homogénea en sus estrategias de marketing. Necesita identificar segmentos naturales para personalizar ofertas y comunicaciones.

**Importancia estratégica:** La segmentación efectiva de clientes permite optimizar campañas de marketing, mejorar la experiencia del cliente y aumentar el valor de vida del cliente (CLV) mediante ofertas personalizadas.

---

## 🔬 Metodología

### Métodos Aplicados

- **K-means Clustering** - Partición en k grupos minimizando varianza intra-cluster
- **Clustering Jerárquico** - Agrupación aglomerativa con visualización de dendrograma

### Justificación

- No existe variable de segmentación predefinida (aprendizaje no supervisado)
- Objetivo de descubrir grupos naturales en comportamiento de clientes
- Uso de múltiples métodos para validar robustez de segmentos

### Herramientas y Librerías

- Python 3.x
- `scikit-learn` - K-means y métricas de clustering
- `scipy` - Clustering jerárquico y dendrogramas
- `pandas`, `numpy` - Manipulación de datos
- `matplotlib`, `seaborn` - Visualización

---

## 📊 Datos

### Descripción del Dataset

| Aspecto | Detalle |
|---------|---------|
| **Archivo** | `retail_customer_data-1.csv` |
| **Observaciones** | Clientes de MegaMart |
| **Variables** | Comportamiento de compra y características demográficas |
| **Tipo** | Datos transaccionales agregados por cliente |

### Variables Clave

- **total_spent** - Gasto total del cliente
- **avg_basket_size** - Tamaño promedio de canasta
- **visit_frequency** - Frecuencia de visitas
- **recency** - Días desde última compra
- Variables demográficas y de comportamiento

📄 Ver [DATA_DICTIONARY.md](./DATA_DICTIONARY.md) para descripción completa de variables.

---

## 🎯 Hallazgos Principales

- ✅ **Estandarización necesaria:** Variables con escalas muy diferentes requirieron normalización previa
- ✅ **Correlaciones identificadas:** Algunas variables altamente correlacionadas (ej. total_spent y avg_basket_size)
- ✅ **Outliers detectados:** Presencia de valores atípicos identificados mediante boxplots
- ✅ **Número óptimo de clusters:** Determinado mediante método del codo y coeficiente de silueta
- ✅ **Segmentos diferenciados:** Clusters con perfiles de comportamiento claramente distintos

---

## 💼 Recomendaciones de Negocio

1. **Personalizar comunicaciones por segmento:** Adaptar mensajes y canales según características de cada cluster

2. **Diseñar ofertas específicas:** Crear promociones que resuenen con las necesidades de cada segmento identificado

3. **Priorizar retención de alto valor:** Enfocar esfuerzos de retención en clusters que generan mayor valor

### Impacto Esperado

- Mayor efectividad de campañas de marketing
- Aumento en tasa de conversión de ofertas
- Mejor retención de clientes de alto valor

### Próximos Pasos

- Validar segmentos con datos de nuevos períodos
- Desarrollar perfiles detallados (personas) por cluster
- Integrar segmentación en sistemas de CRM y marketing automation

---

## 📁 Archivos

| Archivo | Descripción |
|---------|-------------|
| `customer_clustering_analysis.ipynb` | Notebook con análisis completo |
| `retail_customer_data-1.csv` | Dataset original |
| `DATA_DICTIONARY.md` | Diccionario de datos |
| `instructions-1.pdf` | Instrucciones del caso |

---

## ▶️ Cómo Ejecutar

```bash
# Desde la raíz del repositorio
cd case-03-cluster-analysis
jupyter notebook customer_clustering_analysis.ipynb
```

---

## 🎬 Video Explicativo

🔗 [Ver video en YouTube](https://www.youtube.com/watch?v=f_WuRfuMXQw)