# Caminata-aleatoria-en-1D

El programa simula partículas que realizan una marcha aleatoria sobre el eje x, donde cada paso tiene longitud fija a y dirección aleatoria (derecha + o izquierda - con igual probabilidad). Se estudian las propiedades estadísticas de la posición final después de N pasos.
El proyecto está estructurado de la forma: 
random_walk/
├── random_walk_simulation.py  # Código principal de simulación
├── analysis.py               # Análisis de resultados y gráficas
└── README.md                 # Este archivo

# Cómo ejecutar
1. Simulación básica con histograma
Ejecute el primer programa para simular caminatas aleatorias y generar un histograma: python random_walk_histogram.py
2. Análisis de 〈x²〉 vs N
Ejecute el segundo programa para analizar la relación 〈x²〉 ∝ N: python random_walk_analysis.py

* Resultados esperados
-Para el primer programa (histograma):
Media cercana a 0
Varianza cercana a N
Histograma que se ajusta a la campana de Gauss

-Para el segundo programa (análisis):
〈x〉 ≈ 0 para todos los N
〈x²〉 ∝ N con pendiente ≈ 1.0
Constante de difusión D ≈ 0.5

Considere los parámetros ajustables que puede modificar en el código:

N: Número de pasos por caminata
num_simulations: Número de repeticiones
N_values: Valores de N para el análisis

# Interpretación de resultados
Teorema del límite central: El histograma debe coincidir con la distribución gaussiana

Difusión: 〈x²〉 crece linealmente con N, confirmando 〈x²〉 = 2DN

Constante D: D = a²/2τ = 0.5 cuando a = 1 y τ = 1

# Debe considerar que los resultados pueden variar ligeramente debido a la naturaleza aleatoria de las simulaciones, pero deberían ser consistentes con las predicciones teóricas.
