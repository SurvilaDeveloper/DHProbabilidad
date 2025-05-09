# 📏 Métricas de una Distribución de Probabilidad

Las **métricas de una distribución de probabilidad** son medidas que describen diferentes aspectos del comportamiento de una variable aleatoria. Estas métricas permiten resumir, interpretar y comparar distribuciones. A continuación se describen las métricas más comunes y útiles:

---

## 1. **Media (Esperanza Matemática)** — $ \mu = \mathbb{E}[X] $
- Representa el valor promedio esperado de una distribución.
- En distribuciones simétricas, suele coincidir con la mediana y la moda.
- Se interpreta como el “centro de masa” de la distribución.

---

## 2. **Varianza** — $ \sigma^2 = \mathbb{V}[X] $
- Mide la dispersión de los valores de la variable aleatoria respecto a la media.
- Cuanto mayor sea la varianza, mayor es la dispersión de los valores.

---

## 3. **Desviación Estándar** — $ \sigma = \sqrt{\mathbb{V}[X]} $
- Es la raíz cuadrada de la varianza.
- Tiene las mismas unidades que la variable aleatoria, lo que facilita su interpretación.

---

## 4. **Moda**
- Es el valor con mayor densidad o probabilidad en una distribución.
- En distribuciones simétricas como la normal, suele coincidir con la media.
- Algunas distribuciones pueden no tener moda, o pueden tener más de una (bimodales, multimodales).

---

## 5. **Coeficiente de Asimetría (Skewness)** — $\gamma_1$
- Mide qué tan simétrica es una distribución.
  - $\gamma_1 > 0$: Sesgo a la derecha (cola larga hacia la derecha).
  - $\gamma_1 < 0$: Sesgo a la izquierda (cola larga hacia la izquierda).

---

## 6. **Curtosis** — $ \gamma_2 $
- Mide la forma de las colas de la distribución en comparación con una distribución normal.
  - **Curtosis > 3**: Colas más pesadas (leptocúrtica).
  - **Curtosis < 3**: Colas más ligeras (platicúrtica).
  - **Curtosis = 3**: Distribución normal (mesocúrtica).

---

## 7. **Función de Distribución Acumulada (CDF)** — $ F(x) = P(X \le x) $
- Da la probabilidad de que la variable aleatoria sea menor o igual a un valor específico.

---

## 8. **Función de Densidad (PDF) o Masa (PMF)**
- Describe cómo se distribuyen las probabilidades o densidades de la variable aleatoria.
  - **PDF**: Para distribuciones continuas.
  - **PMF**: Para distribuciones discretas.

---

## Otras Métricas Útiles (Avanzadas)

- **Mediana**: Valor que divide la distribución en dos partes iguales.
- **Rango Intercuartílico (IQR)**: Medida de dispersión entre el percentil 25 y el 75.
- **Momentos**: Valores esperados de potencias de $X$ que proporcionan información sobre la forma de la distribución.

---

Estas métricas te permitirán entender y comparar el comportamiento de diferentes distribuciones de probabilidad de manera más detallada.

