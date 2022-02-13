APRENDIZAGEM DE MÁQUINA: APRENDIZAGEM POR REFORÇO – ALGORITMO QLEARNING
*Ambiente gym
*Define-se o objetivo e as recompensas
*Não é necessária uma base de dados

<img src="img/QL1.png" alt="QLearning">

O agente vai seguir o caminho que possui maior valor (maior recompensa).

<img src="img/QL2.png" alt="Ambiente – ações – estado/recompensa">

Conceitos: EXPLORATION - o agente tem uma probabilidade alta de seguir por um caminho mas, pode explorar o ambiente se for necessário – essa abordagem é mais interessante, porque permite a aprendizagem para transpor obstáculos; EXPLOTATION - 100% de chance de seguir um caminho.

<img src="img/QL3.png" alt="Markov Decision Process (MDP)">

Q-Learning: Fórmula matemática para escolher as melhores ações. Quanto maior o valor de Q, melhor a solução (é uma métrica que demonstra a qualidade da ação).

<img src="img/QL4.png" alt="Valores de Q">

Diferença temporal: Executa vários episódios. No final do treinamento, os valores devem estar armazenados, para avaliar a qualidade das ações. 

<img src="img/QL5.png" alt="diferença temporal">


Exercício:
https://colab.research.google.com/drive/1Cwe3qKtdiKo6KVBqBBnnZJYgXSGnpeIA#scrollTo=basKM7zoqn9D
