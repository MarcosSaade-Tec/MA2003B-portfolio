# Portfolio MA2003B - Métodos Multivariados

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📋 Descripción General

Este portfolio presenta tres casos de estudio que demuestran la aplicación práctica de métodos estadísticos multivariados para el análisis de datos en contextos empresariales reales. Cada caso aborda un problema de negocio diferente utilizando técnicas apropiadas de análisis multivariado.

El objetivo principal es demostrar competencia en la selección, aplicación e interpretación de métodos multivariados, así como la capacidad de comunicar hallazgos técnicos de manera efectiva a audiencias de negocio.

---

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Institución:** Tecnológico de Monterrey  
**Curso:** MA2003B - Métodos Multivariados para Ciencia de Datos  
**Profesor:** Juliho Castillo Colmenares  
**Equipo:** 5

---

## 📑 Tabla de Contenidos

- [Descripción General](#-descripción-general)
- [Autores](#-autores)
- [Resumen de Casos de Estudio](#-resumen-de-casos-de-estudio)
- [Estructura del Repositorio](#-estructura-del-repositorio)
- [Instalación y Reproducibilidad](#-instalación-y-reproducibilidad)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Licencia](#-licencia)

---

## 📊 Resumen de Casos de Estudio

| Caso | Método | Pregunta de Negocio | Hallazgo Clave | Link |
|------|--------|---------------------|----------------|------|
| TechnoServe Customer Satisfaction | Factor Analysis | ¿Qué dimensiones latentes impulsan la satisfacción del cliente? | 5 factores explican la mayoría de la varianza; Excelencia Técnica es el factor más importante | [Ver caso →](./case-01-factor-analysis/) |
| LendSmart Credit Risk | Discriminant Analysis | ¿Cómo clasificar aplicantes de crédito en categorías de riesgo? | Modelo con alta accuracy; ingreso anual y ratio deuda-ingreso son predictores clave | [Ver caso →](./case-02-discriminant-analysis/) |
| MegaMart Customer Segmentation | Cluster Analysis | ¿Qué segmentos naturales existen en la base de clientes? | Múltiples clusters identificados con perfiles de comportamiento diferenciados | [Ver caso →](./case-03-cluster-analysis/) |

---

## 📁 Estructura del Repositorio

```
MA2003B-portfolio/
│
├── README.md                          # Este archivo - descripción general
├── LICENSE                            # Licencia MIT
├── .gitignore                         # Configuración para Python
├── requirements.txt                   # Dependencias del proyecto
│
├── case-01-factor-analysis/           # Caso 1: Análisis Factorial
│   ├── README.md                      # Descripción del caso
│   ├── DATA_DICTIONARY.md             # Diccionario de datos
│   ├── customer_satisfaction_data.csv # Dataset
│   ├── main.ipynb                     # Notebook de análisis
│   └── Resumen_Ejecutivo.pdf          # Resumen ejecutivo
│
├── case-02-discriminant-analysis/     # Caso 2: Análisis Discriminante
│   ├── README.md                      # Descripción del caso
│   ├── DATA_DICTIONARY.md             # Diccionario de datos
│   ├── credit_risk_data-1.csv         # Dataset
│   ├── LeadSmart_Analysis.ipynb       # Notebook de análisis
│   └── instructions.pdf               # Instrucciones originales
│
├── case-03-cluster-analysis/          # Caso 3: Análisis de Clusters
│   ├── README.md                      # Descripción del caso
│   ├── DATA_DICTIONARY.md             # Diccionario de datos
│   ├── retail_customer_data-1.csv     # Dataset
│   ├── customer_clustering_analysis.ipynb  # Notebook de análisis
│   └── instructions-1.pdf             # Instrucciones originales
│
├── portfolio-summary/                 # Documentos integradores
│   ├── PORTFOLIO_OVERVIEW.md          # Resumen integrador
│   ├── LESSONS_LEARNED.md             # Reflexiones críticas
│   └── METHODOLOGY_COMPARISON.md      # Comparación de métodos
│
└── presentation/                      # Presentación final
    └── README.md                      # Instrucciones de presentación
```

---

## 🚀 Instalación y Reproducibilidad

### Requisitos

- Python 3.8 o superior
- pip o conda para gestión de paquetes
- Jupyter Notebook o JupyterLab

### Pasos de Instalación

1. **Clonar el repositorio:**

```bash
git clone https://github.com/MarcosSaade-Tec/MA2003B-portfolio.git
cd MA2003B-portfolio
```

2. **Crear un entorno virtual (recomendado):**

```bash
python -m venv venv

# En Windows:
venv\Scripts\activate

# En macOS/Linux:
source venv/bin/activate
```

3. **Instalar dependencias:**

```bash
pip install -r requirements.txt
```

4. **Ejecutar los notebooks:**

```bash
jupyter notebook
```

Navegar a la carpeta del caso deseado y abrir el notebook correspondiente.

### Ejecución de Notebooks

| Caso | Notebook | Comando |
|------|----------|---------|
| Factor Analysis | `main.ipynb` | `jupyter notebook case-01-factor-analysis/main.ipynb` |
| Discriminant Analysis | `LeadSmart_Analysis.ipynb` | `jupyter notebook case-02-discriminant-analysis/LeadSmart_Analysis.ipynb` |
| Cluster Analysis | `customer_clustering_analysis.ipynb` | `jupyter notebook case-03-cluster-analysis/customer_clustering_analysis.ipynb` |

---

## 🛠️ Tecnologías Utilizadas

- **Python 3.x** - Lenguaje de programación principal
- **Jupyter Notebooks** - Entorno de desarrollo interactivo
- **Bibliotecas principales:**
  - `pandas` - Manipulación de datos
  - `numpy` - Cómputo numérico
  - `scikit-learn` - Machine learning y clustering
  - `scipy` - Funciones estadísticas
  - `matplotlib` - Visualización
  - `seaborn` - Visualización estadística
  - `factor-analyzer` - Análisis factorial
  - `pingouin` - Análisis estadístico
  - `statsmodels` - Modelos estadísticos

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

---

## 📞 Contacto

Para preguntas o comentarios sobre este portfolio, contactar a los autores a través de sus perfiles institucionales del Tecnológico de Monterrey.
