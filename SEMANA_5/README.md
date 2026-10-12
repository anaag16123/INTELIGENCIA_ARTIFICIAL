# Semana 5 - Inteligencia Artificial: Aprendizaje por Refuerzo (Q-Learning)

## Descripción
Esta carpeta contiene las actividades y laboratorios correspondientes a la Semana 5, dedicados al estudio e implementación de algoritmos de Aprendizaje por Refuerzo (Reinforcement Learning) en entornos discretos. 

Durante esta semana exploramos la formulación de problemas bajo el paradigma Agente-Entorno, el uso de la Q-Table como estructura de memoria, la regla de actualización de Q-Learning basada en Diferencias Temporales (TD), y la estrategia epsilon-greedy para balancear exploración y explotación.

---

## Contenido del Directorio

| Archivo | Descripción | Tipo |
| :--- | :--- | :--- |
| `02_qlearning_frozenlake (1).ipynb` | Taller práctico sobre el entorno FrozenLake de Gymnasium, enfocado en el entrenamiento de un agente sobre superficies resbaladizas y estados terminales. | Notebook `.ipynb` |
| `03_qlearning_taxi (1).ipynb` | Taller práctico sobre el entorno Taxi-v3, aplicando Q-Learning para navegación, recolección y entrega de pasajeros con recompensas compuestas. | Notebook `.ipynb` |
| `README.md` | Documentación explicativa y estructura de contenidos de la semana. | Documentación |

---

## Conceptos Clave Evaluados

* **Estructura Agente-Entorno:** Interacción mediante estados (S), acciones (A) y recompensas (R).
* **Q-Table:** Matriz de valor estado-acción inicializada en ceros para almacenar la utilidad esperada Q(s, a).
* **Ecuación de Actualización de Q-Learning:**
  * Calculo del TD Target: r + gamma * max(Q(s', a')).
  * Calculo del TD Error: TD Target - Q(s, a).
  * Manejo de Estados Terminales: El valor futuro esperado vale 0 en el estado final.
* **Politica Epsilon-Greedy:**
  * Probabilidad 1 - epsilon: Explotación (selección de la acción con mayor valor Q).
  * Probabilidad epsilon: Exploración (selección de una acción aleatoria).

---

## Instrucciones de Ejecución

1. Abre cualquiera de los cuadernos en Google Colab o en un entorno local con Jupyter Notebook.
2. Asegúrate de contar con las librerías `numpy`, `pandas`, `matplotlib` y `gymnasium` instaladas.
3. Ejecuta las celdas secuencialmente para entrenar a los agentes y visualizar sus curvas de aprendizaje y rendimiento acumulado.
