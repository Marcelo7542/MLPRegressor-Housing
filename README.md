English description below


MLPRegressor-Housing

Descrição do Repositório

Este repositório contém dois exemplos de implementações de redes neurais para regressão usando TensorFlow e Keras:

MLPRegressor: 

Um modelo sequencial baseado em Multilayer Perceptron (MLP) para previsão de valores de uma base de dados.

Functional API: 

Uma abordagem mais flexível para criar modelos de redes neurais com a API funcional do Keras, incluindo entradas e saídas múltiplas.

Ambos os exemplos utilizam o conjunto de dados boston_housing.

MLPRegressor

Nesta implementação, desenvolvi uma rede neural sequencial com:

Normalização dos dados de entrada para melhorar o desempenho do treinamento.

Várias camadas densas (fully connected) com ativação ReLU.

Callback de ModelCheckpoint para salvar os pesos do modelo durante o treinamento.

EarlyStopping para interromper o treinamento quando o modelo não melhorar após um número definido de épocas.

Integração com TensorBoard para monitorar o treinamento em tempo real.

Principais Características

Modelo sequencial com 7 camadas densas.

Função de perda:

mean squared error (mse).

Métrica de avaliação: 

RootMeanSquaredError.

Otimizador: 

Adam com taxa de aprendizado definida manualmente.

O treinamento foi realizado em 10.000 épocas com validação cruzada e visualização das métricas no TensorBoard.

Resultados

Após o treinamento, o modelo foi avaliado no conjunto de teste para prever valores de habitação. A avaliação incluiu o erro quadrático médio (MSE) e a raiz do erro quadrático médio (RMSE).




Functional API

Com a API funcional do Keras, implementei um modelo de regressão que:

Utiliza duas entradas separadas, cada uma passando por um processo de normalização.

Integra as entradas por meio de uma camada de concatenação.

Possui saídas múltiplas para previsão de diferentes alvos.

Principais Características

Modelo mais flexível com estrutura definida dinamicamente.

Três camadas densas no caminho principal.

Uma camada de concatenação para combinar informações das duas entradas.

Duas saídas.

Resultados

A estrutura permitiu analisar diferentes abordagens para tratar entradas e saídas múltiplas. O modelo mostrou-se eficaz na previsão de valores a partir de entradas normalizadas.

Tecnologias Utilizadas

Python: 

Linguagem principal para desenvolvimento.

TensorFlow/Keras: 

Framework para criação e treinamento das redes neurais.

Boston Housing Dataset: 

Conjunto de dados para previsão de preços de casas.

TensorBoard: 

Ferramenta de visualização de métricas de treinamento.

Callbacks: 

Incluindo ModelCheckpoint e EarlyStopping para otimização do treinamento.





MLPRegressor-Housing

Repository Description

This repository contains two examples of neural network implementations for regression using TensorFlow and Keras:

MLPRegressor:

A sequential model based on Multilayer Perceptron (MLP) for predicting values from a dataset.

Functional API:

A more flexible approach to creating neural network models using Keras' Functional API, including multiple inputs and outputs.

Both examples utilize the boston_housing dataset.

MLPRegressor

In this implementation, I developed a sequential neural network with:

Normalization of input data to improve training performance.

Multiple dense (fully connected) layers with ReLU activation.

ModelCheckpoint callback to save model weights during training.

EarlyStopping to stop training when the model stops improving after a defined number of epochs.

Integration with TensorBoard for real-time training monitoring.

Key Features

Sequential model with 7 dense layers.

Loss function:

Mean Squared Error (MSE).

Evaluation metric:

Root Mean Squared Error (RMSE).

Optimizer:

Adam with manually defined learning rate.

Training was conducted over 10,000 epochs with cross-validation and visualization of metrics on TensorBoard.

Results

After training, the model was evaluated on the test set to predict housing values. The evaluation included the Mean Squared Error (MSE) and the Root Mean Squared Error (RMSE).

Functional API

With Keras' Functional API, I implemented a regression model that:

Utilizes two separate inputs, each undergoing a normalization process.

Integrates the inputs through a concatenation layer.

Has multiple outputs.

Key Features

More flexible model with dynamically defined structure.

Three dense layers in the main path.

A concatenation layer to combine information from the two inputs.

Two outputs.

Results

This structure allowed the exploration of different approaches to handling multiple inputs and outputs. The model proved effective in predicting values from normalized inputs.

Technologies Used

Python:

Primary language for development.

TensorFlow/Keras:

Framework for creating and training neural networks.

Boston Housing Dataset:

Dataset for predicting housing prices.

TensorBoard:

Tool for visualizing training metrics.

Callbacks:

Including ModelCheckpoint and EarlyStopping for training optimization.


