## Programaciones para el desarrollo de la Tarea 1 del Módulo VII del Diplomado en Introducción Analítica a la Ciencia de Datos

Módulo 7: Optimización en aprendizaje de máquina
Tarea 1
Julio 2026

# El entregable consiste en:
- Un reporte breve en un notebook reproducible por cada ejercicio que incluye:
1. Descripción del problema
2. Metodología
3. Resultados (tablas y gráficas)
4. Conclusiones

# Son tres optimizaciones, una por cada metodología:
1. SGD y alguna de sus variantes
2. SGD en Scikit-learn
3. SGD y sus variantes en redes neuronales
    3.1. SGD y sus variantes para clasificación
    3.2. SGD y sus variantes en redes neuronales para regresión

# Base de imágenes seleccionada
BloodMNIST es un dataset para análisis médico y visión por computadora: son 28x28 píxeles en escala de grises/RGB (imágenes médicas comprimidas al estilo MNIST) con 8 clases de células sanguíneas periféricas (basófilos, eosinófilos, eritroblastos, ig, linfocitos, monocitos, neutrófilos y plaquetas).
Disponible mediante la librería oficial medmnist

# Detalles de cada metodología:

1. SGD y alguna de sus variantes:
   
    Implementar SGD y una de sus variantes (SGD + momentum, AdaGrad,
    RMSProp, Adam) para la pérdida cross entropy y usarlo en un problema de
    regresión logística con un dataset de imágenes (MNIST, Fashion MNIST,
    CIFAR 10 , etc)


2. SGD en Scikit-learn
    Realizar una revisión de la documentación de scikit-learn sobre el
    uso de descenso de gradiente estocástico, tanto para regresión como para clasificación.
    En particular, deberán revisar las clases SGDRegressor y SGDClassifier.

    El objetivo del proyecto es explicar cómo se implementa SGD en scikit-learn,
        - Qué funciones de pérdida permite usar,
        - Qué parámetros son importantes y
        - Cómo se relaciona su funcionamiento con lo estudiado en clase.

    Hacer un ejemplo de uso con datos reales:
       a) Revisar la documentación oficial de: SGDRegressor y SGDClassifier.
        
       b) Explicar el papel de los siguientes elementos:
            función de pérdida; 
            tasa de aprendizaje;
            regularización; 
            número de épocas;
            escalamiento de variables;
            criterio de parada.
        
       c) Aplicar SGDRegressor a un problema de regresión con una base de
        datos real. Una opción recomendada es la base California Housing,
        disponible en scikit-learn, o bien, aplicar SGDClassifier a un problema de clasificación con una base de datos real. 
        Una opción recomendada es la base Breast Cancer Wisconsin, también disponible en scikit-learn.
        
       d) Comparar los resultados con un método de referencia, por ejemplo:
        regresión lineal ordinaria para el problema de regresión;
        regresión logística para el problema de clasificación.
    
4. SGD y sus variantes en redes neuronales, escoger
uno de los siguientes:
3.1. SGD y sus variantes para clasificación
Usar redes neuronales para un problema de clasificación de imágenes. El
objetivo es comparar el comportamiento de diferentes optimizadores en el
entrenamiento de una misma arquitectura de red neuronal.

3.2 Actividades

a) Construir una red neuronal convolucional sencilla para clasificación de
imágenes.

b) Mantener fija la arquitectura de la red y cambiar únicamente el optimizador.

c) Comparar, según la paquetería utilizada, algunos de los siguientes métodos:

- SGD clásico;
- SGD con momentum;
- SGD con momentum de Nesterov;
- AdaGrad;
- RMSProp;
- Adam;
- AdamW, si está disponible.

d) Reportar la evolución de la función de pérdida durante el entrenamiento.

e) Reportar la exactitud en entrenamiento y validación.

f) Analizar si los optimizadores adaptativos convergen más rápido o si
logran mejor desempeño final.

## Preguntas a responder
a) ¿Qué optimizador reduce más rápido la función de pérdida?

b) ¿El optimizador con mejor desempeño en entrenamiento también es el
mejor en validación?

c) ¿Qué método parece más sensible a la elección de la tasa de aprendizaje?

3.2. SGD y sus variantes en redes neuronales para regresión
Usar redes neuronales para resolver un problema de regresión con datos reales. 
El objetivo es comparar el comportamiento de diferentes optimizadores en el entrenamiento de una red neuronal para regresión.

3
# Actividades
a) Explorar la base de datos seleccionada.

b) Separar los datos en entrenamiento, validación y prueba.

c) Estandarizar las variables explicativas.

d) Construir una red neuronal multicapa sencilla.

e) Entrenar la misma arquitectura usando diferentes optimizadores:
    SGD;
    SGD con momentum;
    AdaGrad;
    RMSProp;
    Adam;
    AdamW, si está disponible.

f) Comparar los métodos usando métricas de regresión como:
    MSE;
    MAE;
    RMSE;
    R2

g) Graficar la pérdida de entrenamiento y validación para cada optimiza-
dor.

Preguntas
a) ¿Qué optimizador converge más rápido?
b) ¿Qué optimizador logra menor error de validación?
c) ¿Hay evidencia de sobreajuste?
d) ¿Cómo afecta la tasa de aprendizaje al desempeño?
