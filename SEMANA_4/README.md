# 🕹️ Semana 4 — Inteligencia Artificial: Toma de Decisiones con MDPs

## 📌 ¿De qué trata esta semana?
En este módulo dejamos atrás la búsqueda a ciegas y nos adentramos en el mundo de los **Procesos de Decisión de Markov (MDP)**. Aquí estudiamos cómo un agente inteligente puede tomar decisiones óptimas cuando el entorno tiene incertidumbre o probabilidad de fallo (¡como un robot en un piso resbaloso o navegando en un almacén!).

Analizamos los componentes clave de la tupla MDP $\langle S, A, P, R, \gamma \rangle$, las Ecuaciones de Bellman y la diferencia entre valorar el presente vs. el futuro descontado.

---

## 🛠️ Contenido del Repositorio

| Archivo | Descripción | Tipo |
| :--- | :--- | :--- |
| `03_lab_warehouse_mdp_estudiantes_(1).ipynb` | Taller práctico guiado sobre la simulación de un robot en un almacén (*Warehouse*) navegando entre metas y obstáculos. | Notebook `.ipynb` |
| `README.md` | Guía de navegación y resumen conceptual de la semana. | Documentación |

---

## 💡 Conceptos Clave para Tener en Cuenta

* **Estados ($S$) y Acciones ($A$):** Lo que el agente ve y lo que puede hacer.
* **Transiciones Estocásticas $P(s' \mid s, a)$:** La probabilidad de terminar en un estado $s'$ tras intentar moverse.
* **Factor de Descuento ($\gamma$):**
  * Si $\gamma \to 0$, al agente solo le importa la recompensa inmediata.
  * Si $\gamma \to 1$, el agente planifica pensando en el largo plazo.
* **Propiedad de Markov:** El futuro solo depende del estado presente, no de cómo se llegó hasta ahí.

---

## 🚀 ¿Cómo ejecutar la práctica?
1. Abre el cuaderno en **Google Colab** o tu entorno local de Jupyter.
2. Asegúrate de tener instalados `numpy`, `pandas` y `matplotlib`.
3. Corre las celdas en orden para verificar la dinámica del entorno del almacén y analizar las políticas de movimiento óptimas.
