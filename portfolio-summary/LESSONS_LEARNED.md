# Lessons Learned - Reflexiones Críticas

## 👥 Autores

| Nombre | Matrícula |
|--------|-----------|
| **Marcos Saade** | A01784220 |
| **Gabriel Masri** | A10666353 |

**Equipo 5** - Tecnológico de Monterrey

---

## 📚 Reflexiones por Caso

### Caso 1: Análisis Factorial

**¿Qué funcionó bien?**
- La verificación de supuestos (KMO, Bartlett) antes del análisis
- La interpretación de factores basada en cargas factoriales
- La visualización con scree plots para determinar número de factores

**¿Qué aprendimos?**
- La importancia de validar la idoneidad de los datos para análisis factorial
- Cómo la rotación (varimax, promax) afecta la interpretabilidad
- La diferencia entre análisis factorial exploratorio y confirmatorio

**Desafíos enfrentados:**
- Decidir el número óptimo de factores a retener
- Interpretar factores cuando las cargas no son claramente diferenciadas
- Manejar variables con comunalidades bajas

---

### Caso 2: Análisis Discriminante

**¿Qué funcionó bien?**
- La comparación sistemática entre LDA y QDA
- El uso de validación cruzada para evaluar el modelo
- La visualización de resultados con matrices de confusión y curvas ROC

**¿Qué aprendimos?**
- Cuándo es apropiado usar LDA vs QDA según los supuestos
- La importancia del balance de clases en problemas de clasificación
- Cómo interpretar la información mutua para selección de variables

**Desafíos enfrentados:**
- Manejar el desbalance de clases en los datos
- Verificar el supuesto de normalidad multivariada
- Evaluar la homogeneidad de matrices de covarianza

---

### Caso 3: Análisis de Clusters

**¿Qué funcionó bien?**
- El uso de múltiples métodos (K-means y jerárquico) para validar resultados
- La aplicación de métricas como el coeficiente de silueta
- La caracterización detallada de cada cluster

**¿Qué aprendimos?**
- La importancia de estandarizar variables antes del clustering
- Cómo usar dendrogramas para determinar el número de clusters
- La necesidad de validar la estabilidad de los clusters

**Desafíos enfrentados:**
- Determinar el número óptimo de clusters
- Manejar outliers que afectan la formación de grupos
- Interpretar clusters cuando hay muchas variables

---

## 🔑 Aprendizajes Transversales

### Preparación de Datos
- **Siempre** verificar datos faltantes y outliers antes del análisis
- La estandarización es crítica cuando las variables tienen escalas diferentes
- La calidad de los resultados depende directamente de la calidad de los datos

### Validación de Supuestos
- Cada técnica tiene supuestos específicos que deben verificarse
- No validar supuestos puede llevar a conclusiones erróneas
- Existen alternativas robustas cuando los supuestos no se cumplen

### Interpretación de Resultados
- Los resultados estadísticos deben traducirse a lenguaje de negocio
- Las visualizaciones son fundamentales para comunicar hallazgos
- Siempre considerar las limitaciones del análisis

### Herramientas y Código
- Documentar el código facilita la reproducibilidad
- Las bibliotecas de Python ofrecen implementaciones robustas
- Es importante entender qué hace cada función, no solo usarla

---

## 💡 Recomendaciones para Futuros Proyectos

1. **Planificar antes de codificar:** Definir claramente objetivos y preguntas de investigación
2. **Explorar exhaustivamente:** No saltar directamente al modelo sin entender los datos
3. **Validar siempre:** Usar técnicas de validación cruzada y múltiples métricas
4. **Iterar:** El primer modelo rara vez es el mejor
5. **Documentar:** Mantener registro de decisiones y justificaciones

---

## 🚀 Próximos Pasos

- Explorar técnicas más avanzadas (SEM, PLS, clustering espectral)
- Aplicar estos métodos en proyectos de industria real
- Profundizar en la automatización de pipelines de análisis

---

## 🎓 Aplicaciones Futuras en Nuestra Carrera Profesional

### En Ciencia de Datos e Inteligencia de Negocios

Los métodos aprendidos son fundamentales para roles de Data Scientist y Business Analyst:

- **Factor Analysis:** Desarrollo de índices de satisfacción, análisis de marca, reducción de features antes de modelos de ML
- **Discriminant Analysis:** Scoring crediticio, detección de fraude, clasificación de leads en ventas
- **Cluster Analysis:** Segmentación de clientes, personalización de productos, análisis de comportamiento

### En Consultoría y Estrategia

Estos métodos permiten ofrecer insights basados en evidencia:

- Transformar datos complejos en recomendaciones accionables
- Justificar decisiones estratégicas con análisis cuantitativo
- Comunicar hallazgos técnicos a audiencias ejecutivas

### En Desarrollo de Productos

Aplicaciones en mejora continua y desarrollo de nuevos productos:

- Identificar atributos clave que valoran los clientes
- Segmentar mercados para desarrollo de productos específicos
- Predecir adopción de nuevos productos/servicios

### Habilidades Transferibles

Más allá de los métodos específicos, desarrollamos competencias valiosas:

1. **Pensamiento analítico:** Descomponer problemas complejos en partes manejables
2. **Comunicación de datos:** Traducir hallazgos estadísticos a lenguaje de negocio
3. **Programación en Python:** Herramienta esencial para cualquier rol analítico
4. **Documentación profesional:** Crear reportes y notebooks reproducibles
5. **Trabajo colaborativo:** Gestión de proyectos con Git y metodologías ágiles
