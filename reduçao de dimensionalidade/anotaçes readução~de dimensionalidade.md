REDUÇÃO DE DIMENSIONALIDADE
Serve para diminuir a quantidade de componentes.

a)	PCA: Utiliza-se para analisar e descobrir os principais componentes. Existe diferença entre fazer uma seleção e uma extração de características. Em uma seleção, os principais atributos são selecionados e constrói-se um novo modelo utilizando-se estes atributos. Com a extração, se faz uma análise dos melhores atributos e criam-se novos, a partir de uma compactação, ou seja, uma combinação de atributos.
É um algoritmo de aprendizagem não supervisionada (não utiliza classes).
Identifica a correlação entre as variáveis (uma forte correlação pode reduzir a dimensionalidade).

b)	LDA: encontra os componentes principais e os eixos que maximizam a separação entre as múltiplas classes. É um algoritmo de aprendizagem supervisionada (encontra e utiliza classes).

O PCA e o LDA são utilizados quando os dados podem ser linearmente separáveis.

c)	PCA Kernel: Utilizado para problemas mais complexos. É uma versão do PCA em que os dados são mapeados para uma dimensão maior (aumenta a dimensão) usando o kernel trick (para dados não linearmente separáveis). Após extrai-se os principais componentes.

Obs: O código está me construção, logo vai ser revisado... existem erros na aplicação de algumas células do PCA e Kernel