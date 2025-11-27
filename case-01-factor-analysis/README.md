# Caso 01 — Análisis Factorial

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5**

---

## 🏢 Contexto del Negocio

**Cliente:** TechnoServe Solutions - Firma de consultoría tecnológica

**Problema:** La empresa recopila extensas encuestas de satisfacción con 23 ítems diferentes, lo que dificulta identificar qué aspectos son realmente importantes para los clientes y cómo priorizar mejoras.

**Importancia estratégica:** Comprender las dimensiones subyacentes de la satisfacción del cliente permite a TechnoServe enfocar recursos en las áreas que generan mayor impacto, optimizando la experiencia del cliente y aumentando la retención.

---

## 🔬 Metodología

### Método Aplicado

**Análisis Factorial Exploratorio (EFA)** - Técnica de reducción de dimensionalidad que identifica factores latentes subyacentes a un conjunto de variables observadas.

### Justificación

- Dataset con 23 variables de satisfacción altamente correlacionadas
- Necesidad de simplificar la estructura de datos
- Objetivo de descubrir patrones no evidentes en las respuestas

### Herramientas y Librerías

- Python 3.x
- `factor_analyzer` - Implementación de análisis factorial
- `pandas`, `numpy` - Manipulación de datos
- `matplotlib`, `seaborn` - Visualización
- `scipy` - Pruebas estadísticas

---

## 📊 Datos

### Descripción del Dataset

| Aspecto | Detalle |
|---------|---------|
| **Archivo** | `customer_satisfaction_data.csv` |
| **Observaciones** | 3,400 respuestas |
| **Clientes únicos** | 850 |
| **Variables de satisfacción** | 23 ítems (escala Likert 1-7) |
| **Período** | Q1-Q4 2024 |

### Variables Clave

Las 23 variables de satisfacción se agrupan en 5 categorías originales:

- **Technical Excellence & Innovation** (5 variables)
- **Relationship Management & Communication** (5 variables)
- **Project Delivery & Quality** (5 variables)
- **Value & Financial Transparency** (5 variables)
- **Support & Service Excellence** (3 variables)

📄 Ver [DATA_DICTIONARY.md](./DATA_DICTIONARY.md) para descripción completa de variables.

---

## 🎯 Hallazgos Principales

- ✅ **Validación de idoneidad:** KMO y Test de Bartlett confirman que los datos son apropiados para análisis factorial
- ✅ **Reducción efectiva:** 23 variables originales reducidas a factores interpretables
- ✅ **Factores identificados:** Dimensiones latentes claras que agrupan aspectos relacionados de satisfacción
- ✅ **Excelencia Técnica:** Emerge como el factor con mayor peso en la satisfacción general
- ✅ **Varianza explicada:** Los factores retenidos explican un porcentaje significativo de la varianza total

---

## 💼 Recomendaciones de Negocio

1. **Priorizar inversión en excelencia técnica:** Dado que es el factor más importante, enfocar recursos en capacitación técnica y mejora de soluciones

2. **Simplificar encuestas futuras:** Usar los factores identificados para crear encuestas más cortas pero igualmente informativas

3. **Segmentar estrategias de mejora:** Diferentes clientes pueden valorar diferentes factores; personalizar acciones según perfiles

### Impacto Esperado

- Reducción del tiempo de análisis de encuestas
- Mayor claridad en priorización de mejoras
- Mejor asignación de recursos de servicio al cliente

### Próximos Pasos

- Validar factores con análisis factorial confirmatorio (CFA)
- Desarrollar dashboard de seguimiento por factor
- Integrar scores factoriales en CRM

---

## 📁 Archivos

| Archivo | Descripción |
|---------|-------------|
| `main.ipynb` | Notebook con análisis completo |
| `customer_satisfaction_data.csv` | Dataset original |
| `DATA_DICTIONARY.md` | Diccionario de datos |
| `Resumen_Ejecutivo.pdf` | Resumen ejecutivo |

---

## ▶️ Cómo Ejecutar

```bash
# Desde la raíz del repositorio
cd case-01-factor-analysis
jupyter notebook main.ipynb
```