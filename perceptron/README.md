# Perceptron

O tipo mais básico de Rede Neural Artificial é formada por apenas um neurônio, o Perceptron. Inicialmente, o Perceptron foi projetado para ser um classificador binário linear responsável por mapear uma ou mais entradas em uma saída desejada. Porém, também podemos utilizá-lo para resolver problemas de regressão linear. Ele foi projetado em 1957 por Frank Rosenblatt.

O perceptron é formado por:

<p align='center'>
  <img 
       src='https://www.researchgate.net/publication/355759683/figure/fig5/AS:1142409744396299@1649383116832/Single-Perceptron-by-Frank-Rosenblatt.png' 
       width='400'>
  </img>
</p>

- Entradas x<sub>1</sub>,...,x<sub>n</sub> representam os atributos dos seus dados com dimensionalidade n. O Perceptron aceita qualquer tamanho de entrada, porém a saída é sempre apenas um valor.
- Junção aditiva &sum;: também chamada de _função agregadora_, nada mais é que a soma ponderada das entradas com os pesos (w<sub>1</sub>,...,w<sub>n</sub>). Em geral, o resultado é somado com um bias _b_, responsável por deslocar o resultado do somatório. A junção aditiva é descrita pela seguinte fórmula:

<h2 align='center'>&sum;<sub>i</sub><sup>n</sup> x<sub>i</sub>w<sub>i</sub> + <i>b</i> </h2>

- Função de ativação &fnof;: utilizada para mapear o resultado da junção aditiva em uma saída esperada. Logo, o Perceptron é representado pela seguinte fórmula matemática:

<h2 align='center'> 
  Y = &fnof;(&sum;<sub>i</sub><sup>n</sup> x<sub>i</sub>w<sub>i</sub> + <i>b</i>)
</h2>

Onde:

- n: representa a dimensionalidade das amostras, ou seja, a quantidade de atributos de cada amostra.
- x<sub>i</sub>: representam os atributos de uma amostra que servem de entrada para o Perceptron.
- w<sub>i</sub>: representam os __pesos sinápticos__ que ponderam as entradas.
- _b_: representa o bias, responsável por deslocar a fronteira de decisão além da origem e não depende de nenhum valor de entrada. Repare que o bias encontra-se fora do somatório.
- &fnof;: função de ativação. Quando a função de ativação é linear, ou seja, nenhuma transformação é aplicada no resultado da junção aditiva, o Perceptron atua como um Regressor Linear. Se precisamos efetuar uma Classificação binária, devemos utilizar a função _step_ (também conhecida como _função degrau_) para mapear a saída em um valor discreto (0 ou 1): <br>
<h3 align='center'>&fnof; = 1; <i> se wx + b > 0 </i> <br> &fnof; = 0; <i> caso contrário </i></h3>
  
- Y: representa a saída do Perceptron (o valor predito).

Observações importantes:

- O Perceptron não faz Classificação Multiclasse.
- A atualização dos pesos é *online*, ou seja, efetuada amostra a amostra utilizando uma fórmula pré-definida.
