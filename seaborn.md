# seaborn

```python
import seaborn as sns
import matplotlib.pyplot as plt
```

| Tipo de Gráfico           | Función en Seaborn                  | Descripción                                                      |
|---------------------------|-------------------------------------|------------------------------------------------------------------|
| **Distribución univariada**| `sns.histplot()`                    | Histograma con posibilidad de superponer una distribución        |
|                           | `sns.kdeplot()`                     | Gráfico de densidad de Kernel                                     |
|                           | `sns.displot()`                     | Gráfico de distribución de datos                                  |
| **Distribución bivariada** | `sns.jointplot()`                   | Relación entre dos variables, con diferentes opciones de visualización|
|                           | `sns.pairplot()`                    | Matriz de gráficos para explorar relaciones entre múltiples variables|
| **Gráfico de cajas**       | `sns.boxplot()`                     | Boxplot mostrando la distribución de datos con caja y bigotes    |
|                           | `sns.violinplot()`                  | Boxplot combinado con un gráfico de densidad                      |
|                           | `sns.boxenplot()`                   | Variante del boxplot mostrando más detalles de las colas         |
| **Gráfico de barras**      | `sns.barplot()`                     | Barra para representar la media (o alguna estadística) de una variable categórica |
|                           | `sns.countplot()`                   | Muestra el conteo de observaciones para cada categoría            |
| **Gráfico de puntos**      | `sns.pointplot()`                   | Muestra la media de una categoría en formato de puntos           |
| **Gráfico de segmentos**   | `sns.stripplot()`                   | Muestra las observaciones individuales en una categoría          |
|                           | `sns.swarmplot()`                   | Similar a stripplot, pero ajusta las posiciones para evitar superposiciones |
| **Gráfico de regresión**   | `sns.regplot()`                     | Gráfico de dispersión con línea de regresión ajustada             |
|                           | `sns.lmplot()`                      | Similar a `regplot()`, pero con la posibilidad de facetado       |
| **Gráfico de dispersión**  | `sns.relplot()`                     | Gráfico de dispersión con opciones de ajuste (como regresión)    |
| **Gráfico de matriz**      | `sns.heatmap()`                     | Muestra una matriz de valores con colores representando magnitudes |
|                           | `sns.clustermap()`                  | Muestra una matriz de distancias o correlaciones con un clúster jerárquico |
| **Gráfico de facetas**     | `sns.FacetGrid()`                   | Crea subgráficos en un grid para comparar distribuciones o relaciones entre variables |
|                           | `sns.catplot()`                     | Gráficos categóricos en un grid de facetas                       |
| **Gráfico de series temporales** | `sns.lineplot()`            | Gráfico de líneas para representar series temporales             |
| **Gráfico de densidad**    | `sns.kdeplot()`                     | Estimación de la densidad de probabilidad de una o dos variables |
| **Gráfico de correlación** | `sns.pairplot()`                    | Matriz de gráficos de dispersión para comparar las relaciones entre múltiples variables|
