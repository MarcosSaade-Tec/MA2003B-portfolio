# Caso 02 — Análisis Discriminante

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5**

---

## 🏢 Contexto del Negocio

**Cliente:** LendSmart - Institución financiera de préstamos

**Problema:** La empresa necesita un sistema objetivo para clasificar solicitantes de crédito en categorías de riesgo (default vs no default), reduciendo pérdidas por morosidad mientras mantiene una cartera de clientes saludable.

**Importancia estratégica:** Una clasificación precisa del riesgo crediticio permite aprobar préstamos de manera más eficiente, reducir tasas de incumplimiento y optimizar la rentabilidad del portafolio de créditos.

---

## 🔬 Metodología

### Métodos Aplicados

- **Linear Discriminant Analysis (LDA)** - Clasificación asumiendo covarianzas iguales entre grupos
- **Quadratic Discriminant Analysis (QDA)** - Clasificación permitiendo covarianzas diferentes

### Justificación

- Variable dependiente categórica binaria (default/no default)
- Necesidad de modelo interpretable para decisiones de crédito
- Comparación de métodos para seleccionar el más apropiado

### Herramientas y Librerías

- Python 3.x
- `scikit-learn` - Implementación de LDA y QDA
- `pingouin` - Análisis estadístico
- `pandas`, `numpy` - Manipulación de datos
- `matplotlib`, `seaborn` - Visualización

---

## 📊 Datos

### Descripción del Dataset

| Aspecto | Detalle |
|---------|---------|
| **Archivo** | `credit_risk_data-1.csv` |
| **Observaciones** | Solicitudes de crédito históricas |
| **Variable objetivo** | `loan_status` (0 = no default, 1 = default) |
| **Variables predictoras** | Demográficas, financieras, historial crediticio |

### Variables Clave

- **annual_income** - Ingreso anual del solicitante
- **debt_to_income** - Ratio deuda/ingreso
- **employment_years** - Años de empleo
- **asset_value** - Valor de activos
- **credit_history** - Historial crediticio

📄 Ver [DATA_DICTIONARY.md](./DATA_DICTIONARY.md) para descripción completa de variables.

---

## 🎯 Hallazgos Principales

- ✅ **Desbalance de clases:** Identificado y manejado mediante estratificación en train/test split
- ✅ **Variables más discriminantes:** Ingreso anual, ratio deuda-ingreso, años de empleo y valor de activos muestran mayor separación entre clases
- ✅ **Información mutua:** Cuantificación de la relevancia de cada variable para la clasificación
- ✅ **Comparación LDA vs QDA:** Evaluación de ambos modelos con métricas de clasificación
- ✅ **Performance del modelo:** Alta accuracy en la clasificación de riesgo crediticio

---

## 💼 Recomendaciones de Negocio

1. **Implementar modelo en proceso de aprobación:** Usar el modelo discriminante como herramienta de screening inicial para solicitudes de crédito

2. **Monitorear variables clave:** Establecer alertas cuando ingreso o ratio deuda-ingreso de solicitantes estén en rangos de alto riesgo

3. **Revisar umbrales periódicamente:** Ajustar puntos de corte del modelo según evolución de la cartera y condiciones del mercado

### Impacto Esperado

- Reducción de tasa de default
- Proceso de aprobación más eficiente y objetivo
- Mejor gestión del riesgo crediticio

### Próximos Pasos

- Validar modelo con datos más recientes
- Explorar técnicas de balanceo de clases (SMOTE, undersampling)
- Implementar monitoreo de drift del modelo

---

## 📁 Archivos

| Archivo | Descripción |
|---------|-------------|
| `LeadSmart_Analysis.ipynb` | Notebook con análisis completo |
| `credit_risk_data-1.csv` | Dataset original |
| `DATA_DICTIONARY.md` | Diccionario de datos |
| `instructions.pdf` | Instrucciones del caso |

---

## ▶️ Cómo Ejecutar

```bash
# Desde la raíz del repositorio
cd case-02-discriminant-analysis
jupyter notebook LeadSmart_Analysis.ipynb
```