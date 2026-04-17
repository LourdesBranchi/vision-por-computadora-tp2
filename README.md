# Trabajo Práctico 2 – Visión por Computadora

## Descripción

En este trabajo práctico se implementa un detector de máximo enfoque sobre un video, aplicando técnicas de análisis espectral similares a las utilizadas por las cámaras digitales modernas.

El objetivo es:

* Implementar el algoritmo de medición de nitidez propuesto en el paper *"Image Sharpness Measure for Blurred Images in Frequency Domain"*
* Aplicarlo frame a frame sobre un video para detectar el punto de máximo enfoque de manera automática
* Comparar el comportamiento de la métrica sobre el frame completo vs. una ROI central

## Contenido

### Notebook

El desarrollo completo, junto con los resultados, visualizaciones y conclusiones, se encuentra en el siguiente notebook:

* `GonzalezBranchiLourdes-TP2_VPC.ipynb`

### Estructura del notebook

1. **Lectura del video**: carga y descripción del archivo `focus_video.mov`
2. **Algoritmo FM**: implementación comentada paso a paso de la métrica de calidad de imagen
3. **Inspección de cómo funciona el algoritmo**: visualización de la Transformada de Fourier, el espectro centrado y la máscara de umbral para el primer y último frame
4. **Experimento 1**: cálculo de FM frame a frame sobre el frame completo
5. **Experimento 2**: cálculo de FM frame a frame sobre una ROI central del 5% del área
6. **Comparación** – curvas y tabla comparativa entre ambos experimentos

## Ejecución

Colocar el archivo `focus_video.mov` en el mismo directorio que el notebook, luego abrir el notebook y ejecutar las celdas en orden. De todas formas, se encuentra ejecutado el notebook completo.

## Autor

Lourdes Gonzalez Branchi
