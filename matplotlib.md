# matplotlib

```python
import matplotlib.pyplot as plt
```

# Tipos de Gráficos en Matplotlib

A continuación se presenta una tabla con los tipos más comunes de gráficos que se pueden realizar con la librería `matplotlib` en Python, junto con una breve descripción:

| Tipo de gráfico                     | Función principal         | Descripción                                                                 |
|------------------------------------|---------------------------|-----------------------------------------------------------------------------|
| Línea                              | `plot()`                  | Muestra series de datos o funciones matemáticas como líneas continuas.     |
| Barras verticales / horizontales   | `bar()` / `barh()`        | Representa frecuencias o cantidades mediante barras.                        |
| Histograma                         | `hist()`                  | Distribución de frecuencias de un conjunto de datos.                        |
| Dispersión                         | `scatter()`               | Muestra puntos individuales en el plano XY.                                |
| Diagrama de caja (boxplot)         | `boxplot()`               | Resume la distribución con mediana, cuartiles y valores atípicos.          |
| Gráfico de violín                  | `violinplot()`            | Variante del boxplot que incluye densidad de probabilidad.                 |
| Gráfico escalonado                 | `step()`                  | Representa funciones escalonadas (útil para CDFs).                          |
| Barras de error                    | `errorbar()`              | Muestra valores con sus respectivas barras de incertidumbre.               |
| Gráfico de tallo y hoja            | `stem()`                  | Representa puntos con líneas verticales (útil para series discretas).      |
| Gráfico circular (pie chart)       | `pie()`                   | Distribución de categorías como proporciones de un círculo.                |
| Gráfico de densidad hexagonal      | `hexbin()`                | Densidad de puntos usando celdas hexagonales.                              |
| Campo de vectores                  | `quiver()`                | Representa vectores con flechas (dirección y magnitud).                    |
| Líneas de flujo                    | `streamplot()`            | Muestra flujos en campos vectoriales.                                      |
| Coordenadas polares                | `polar()`                 | Gráfico basado en ángulo y radio.                                          |
| Gráfico de radar                   | `plot()` en ejes polares  | Usado para comparar múltiples variables (se necesita configuración extra). |
| Imagen / matriz de calor           | `imshow()` / `matshow()`  | Representa matrices o imágenes como mapas de color.                        |
| Contornos                          | `contour()` / `contourf()`| Muestra niveles o curvas de igual valor (funciones de dos variables).      |
| Gráficos en 3D                     | `Axes3D` de `mpl_toolkits`| Superficies, líneas y dispersión en 3D.                                    |

> 💡 Muchos de estos gráficos pueden combinarse en una misma figura o subfiguras (`subplots`), lo que permite construir visualizaciones ricas y personalizadas.

# Principales Objetos de Matplotlib

Matplotlib está compuesto por múltiples clases y módulos. Aquí tienes los objetos más importantes:

---

## 🎨 Figura y Ejes

| Objeto | Descripción |
|--------|-------------|
| `Figure` | Contenedor principal de toda la imagen o figura. Puede contener múltiples `Axes`. |
| `Axes` | Área donde se dibujan los datos (subgráfico). Una figura puede tener varios `Axes`. |
| `Axis` | Representa un eje individual dentro de un `Axes` (X o Y). |

---

## 📐 Elementos de dibujo

| Objeto | Descripción |
|--------|-------------|
| `Line2D` | Representa una línea en el gráfico. |
| `Patch` | Formas geométricas como rectángulos, círculos, polígonos (`Rectangle`, `Circle`, etc.). |
| `Text` | Texto que se muestra en el gráfico (títulos, etiquetas, anotaciones). |
| `Collection` | Conjunto de objetos como líneas o polígonos, útil para eficiencia. |

---

## 🖌️ Artistas

| Objeto | Descripción |
|--------|-------------|
| `Artist` | Clase base de todos los objetos visibles. Todo en Matplotlib hereda de `Artist`. |
| `Text`, `Line2D`, `Patch`, `Image` | Todos estos son artistas. Puedes agregarlos manualmente a `Axes` o `Figure`. |

---

## 🧰 Backends y Canvas

| Objeto | Descripción |
|--------|-------------|
| `FigureCanvas` | Interfaz entre la figura y el backend de renderizado (por ejemplo, Agg, TkAgg, etc.). |
| `Renderer` | Se encarga del renderizado final en píxeles o vectores. |

---

## 🧩 Otros módulos útiles

| Módulo | Uso |
|--------|-----|
| `matplotlib.pyplot` | API de alto nivel basada en estado (como MATLAB). Muy usada en notebooks. |
| `matplotlib.style` | Aplicar estilos visuales fácilmente (`style.use('ggplot')`). |
| `matplotlib.ticker` | Control preciso del formato de los ticks. |
| `matplotlib.dates` | Manejo de fechas y tiempos en ejes. |

---

## 🧠 Notas

- `Axes` es el lugar donde sucede la magia: líneas, barras, imágenes, textos, etc.
- La mayoría de gráficos complejos se logran manipulando objetos directamente (`Figure` → `Axes` → `Artist`).
- Para aplicaciones avanzadas, se recomienda usar la API orientada a objetos en lugar de `pyplot`.

