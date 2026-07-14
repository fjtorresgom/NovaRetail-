# NovaRetail-

## Descripción

Este proyecto tiene como objetivo identificar qué variables del comportamiento de los clientes están más asociadas con el ingreso anual generado para NovaRetail+ durante 2024. Para ello, se aplicaron técnicas de análisis correlacional utilizando variables numéricas, binarias y categóricas.

El análisis tiene un enfoque exploratorio y correlacional, por lo que los resultados permiten identificar asociaciones entre variables, pero no establecer relaciones de causalidad.

---

## Dataset

**Archivo utilizado:**

`/datasets/novaretail_comportamiento_clientes_2024.csv`

### Variables analizadas

- id_cliente
- edad
- nivel_ingreso
- visitas_mes
- compras_mes
- gasto_publicidad_dirigida
- satisfaccion
- miembro_premium
- abandono
- tipo_dispositivo
- region
- ingreso_anual

La variable principal de análisis fue **ingreso_anual**, utilizada para evaluar el valor económico generado por cada cliente.

---

## Objetivos del proyecto

- Explorar la estructura y calidad de los datos.
- Identificar relaciones entre variables numéricas mediante correlaciones de Pearson y Spearman.
- Analizar asociaciones entre variables binarias y numéricas mediante correlación punto-biserial.
- Evaluar asociaciones entre variables categóricas mediante V de Cramér.
- Generar evidencia visual y numérica para apoyar los hallazgos.
- Proponer implicaciones de negocio basadas en los resultados obtenidos.

---

## Metodología

### 1. Exploración y preparación de datos

- Revisión de tipos de datos.
- Verificación de valores nulos.
- Clasificación de variables numéricas, binarias y categóricas.
- Definición de supuestos del análisis.

### 2. Análisis exploratorio

- Estadísticas descriptivas.
- Distribución de variables numéricas.
- Exploración de variables binarias y categóricas.

### 3. Visualización de relaciones

- Heatmap de correlaciones.
- Scatterplots para relaciones relevantes.
- Identificación visual de patrones y tendencias.

### 4. Análisis correlacional

Se aplicaron distintos coeficientes según la naturaleza de las variables:

- **Pearson:** relaciones lineales entre variables numéricas.
- **Spearman:** relaciones monotónicas entre variables numéricas.
- **Punto-biserial:** relaciones entre variables binarias y numéricas.
- **V de Cramér:** asociaciones entre variables categóricas.

---

## Principales hallazgos

### Hallazgo 1: Las compras mensuales son el principal driver asociado al ingreso anual

- Pearson: **0.967**
- Spearman: **0.967**

Se identificó una asociación positiva muy fuerte entre el número de compras realizadas y el ingreso anual generado por los clientes.

### Hallazgo 2: Las visitas mensuales presentan una asociación moderada con el ingreso

- Pearson: **0.337**
- Spearman: **0.321**

Los clientes que visitan con mayor frecuencia la plataforma tienden a generar mayores ingresos, aunque la relación es considerablemente menor que la observada para las compras.

### Hallazgo 3: Las variables demográficas y categóricas tienen poca capacidad explicativa

Variables como edad, nivel de ingreso, región, tipo de dispositivo, membresía premium y abandono mostraron asociaciones débiles o prácticamente nulas con el ingreso anual.

---

## Limitaciones

- La correlación no implica causalidad.
- El análisis se basa en datos observacionales.
- Solo se analizaron las variables disponibles en el dataset.
- Pueden existir variables externas no incluidas que expliquen parte del comportamiento observado.
- Los resultados representan únicamente el período analizado.

---

## Recomendaciones

- Implementar estrategias para aumentar la frecuencia de compra de los clientes.
- Fortalecer acciones de engagement para incrementar las visitas a la plataforma.
- Realizar modelos predictivos para cuantificar el impacto conjunto de múltiples variables.
- Diseñar experimentos controlados (A/B Testing) para validar hipótesis antes de implementar cambios estratégicos.

---

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- SciPy
- Jupyter Notebook

---

## Cómo ejecutar el proyecto

1. Clonar el repositorio:

```bash
git clone https://github.com/usuario/proyecto-novaretail.git
```

2. Instalar dependencias:

```bash
pip install pandas numpy matplotlib seaborn scipy
```

3. Abrir el notebook en Jupyter Notebook o Google Colab.

---

## Conclusión

El análisis permitió identificar que las variables de comportamiento, especialmente el número de compras mensuales, presentan la asociación más fuerte con el ingreso anual generado por los clientes. Por el contrario, las variables demográficas, binarias y categóricas mostraron una influencia mínima. Estos hallazgos sugieren que las estrategias de crecimiento deberían enfocarse en incrementar la actividad transaccional de los usuarios y fortalecer los mecanismos de retención y fidelización.
