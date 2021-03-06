CÁLCULOS DE DISTRIBUIÇÃO NORMAL - "NORMALIDADE": Modela o que ocorre normalmente em um cenário real.

...........................................................................................................................
TESTE DE HIPÓTESES - INTERVALOS DE CONFIANÇA

Exemplo: Se temos 3 preços: 15, 20 e 25: podemos dizer que o intervalo de confiança está entre 15 e 25. 
Os testes de hipóteses servem para identificar sim ou não (confirmar ou rejeitar uma afirmação) - validação de hipóteses.
Os testes de hipóteses são aplicados em AMOSTRAS.

*Hipótese nula (H0): Dado que já existe (afirmação que já existe). 
A ideia é presumir que a afirmação é verdadeira até "que se prove o contrário"

*Hipótese alternativa (H1): tudo que é diferente da hipótese nula.

*Alpha (confiabilidade): É a probabilidade de rejeitar a hipótese nula (nível de significância) - Quanto menor, mais seguro.
Em geral, o nível de significância é 0,01 (99% de confiabilidade, ou seja, 1% de chance de rejeitar a hipótese nula) ou 0,05.

*Valor de p (p-value):
 a) Se p-value >=alpha: Não rejeita H0
 b) Se p-value < alpha: rejeita H0 (temos evidência)

*Erro tipo I: rejeitar H0 quando não deveria
*Erro tipo II: não rejeitar a hipótese nula  quando deveria ter rejeitado 

Calculando: Teste de Hipótese Z
Z= média do experimento novo (H1) - média antiga (H0) / erro padrão

(standard erro ou erro padrão: desvio padrão/raiz quadrada de n)

Case: Registros de altura (cm)
média H1 = 164,02
média H0 = 159,25
Desvio padrão H1 = 14,05
n = quantidade de registros de altura (100)
alpha = 0,05 (5%)

Z = 164,02 - 159,25 / 1,4 = 3,39
Observar o valor correspondente na tabela Z: 0,99965

Valor de p = 1 - 0,999 = 0,001
(O valor de p é menor que alpha, isso indica que devemos rejeitar H0 e aceitar H1)
A média atual das alturas será 164,02.

...............................................................................
TESTE ANOVA: Análise de variação (teste de hipóteses) - Busca valores da tabela F

*   Indica se há ou não diferença estatística entre os grupos.
*   É adequado quando as amostras são independentes, para fazer a comparação entre 3 ou mais grupos.
*   É possível utilizar "mesclando" variáveis quantitativas (numéricas) e qualitativas (categóricas).
*   Para a realização desse cálculo necessário que a distribuição seja normal.
*   H0 indica que não há diferença estatística e o H1 indica que há diferença estatística.

Case: Testando a variância de altura (cm) de 3 grupos diferentes de pessoas: Grupos A, B, C
Média de altura dos grupos: A = 151, B = 152, C = 156 (cada grupo possui 5 registros)

Passo 1: Média geral = 153

Passo 2: Eleva-se os elementos ao quadrado:
A= (151-153)=4
B= (152-153)=1
C= (156-153)=9
Total = 14

Passo 3: SSG (sum of square group): Total x número de registros em cada grupo: 14 x 5 = 70

Passo 4: DFG (grau de liberdade - degrees of freedom groups): Número de grupos - 1: 3-1 = 2

Passo 5: SSE (Sum of squares error) 
Quadrado do erro: (valor do registro - média do grupo) ao quadrado
Este passo é calculado para cada regitro e depois realiza-se a soma dos valores do grupo
Exemplo: Grupo A: 165, 152, 143, 140, 155 = Média 151
                  (165-151) ao quadrado=196
                  (152-151) ao quadrado=1
                  (143-151) ao quadrado=64
                  (140-151) ao quadrado=121
                  (155-151) ao quadrado=16
                  Somatório (A)= 398
                  Somatório (B)= 1002
                  Somatório (C) = 106
                  SSE = 1506
                  DFE (grau de liberdade do erro): (linhas - 1) x grupo = (5-1)x3=12

Passo 6: Cálculo de F (finalidade: comparação com a Tabela F)
                    F= (SSG/DFG)/(SSE/DFE)
                    F= (70/2)/(1506/12)=35/125,5=0,27
CONSULTANDO A TABELA: F crítrico (utiliza-se a tabela com alpha 0,05 - 95% de confiança)
F crítico: Na tabela F, encontra-se a intersecção entre os dois graus de liberdade calculados: 2 e 12 = 3,88

Interpretando o cálculo: Verifica-se se F fica entre o valor de 0 e Fcrítico (3,88). 
Se o valor de F fica entre os pontos 0 e 3,88, não há diferença estatística enttre os grupos.
Se o valor ficar a direita deste intervalo de 0 e 3,88, há diferença estatística.
Como o F calculado foi 0,27, não existe diferença estatística entre a média da altura dos grupos A,B,C.

Nota: Se houver diferença estatística entre os grupos, aplica-se o Teste T, que mede a diferença entre os grupos, por exemplo, entre o grupo A e B, entre o grupo B e C...
         