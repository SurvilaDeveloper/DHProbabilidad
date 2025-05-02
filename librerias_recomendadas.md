# 🧮 Librerías de Python para Resolver Problemas de Probabilidad

Existen diversas librerías en Python que permiten resolver problemas de **probabilidad** y **estadística**, ya sea mediante cálculos teóricos, simulaciones, visualizaciones o modelado bayesiano.

---

## 📦 Librerías para cálculo de distribuciones y estadística clásica

### ✅ `scipy.stats`
- Biblioteca principal para trabajar con distribuciones de probabilidad (discretas y continuas).
- Incluye funciones como `pdf`, `cdf`, `ppf`, generación aleatoria, etc.
- Más de 100 distribuciones disponibles.

---

## 📊 Librerías para simulación y visualización

### ✅ `numpy`
- Contiene el módulo `numpy.random` para generar valores aleatorios de distribuciones comunes.
- Muy eficiente para simulaciones Monte Carlo.

### ✅ `matplotlib` y `seaborn`
- Herramientas estándar para graficar funciones de densidad, histogramas, funciones acumuladas.
- `seaborn` agrega funciones estadísticas como `sns.histplot`, `sns.kdeplot`, etc.

### ✅ `plotly`
- Ofrece gráficos interactivos, útiles para explorar visualmente distribuciones.

---

## 🔁 Librerías para simulaciones probabilísticas y modelos bayesianos

### ✅ `PyMC` (v5)
- Framework para modelos probabilísticos bayesianos.
- Usa MCMC y otros métodos de inferencia.
- Permite definir modelos estadísticos complejos.

### ✅ `TensorFlow Probability`
- Basado en TensorFlow.
- Útil para integrar probabilidad en redes neuronales bayesianas.

### ✅ `NumPyro`
- Similar a PyMC, pero construido sobre JAX para una mayor eficiencia en simulaciones.

---

## 🧮 Librerías para álgebra simbólica

### ✅ `sympy.stats`
- Permite definir variables aleatorias de forma simbólica.
- Permite calcular probabilidades, esperanzas y varianzas exactas.

```python
from sympy.stats import Normal, P
X = Normal('X', 0, 1)
P(X > 1)  # Probabilidad simbólica

| Necesidad                          | Librería recomendada            |
|-----------------------------------|---------------------------------|
| Distribuciones y cálculos         | `scipy.stats`, `numpy.random`   |
| Simulaciones básicas              | `numpy`, `random`               |
| Gráficos                          | `matplotlib`, `seaborn`, `plotly` |
| Modelado bayesiano                | `PyMC`, `NumPyro`, `TFP`        |
| Cálculo simbólico                 | `sympy.stats`                   |
| Modelos estadísticos clásicos     | `statsmodels`                   |