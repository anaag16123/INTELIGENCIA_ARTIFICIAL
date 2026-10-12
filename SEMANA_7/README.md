# Semana 7 - Inteligencia Artificial: Redes Neuronales Profundas con Keras 3

## Descripción
Esta carpeta contiene los materiales, desafíos y talleres prácticos correspondientes a la Semana 7. En este módulo introducimos el aprendizaje profundo (Deep Learning) utilizando la biblioteca Keras 3 con backend de TensorFlow/PyTorch/JAX. 

Durante la semana se abordó el diseño, entrenamiento y evaluación de Perceptrones Multicapa (MLP) y arquitecturas feedforward aplicadas a problemas de clasificación multiclase sobre datasets canónicos de visión por computadora y reconocimiento facial.

---

## Contenido del Directorio

| Archivo / Notebook | Descripción | Tipo |
| :--- | :--- | :--- |
| `YourFirstDeepNN_FashionMNIST_Keras3_(2).ipynb` | Taller introductorio de Deep Learning para la construcción, entrenamiento y evaluación de una red neuronal profunda sobre el conjunto de datos FashionMNIST. | Notebook `.ipynb` |
| `Challenge_Keras3_CIFAR10_Grayscale.ipynb` | Desafío práctico de clasificación multiclase sobre el dataset CIFAR-10 preprocesado en escala de grises. | Notebook `.ipynb` |
| `Challenge_Keras3_OlivettiFaces.ipynb` | Desafío avanzado sobre el dataset Olivetti Faces para tareas de reconocimiento facial utilizando arquitecturas totalmente conectadas. | Notebook `.ipynb` |
| `README.md` | Documentación estructurada de la semana y resumen de contenidos del directorio. | Documentación |

---

## Conceptos Clave Tratados

* **Fundamentos de Redes Neuronales:**
  * Estructura de capas: `Sequential`, capas densas (`Dense`) y capas de aplanado (`Flatten`).
  * Funciones de activación: ReLU, Softmax y Sigmoide.
  * Inicialización de pesos y sesgos.
* **Flujo de Entrenamiento en Keras 3:**
  * Compilador de modelos: Funciones de pérdida (`SparseCategoricalCrossentropy`, `CategoricalCrossentropy`) y optimizadores (`Adam`, `SGD`).
  * Configuración de métricas de desempeño (`accuracy`).
  * Ajuste mediante `model.fit()` con validación cruzada/split y uso de callbacks (`EarlyStopping`).
* **Preprocesamiento e Ingeniería de Datos:**
  * Normalización de píxeles ($[0, 255] \to [0, 1]$).
  * Conversión de canales de color (RGB a Grayscale para CIFAR-10).
  * Reshaping de tensores de entrada para capas totalmente conectadas.
* **Evaluación de Modelos:**
  * Análisis de curvas de pérdida y exactitud (`loss` vs `val_loss`, `accuracy` vs `val_accuracy`).
  * Diagnóstico de sobreajuste (Overfitting) y bajo ajuste (Underfitting).

---

## Requisitos e Instalación

Para ejecutar los cuadernos de esta semana, instala las librerías necesarias mediante:

```bash
pip install keras tensorflow numpy pandas matplotlib scikit-learn
