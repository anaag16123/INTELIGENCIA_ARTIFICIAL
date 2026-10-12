# Semana 6 - Inteligencia Artificial: Desafío de Clasificación y Proyectos de NLP

## Descripción
Esta carpeta contiene los materiales, proyectos y desafíos correspondientes a la Semana 6. Durante este módulo nos enfocamos en el desarrollo de soluciones avanzadas combinando técnicas de Machine Learning, Procesamiento de Lenguaje Natural (NLP), métricas de evaluación de modelos y despliegue interactivo con Streamlit.

---

## Contenido del Directorio

| Directorio / Archivo | Descripción | Tipo |
| :--- | :--- | :--- |
| `challenge/` | Carpeta contenedora del reto práctico de clasificación, modelos entrenados y módulos de análisis de desempeño. | Directorio |
| `README.md` | Documentación estructurada de la semana y resumen de contenidos del directorio. | Documentación |

---

## Temas y Desarrollos Evaluados

* **Módulos de Clasificación:** Entrenamiento, optimización e interpretación de modelos en problemas de clasificación supervisada.
* **Procesamiento de Lenguaje Natural (NLP):**
  * Tokenización visual por palabras, caracteres y subpalabras (n-grams).
  * Construcción de matrices Bag of Words (BoW) y representación vectorial.
  * Evaluación de métricas de similitud (Similitud Coseno sobre embeddings y vectores de frecuencia).
* **Integración con Modelos de Lenguaje (LLMs):**
  * Integración de la API de Groq para generación de texto dinámico.
  * Comparativa de respuestas variando la temperatura (exploración vs. determinismo).
* **Análisis de Métricas Textuales:**
  * Evaluación de legibilidad (Flesch Reading Ease, Gunning Fog Index).
  * Diversidad léxica (Type-Token Ratio - TTR), cohesión gramatical y estructura sintáctica.

---

## Requisitos e Instalación

Para ejecutar las aplicaciones e interfaces desarrolladas durante esta semana, instala las dependencias necesarias:

```bash
pip install streamlit groq scikit-learn numpy pandas pillow textstat

