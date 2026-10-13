# Semana 8 - Inteligencia Artificial: Aprendizaje por Transferencia (Transfer Learning) y Ajuste Fino (Fine-Tuning)

## Descripción
Esta carpeta contiene los recursos, laboratorios y proyectos correspondientes a la Semana 8. En esta unidad exploramos el paradigma de Transfer Learning aplicado a Visión por Computadora (Computer Vision), utilizando redes neuronales convolucionales (CNN) preentrenadas sobre conjuntos de datos masivos como ImageNet.

Durante la semana se abordó el flujo completo de Fine-Tuning: desde la extracción de características con capas congeladas (*Feature Extraction*), la descongelación selectiva de capas convolucionales profundas, el entrenamiento diferencial con tasas de aprendizaje reducidas, hasta el análisis riguroso de errores de clasificación en datasets de dominio específico.

---

## Contenido del Directorio

| Directorio / Archivo | Descripción | Tipo |
| :--- | :--- | :--- |
| `transfer_learning/` | Carpeta contenedora de los cuadernos de trabajo, experimentos de fine-tuning y módulos de clasificación. | Directorio |
| `README.md` | Documentación estructurada de la semana y resumen de contenidos del directorio. | Documentación |

---

## Conceptos Clave Tratados

* **Estrategias de Transfer Learning:**
  * **Feature Extraction (Base Congelada):** Uso de la arquitectura base preentrenada (`EfficientNetB0`) con pesos congelados (`trainable = False`), adaptando únicamente la cabeza de clasificación final.
  * **Fine-Tuning (Ajuste Fino):** Descongelación de las capas superiores del backbone (`N_UNFROZEN`) y entrenamiento fino utilizando optimizadores con tasas de aprendizaje muy bajas ($10^{-5}$).
  * **Comparativa vs. Entrenamiento desde cero:** Ventajas en aceleración de convergencia y mitigación del sobreajuste en datasets pequeños.
* **Técnicas de Regularización y Manejo de Datos:**
  * Configuración de callbacks como `EarlyStopping` monitoreando la pérdida de validación (`val_loss`).
  * Data Augmentation para incrementar la variabilidad del conjunto de entrenamiento.
* **Análisis de Errores y Diagnóstico:**
  * Identificación de patrones de falla en imágenes ambiguas, con oclusiones, sesgos de fondo o clases visualmente similares.
  * Evaluación de impacto del Fine-Tuning en métricas globales e individuales por clase.

---

## Requisitos e Instalación

Para ejecutar los experimentos de esta semana, instala las dependencias requeridas mediante:

```bash
pip install keras tensorflow numpy pandas matplotlib pillow scikit-learn
