# Redes Neurais

## O que são Redes Neurais?
Redes neurais são sistemas de computação com nós interconectados que funcionam como os neurônios do cérebro humano. Usando algoritmos, elas podem reconhecer padrões escondidos e correlações em dados brutos, agrupá-los e classificá-los, e – com o tempo – aprender e melhorar continuamente.
O primeiro tijolo na construção de uma rede neural são os neurônios. Um neurônio é como uma função, aceita algumas entradas e devolve algumas saídas.

<img src='https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/Neural_network.svg/1200px-Neural_network.svg.png' width=350></img>

Neurônios que podem ser usados em redes neurais:

- <strong><h3> Perceptron (Frank Rosenblatt - 1957) </h3></strong>
  - Formado por N entradas e 1 saída
  - É um classificador binário linear, ou seja, resolve problemas de classificação cuja a saída é categórica. Mas, pode ser adaptado para efetuar regressão       linear
  - Linear quer dizer que o Perceptron só resolve um problema de classificação binária, separaveis por uma reta
  - O problema de classificação tem que ser binário, ou seja, um problema de duas classes
  - Aprende através da Perceptron Rule. Aprendizado online, atualiza os pesos toda vez que recebe uma amostra (dado)

- <strong><h3> Adaline </h3></strong>
  - Implementação melhorada do Perceptron
  - Função de ativação: linear (+ steps)
  - N entradas 1 saída
  - Por definição, é um classificador binário linear, mas também pode ser adaptado para efetuar regressão linear
  - A grande diferença entre o Perceptron e o Adaline, é que o Adaline sabe o 'quanto' errou, enquanto que o Perceptron sabe apenas que errou
  - Pode-se aplicar o Gradiente Descendente
  - Aprende através da Delta Rule. Aprendizado online, atualiza os pesos toda vez que recebe uma amostra (dado)

- <strong><h3> Sigmoid </h3></strong>
  - Função de ativação: sigmoid
  - Função derivável em todos os pontos
  - Função de custo: entropia cruzada (cross entropy)
  - N entradas 1 saída
  - Por definição é um classificador binário
  - Pequenas mudanças nos parâmetros, causam pequenas mudanças na saída
  - Também sabe o 'quanto' errou, assim como o Adaline

## Para que serve uma Rede Neural?
As redes neurais refletem o comportamento do cérebro humano, permitindo que programas de computador reconheçam padrões e resolvam problemas comuns nos campos de IA, machine learning e deep learning. Portanto, o campo de atuação das redes neurais é gigantesco. Algumas aplicações são:

- Previsões
- Descoberta de novos remédios
- Entendimento de linguagem natural
- Carros autônomos
- Reconhecimento facial
- Bolsa de valores

## Como uma Rede Neural funciona?
Com um valor de entrada, a rede processa e retorna uma resposta. O neurônio é ativado somente se o valor for maior que um limiar. <br>
<h4 align="center">ENTRADA -> NEURÔNIOS E AXÔNIOS -> SAÍDA </h4>

A RN fará atualização de pesos e também pode conter camadas ocultas, que podem ser definidas pelo programador. Também podem ser escolhidos os tipos de função de ativação. Os mais comuns são:
- Linear
- Sigmoid (também chamada de função logística)
- Tanh
- ReLU
- Leaky ReLU
- eLU

Cada uma pode ser aplicada em diferentes tipos de problemas, podendo ser eficientes ou não, depende do tipo de problema a ser resolvido.
Você vai encontrar muita mais informações na [documentação](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html).

 A base de dados pode ser encontrada no repositório de [Pre-Processamento](https://github.com/Gregory-JP/Pre-Processamento).
