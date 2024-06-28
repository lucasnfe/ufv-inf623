---
layout: page
title: TP 4 - Aprendizado supervisionado
permalink: /assignments/tp4-aprendizado-supervisionado
nav_exclude: true
---

# TP4 - Aprendizado supervisionado

## Introdução

Nesse projeto você irá implementar uma rede neural artificial (RNA) de 3 camadas (1 de entrada, 1 escondidada e 1 de saída) para classificação de dígitos escritos manualmente. Para isso, você irá treinar a sua RNA no conjunto de dados [[MNIST]](http://yann.lecun.com/exdb/mnist/), que possui 70.000 imagens com resolução 28x28 dos dígitos de 0 a 9. O objetivo é praticar a modelagem e a implementação de RNAs, bem como analisar os resultados desse tipo de algoritmo, em particular o impacto dos parâmetros do algoritmo no desempenho do agente.

## Código-base

### Executar servidor

Clique [aqui](/assets/code/tp4-aprendizado-supervisionado.zip) para baixar o código-base, que inclui um cliente em JavaScript para configurar os hiperparâmetros da RNA e iniciar seu treinamento, além de salvar e carregar resultados (pesos e curva de aprendizado). O código também contém um servidor em Python para implementar e executar o treinamento da RNA. Para executar o servidor, você precisará instalar as dependências do projeto e iniciar o servidor com os seguintes comandos:

```
pip install -r requirements.txt # Instalar dependencias
python3 server.py -port 5001 # Executar o servidor
```

Assim que o servidor iniciar, você pode abrir o seguinte endereço em qualquer navegador: [http://localhost:5001](http://localhost:5001).

## Tarefas

Todas as suas tarefas de implementação serão realizadas no arquivo `learn.py`. Antes de começar sua implementação, abra esse arquivo e se familiarize com as funções definidas nesse arquivo. Em seguida, estude a função `gradient_descent_step()` do arquivo `serve.py`, pois ela que executa as funções que terá que implementar.

### 1. Inicialização dos parâmetros (pesos)

Implemente a função `initialize_parameters(input_size, hidden_size, output_size)` para inicializar os parâmetros (pesos) da RNA. Os parâmetros `input_size, hidden_size, output_size` representam o número de neurônios nas camadas de entrada, encondida e de saída, respectivamente. Como o MNIST tem dígitos de 0 a 9, temos um problema de classificação multiclasse com `C=10` classes. Sendo assim, o número de neurônios da camada de saída será `output_size = 10`. Além disso, como as imagens de entrada tem 28x28 pixels de resolução, o número de neurônios na camada de entrada será `input_size = 28x28 = 784`.
A número de neurônios da camada escondida é um hiperparâmetro configurado no cliente no campo de entrada `Neurônios (camada escondida)`.

Essa função deve retornar uma tupla (tuple) com quatro arranjos numpy: `(W1, b1, W2, b2)`, onde `W1, b1` são os pesos da primeira camada e `W2, b2` os pesos da segunda. Lembre-se que em RNAs precisamos inicializar os pesos `W` com valores aleatórios próximos de zero. Os pesos `b` podem ser inicializados com zero, sem problemas. Portanto, utilize a função `np.random.randn` do numpy para inicializar os pesos `W` e a função `np.zeros` para os pesos `b`. O tamanho das matrizes `W1` e `W2` devem ser `input_size x hidden_size` e `hidden_size x output_size`, respectivamente. O tamanho dos vetores `b1` e `b2` devem ser `1 x hidden_size` e `1 x output_size`, respectivamente.

### 2 Funções de ativação

Antes de implementar a propagação das entradas, você precisa implementar as funções de ativação da sua RNA. Nesse trabalho, usaremos a relu como ativação da camada escondida e a softmax para a camada de saída, pois temos um problema multiclasse. 

#### 2.1 Relu

Implemente a função `relu(z)` com a ativação relu, como visto em sala de aula:

#### 2.2 Softmax

Implemente a função `softmax(z)` com a ativação softmax para , como visto em sala de aula:

### 3. Propagação das entradas

Implemente a função `forward(X, parameters)` para propagar as entradas `X` pela RNA definida pelos parâmetros `parameters` (tupla com `(W1, b1, W2, b2)`). Para facilitar o cálculo dos gradientes, é importante calcular a ativação de cada camada em duas etapas: (i) combinação linear e (ii) função de ativação. Portanto, calcule primeiro a combinação linear da camada escondida `Z1 = XW1 + b1` e em seguida aplique a função relu para calcular sua ativação `A1 = relu(Z1)`. Faça a mesma coisa para a camada de saída, calculando primeiro `Z2` e depois `A2`. Note que a entrada da camada de saída é a ativação da camada escondidade `A1`, e não a matrix de exemplos `X`. A funcão `forward` deve retornar uma tupla `(Z1, A1, Z2, A2)`. Utilize a função `np.dot` para fazer as multiplicações de matrizes `XW1` e `A1W2`.

### 4. Função de perda

Implemente a função `cross_entropy_loss(y_true, y_pred)` para calcular a entropia cruzada entre a distribuição real de rótumos `y_true` e as previsões da RNA `y_pred`. Como visto em sala de aula, a função de perda é definida da seguinte maneira:

Utilize a função `np.log` para calcular o logarítmo e `np.sum` para o somatório.

### 5. Gradiente descendente

Implemente a função `gradient_descent_step(X, y, parameters, learning_rate)` para executar uma única época do gradiente descendente:

1. Utilize a função `forward()` para propagar as entradas `X` pela RNA
2. Calcule o erro `l` de previsão atual com a função `cross_entropy_loss()`
3. Calcule os gradientes com a função `backward()` (já está implementado para você)
4. Atulize os pesos `W1, b1, W2, b2` com a regra de atualização do gradiente descendente `w = w - alpha dw`

A sua função deve retornar uma tupla com pesos atualizados `(W1, b1, W2, b2)` e o erro atual `l` da rede, nessa ordem. 

### 6. Avaliação do modelo

Como esse é um problema de classificação, você irá avaliar a sua rede usando a acurácia de previsão, isto é, a taxa de acerto da rede no conjunto de teste. Implemente a função `accuracy(y_true, y_pred)` para calcular a acurácia entre os rótulos reais `y_true` e as previsões `y_pred`. Você pode fazer essa implementação de maneira vetorial em uma linha utilizando as funções `np.mean` e `np.argmax` do numpy.

### 7. Relatório

Nesse trabalho prático você não precisa enviar um relatório, no entanto, você precisará enviar dois gráficos, um com a curva de erro e o outro com a curva de acurácia da sua RNA. Para gerar esses gráficos, execute o script `plot.py`, que irá produzir as curvas utilizando os dados dos arquivos `model/losses.csv` e `model/accuracies.csv`.

## Submissão

Para submeter o seu trabalho, envie o seu arquivo `learn.py` e as duas imagens `losses.png` e `accuracies.png` na tarefa **TP4 - Aprendizado supervisionado** no PVANet.
