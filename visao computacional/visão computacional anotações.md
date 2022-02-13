VISÃO COMPUTACIONAL
•	Detecção de faces e objetos
•	Reconhecimento facial
•	Reconhecimento de objetos

a)	Classificador CASCADE 
•	Treinamento com dois conjuntos de imagens: conjunto de imagens positiva (Ex: faces) e negativas (Ex: não faces).
•	Aplicação no formato de cascata (janelas): Faz a soma de pixels branco – soma de pixels preto. Em uma imagem de 24x24 pixels, tem uma combinação de 160.000 janelas.
•	Detector de face frontal: haarcascade_frontalface_default.xml
•	Treinamento para detectar o corpo das pessoas: Fullbody.xml

Exercício: Detectando faces e o corpo inteiro das pessoas com o Open cv
•	Códigos em: https://colab.research.google.com/drive/1SdWumF--Hcvmcf2hNIcomn_SBw6FUe9F#scrollTo=QXw27smvO53r&uniqifier=2


b)	LDBH - LOCAL BINARY PATTERNS HISTOGRAM
•	Este algoritmo que faz a detecção de imagens utilizando histograma.
•	Numeração das cores dos pixels (RGB): são 255 valores (quanto mais próximo do zero temos as cores escuras, o zero é o preto. Quanto mais próximo do 255, temos cores mais claras, 255 é o branco.

c)	Rastreamento de objetos (algoritmo CRST)
•	Utiliza HOG para extrair informações úteis do objeto (histogramas)
•	 Utiliza o teste matemático de Markov para descobrir probabilidade posterior de aparecer o objeto
