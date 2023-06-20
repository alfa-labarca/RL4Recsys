# RL4Recsys

## Procesos

1. Se generó un environment de Reinforcement Learning para recomendación secuencial.
  1. Se entrenó sobre un subconjunto del dataset RetailRocket con 700 usuarios, donde cada uno tiene máximo 3 eventos en el set de testeo.

2. Al entrenar modelos más grandes, se notó que a medida que el entrenamiento continua, más largo es cada episodio, lo cual es contrario a lo esperado.
3. Se entrenaron diversos modelos intentando mejorar este resultado, sin ningún resultado convincente.

## Descubrimientos
1. En el entrenamiento, se testeó sobre los datos de testeo y fue comparado con un agente aleatorio y most popular. Sobre métricas de ranking, diversidad y novelty.
   1. La distancia en la novelty se calculó utilizando el árbol de categorías de RetailRocket.
   2. Se comparó el rendimiento de un agente entrenado por 1000 episodios con gamma=0.99 y gamma=0.8 y los resultados mostraron que en términos de recompensa, el agente con gamma=0.99 obtuvo mejor recall@1, mostrando un salto en su rendimiento alrededor del episodio 300.
   3. En términos de novelty, los agentes DQN comienzan con términos más obscuros en las primeras recomendaciones.
2. 

## Pasos futuros

## Ideas
