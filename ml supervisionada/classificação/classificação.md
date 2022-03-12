APRENDIZAGEM SUPERVISIONADA: CLASSIFICAÇÃO

•	Parte prática: https://colab.research.google.com/drive/1qXAzDIOFjyuNCSTsib16GL2D1JHP4EAz#scrollTo=g3vWK9OO34Zk

1.	Pré-processamento e preparação de bases de dados para classificação:
•	Importação de bibliotecas básicas (pandas, numpy, seaborn, matplotlib.pyplot, plotly.express)
•	Tratamento de valores faltantes e inconsistentes
•	Exploração e visualização dos dados
•	Divisão entre previsores e classes
•	OneHotEncoder: Para transformar categorias (strings) em numérica
•	Escalonamento (padronização de escala entre as variáveis)

2.	Aprendizagem bayesiana (algoritmo Naive Bayes):
•	Abordagem probabilística
•	Analisa uma base de dados histórica, a partir dela construir uma tabela de classificação (estatística).
•	A correção Laplaciana é utilizada para corrigir a tabela, adicionando registros, para não encontra nenhum registro como zero.
•	Utilizando o conceito de raio para descobrir se a bolinha é vermelha ou azul.

<img src="img/01%20Naive%20Bayes.png" alt="Modelo de Naive Bayes">

3.	Aprendizagem por árvores de decisão (algoritmo básico de árvores e Random Forest):
As árvores de decisão são modelos práticos, que organizam os atributos, analisam a base de dados original e colocam os atributos mais importantes no topo. 
Os atributos ficam nos vértices e nos “ramos” ficam os valores. As classes são as respostas. Este método apresenta as árvores de decisão como funções, que são treinadas de acordo com regras de classificação. 
As árvores de decisão classificam instâncias, ordenando da raiz para algum nó da folha. 
Exemplo: Uma árvore de decisão para descobrir se o cliente vai pagar o empréstimo ao banco ou não.

<img src="img/02%20-%20arvore%20de%20decisao.png" alt="Árvore de decisão">

Percebe-se que o atributo mais importante é a renda, seguido pelo histórico de crédito e dívidas. Se a renda for <15, o risco é alto (o cliente não via pagar). Se a renda está entre 15 e 35 ou >35, analisa-se o segundo atributo (histórico). A classe (resposta) baixo, ou seja, o cliente vai pagar a dívida , está disposta para aqueles que possuem renda acima de 35 e histórico de crédito bom ou deconhecido.
Os atributos mais importantes são encontrados pelo algoritmo através de dois cálculos: entropia e ganho de informação:

<img src="img/03%20-%20entropia.png" alt="Fórmula da Entropia">

•	Random Forest: Apresenta como vantagem a aprendizagem em conjunto, são vários algoritmos que juntos constroem um algoritmo mais forte. Para responder, usa a média (regressão) ou a maioria dos votos (classificação). Escolhe de forma aleatória K atributos para comparação da métrica de pureza/impureza (impureza de gini/entropia). Exemplo: se k=3, a árvore apresenta 3 atributos (que fazem comparações de forma aleatória/randômica).

<img src="img/04%20-%20random%20forest.png" alt="Random Forest">

4.	Aprendizagem por regras:
•	Trabalha com atributos categóricos
•	Algoritmo OneR (se...então)
•	Algoritmo PRISM (se=)

5.	Aprendizagem baseada em instâncias: 
•	Algoritmo kNN (k é o número de vizinhos mais próximos). 
•	Calcula a distância euclidina (DE): Quanto menor a distância (DE) entre os “vizinhos” melhor, porque os registros são mais parecidos. 

<img src="img/05%20-%201DE.png" alt="Distribuição Euclidiana">  

•	Não constrói modelo. Este algoritmo, armazena um modelo de comparação de distância (lazi=preguiçoso).
•	 Ex: Sistema de recomendação

6.	Regressão logística:
•	É um método preditivo de classificação (utiliza técnicas de estimativas de probabilidade).
•	Constrói uma linha (em formato s), utilizando a função sigmoide. É necessário fazer o encode (transforma o atributo em valor numérico – parâmetros). Utiliza-se o algoritmo de descida de gradiente para encontrar o melhor conjunto dos parâmetros b (mínimo custo, menor erro possível e ajusta o processo a partir de várias repetições). 
•	A fórmula sempre oferece como resultado os valores positivos (entre 0 e 1) e, transforma-se em percentual. Primeiro calcula-se a equação da reta e a transformação “logit”.

<img src="img/06%20-%20sigmoide.png" alt="Sigmoide">  

7.	Máquinas de vetores de suporte (SVM):
•	Em geral oferece melhores resultados.
•	Encontra retas: margem máxima (distância entre a linha e o vetor: ponto mais próximo)
•	Generaliza melhor os registros que a regressão linear (porque os vetores de suporte constroem o melhor hiperplano)
•	Precisa configurar: cost (c mais alto, melhor) e kernel. 
•	Slack: transforma 2D em 3D (aprende melhor os conceitos)

8.	Redes neurais artificiais:
•	Deep learning, scikit learn
