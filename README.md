![](figures/Twitter.png)

Este é um projeto de Processamento de Linguagem Natural (PLN).

O conjunto de dados utilizado está disponível [neste link](https://www.kaggle.com/c/i2a2-nlp-2021-sentiment-analysis/data). 

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

# Entendimento do Negócio

Imagine uma empresa que quer saber sobre a repercussão de uma campanha de marketing que foi lançada no mercado. É possível usar as redes sociais para buscar informações, mas como saber se estão falando bem ou mal dessa campanha? Ler, entender e tirar uma conclusão de milhares de comentários de usuários pode ser uma tarefa inviável.

É nesse cenário que o objetivo desse projeto se enquadra. Iremos desenvolver um modelo de aprendizado de máquina capaz de classificar tweets sobre um determinado tema em positivo ou negativo. Aqui, não iremos avaliar nenhuma campanha, produto ou serviço de uma empresa específica, em vez disso, utilizaremos tweets relacionados a Black Friday, um tema mais "genérico" que não irá expor nenhuma empresa.

O grande desafio desse projeto se dá porque não existe um conjunto de dados de tweets pré-etiquetados para treinar o modelo, então, para a fase de treinamento utilizaremos outros dados de contexto parecido, o de avaliações do grupo B2W Digital. Este grupo é responsável pelas lojas Submarino, Shoptime e Americanas.

Outro desafio desse projeto é em relação a linguagem das mensagens publicadas no Twitter que, em geral, contém gírias, ironias, e caracteres especiais, então, teremos de realizar o pré-processamento nesses dados, para que o modelo consiga classificar textos que "nunca viu antes" de forma satisfatória. Para isso, será utilizado o algoritmo *Multinomial Naive Bayes*, que é um modelo probabilístico baseado na frequência de um termo e excelente para classificação de documentos.

# Dicionário de Dados

Como descrito acima, iremos utilizar o conjunto de dados do grupo B2W Digital para o treinamento do modelo.

Esse conjunto está dividido em dois arquivos, "train.csv" e "test.csv", porém, vamos utilizar apenas o conjunto de treino, que possui as avaliações dos consumidores.
