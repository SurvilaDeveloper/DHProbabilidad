---
---
# Distribuciones de Probabilidad

Una **distribución de probabilidades** describe cómo se distribuyen los posibles valores de una variable aleatoria, asignando una probabilidad a cada resultado. Existen dos tipos principales de distribuciones de probabilidad: **discretas** y **continuas**.

---
---

## Distribuciones Discretas
---
1. ### Distribución Bernoulli
   - Describe un experimento con dos posibles resultados: **éxito** (1) o **fracaso** (0).
   - La probabilidad de éxito es **p** y la de fracaso es **1-p**.
   - La probabilidad de que ocurra un éxito es:
   $$
   P(X = 1) = p, \quad P(X = 0) = 1 - p
   $$

   **Ejemplo:** Lanzamiento de una moneda.
---
2. ### Distribución Binomial
   - Se utiliza cuando tenemos **n ensayos** independientes y la variable de interés tiene dos resultados posibles (éxito o fracaso).
   - La probabilidad de éxito en cada ensayo es **p**.
   - La fórmula para la probabilidad de obtener exactamente **x** éxitos en **n** ensayos es:
   $$
   P(X = x) = \binom{n}{x} p^x (1-p)^{n-x}
   $$

   **Ejemplo:** El número de caras al lanzar 5 veces una moneda.
---
3. ### Distribución Geométrica
   - Modela el número de ensayos necesarios hasta obtener el primer éxito en un proceso de Bernoulli.
   - La probabilidad de que el primer éxito ocurra en el **x**-ésimo ensayo es:
   $$
   P(X = x) = (1 - p)^{x-1} p
   $$

   **Ejemplo:** El número de lanzamientos de una moneda necesarios para obtener la primera cara.
---
4. ### Distribución Hipergeométrica
   - Describe la probabilidad de obtener **k** éxitos en **n** ensayos sin reemplazo, de una población que contiene **K** éxitos en total.
   - La fórmula es:
   $$
   P(X = k) = \frac{\binom{K}{k} \binom{N-K}{n-k}}{\binom{N}{n}}
   $$

   **Ejemplo:** Extraer bolas de una urna sin reemplazo.
---
5. ### Distribución Poisson
   - Describe el número de eventos que ocurren en un intervalo de tiempo o espacio fijo, cuando los eventos ocurren de manera independiente y a una tasa promedio constante.
   - La fórmula de la función de probabilidad es:
   $$
   P(X = x) = \frac{e^{-\lambda} \lambda^x}{x!}
   $$

   **Ejemplo:** El número de autos que pasan por un peaje en una hora.
---
6. ### Distribución Binomial Negativa: Dos Formulaciones

---

La **distribución binomial negativa** modela la cantidad de ensayos necesarios hasta obtener un número fijo de éxitos \( r \), en una secuencia de ensayos de Bernoulli independientes con probabilidad de éxito \( p \).

#### 🔹 Opción 1: Total de ensayos hasta el r-ésimo éxito

Esta forma modela la **cantidad total de ensayos** necesarios para obtener exactamente \( r \) éxitos.

$$
P(X = x) = \binom{x - 1}{r - 1} \cdot p^r \cdot (1 - p)^{x - r}
$$

- \( X \): número total de ensayos hasta obtener el \( r \)-ésimo éxito.
- Soporte: \( x = r, r+1, r+2, \dots \)

---

#### 🔹 Opción 2: Número de fracasos antes del r-ésimo éxito

Esta formulación modela la **cantidad de fracasos** observados antes de obtener el \( r \)-ésimo éxito.

$$
P(X = k) = \binom{k + r - 1}{r - 1} \cdot p^r \cdot (1 - p)^k
$$

- \( X \): número de fracasos antes de obtener el \( r \)-ésimo éxito.
- Soporte: \( k = 0, 1, 2, \dots \)

---

**Uso típico**

- Evaluar cuántos errores comete un operador antes de completar una cierta cantidad de tareas correctamente.
- Contar cuántas veces falla un sistema antes de que funcione correctamente varias veces.
- Modelar situaciones de conteo hasta el éxito repetido (como en telecomunicaciones, biología, etc.).

---
---
7. ### Distribución Uniforme Discreta
   - Es aquella en la que **todos los valores enteros dentro de un rango específico tienen la misma probabilidad de ocurrir**.

**Definición formal**

Sea \( X \) una variable aleatoria discreta que toma valores enteros \( x_1, x_2, \ldots, x_n \). Se dice que \( X \) tiene una distribución uniforme discreta si:

$$
P(X = x_i) = \frac{1}{n}, \quad \text{para } i = 1, 2, \ldots, n
$$

   **Ejemplo** Si tirás un dado justo de 6 caras:

- Los posibles valores son \( 1, 2, 3, 4, 5, 6 \)
- Cada uno tiene la misma probabilidad: 

$$
P(X = k) = \frac{1}{6}, \quad \text{para } k = 1,2,\dots,6
$$

---
---

## Distribuciones Continuas

1. ### Distribución Uniforme
   - En la distribución uniforme continua, todos los valores dentro de un intervalo tienen la misma probabilidad de ocurrir.
   - La función de densidad es:
   $$
   f(x) = \frac{1}{b - a}, \quad a \leq x \leq b
   $$

   **Ejemplo:** El lanzamiento de un dado o el valor de un número aleatorio entre 0 y 1.

2. ### Distribución Exponencial
   - Se utiliza para modelar el tiempo entre eventos en un proceso de Poisson, es decir, describe el tiempo que transcurre hasta que ocurre un evento.
   - La función de densidad de probabilidad es:
   $$
   f(x) = \lambda e^{-\lambda x}, \quad x \geq 0
   $$

   **Ejemplo:** El tiempo entre llegadas de llamadas a un centro de atención.

3. ### Distribución Normal (Gaussiana)
   - Es una de las distribuciones más conocidas y tiene una forma de campana simétrica.
   - Está completamente definida por la **media** (\(\mu\)) y la **desviación estándar** (\(\sigma\)).
   - La función de densidad de probabilidad es:
   $$
   f(x) = \frac{1}{\sqrt{2\pi \sigma^2}} \exp \left( - \frac{(x - \mu)^2}{2\sigma^2} \right)
   $$

   **Ejemplo:** La altura de una población humana o el rendimiento de un examen estandarizado.

4. ### Distribución Log-Normal
   - Si una variable aleatoria **X** tiene una distribución normal, entonces \( e^X \) sigue una distribución log-normal.
   - La función de densidad de probabilidad es:
   $$
   f(x) = \frac{1}{x \sigma \sqrt{2\pi}} \exp \left( - \frac{(\ln(x) - \mu)^2}{2\sigma^2} \right)
   $$

   **Ejemplo:** El crecimiento del capital en inversiones.

5. ### Distribución Chi-cuadrada
   - Es una distribución especial de la familia de la distribución normal. La chi-cuadrada es la suma de los cuadrados de variables aleatorias independientes, cada una con distribución normal estándar.
   - La función de densidad es:
   $$
   f(x) = \frac{1}{2^{k/2} \Gamma(k/2)} x^{(k/2)-1} e^{-x/2}, \quad x \geq 0
   $$

   **Ejemplo:** Usada en pruebas de hipótesis como la prueba de bondad de ajuste.

6. ### Distribución de Weibull
   - Se utiliza en modelos de confiabilidad y tiempo de vida, describiendo el tiempo hasta que ocurre un evento (por ejemplo, fallo de un sistema).
   - La función de densidad es:
   $$
   f(x) = \lambda k x^{k-1} e^{-(x/\lambda)^k}, \quad x \geq 0
   $$

   **Ejemplo:** El tiempo hasta que un componente electrónico falle.

7. ### Distribución t de Student
   - Es útil para estimar la media de una población cuando el tamaño de la muestra es pequeño y la varianza es desconocida.
   - La función de densidad es:
   $$
   f(x) = \frac{\Gamma\left(\frac{\nu + 1}{2}\right)}{\sqrt{\nu \pi} \Gamma\left(\frac{\nu}{2}\right)} \left( 1 + \frac{x^2}{\nu} \right)^{-(\nu + 1)/2}
   $$

   **Ejemplo:** Usada en pruebas t para comparaciones de medias.

8. ### Distribución Gamma
   - Generaliza tanto la distribución exponencial como la chi-cuadrada. Describe el tiempo hasta que ocurren **k** eventos.
   - La función de densidad es:
   $$
   f(x) = \frac{x^{k-1} e^{-x/\theta}}{\Gamma(k) \theta^k}, \quad x \geq 0
   $$

   **Ejemplo:** El tiempo hasta que ocurra un número fijo de eventos en un proceso de Poisson.

9. ### Distribución Beta
   - Modela distribuciones continuas de probabilidades en un intervalo \([0, 1]\), como proporciones o probabilidades.
   - La función de densidad es:
   $$
   f(x) = \frac{x^{\alpha - 1} (1 - x)^{\beta - 1}}{B(\alpha, \beta)}, \quad 0 \leq x \leq 1
   $$

   **Ejemplo:** Distribución de probabilidades de una proporción, como la probabilidad de que un producto pase una prueba.

---

## Conclusión

Las distribuciones de probabilidad son fundamentales en la teoría de la probabilidad y tienen aplicaciones en diversos campos como estadística, ingeniería, economía, biología, y más. Conocerlas nos permite modelar y entender fenómenos aleatorios en diferentes contextos.

---
---