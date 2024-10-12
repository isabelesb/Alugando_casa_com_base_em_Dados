# Escolhendo a melhor casa para alugar!

O objetivo aqui é encontrar uma casa para alugar, com o melhor custo benefício possível.
Para isso, utilizamos dados de moradias em Barcelona e na cidade do Porto. E de acordo com as características delas, fomos diminuindo as opções até chegarmos a apenas duas, que melhor se encaixaram nas exigÊncias do cliente. 

## Condições do cliente:
1.  Valor de aluguel abaixo de 4 mil euros.
2.  Aceitar pets.
3.  Ter 2 ou 3 quartos.
4.  Em prédios, dar preferência a andares superiores.

## Bibliotecas do python:
1. Pandas.
2. Seaborn.

## Entendimento e tratamento dos Dados:
1. O primeiro tratamento foi realizado nos nomes das colunas do dataframe, pois havia espaço entre palavras de alguns deles.
2. A seguir, o tipo de alguns dados foi modificado.
3. Foi utilizado um filtro triplo para estipular 4000.00 como valor máximo do aluguel, para garantir que o local aceite animais de estimação e para assegurar que hajam dois ou três quartos. A partir desse filtro, um novo dataframe foi criado.
4. Analisamos que o desvio padrão dos dados é baixo, o que é satisfatório. Pois isso indica que não há dados discrepantes.

## Visualizações:
1. Foi verificada a média de preços para cada cidade e percebemos que a diferença é pequena.
2. Com um histograma, verificou-se então a quantidade de casas em cada cidade, de acordo com o preço. Aqui percebe-se uma diferença razoavel na distribioção delas, Barcelona tendo mais casa caras do que baratas. Com essa informação, foi decidido que a melhor cidade para morar seria o Porto.
3. O passo seguinte foi escolher em qual andar focar. Com um gráfico de barras, relacionando o número de andares com o preço do aluguel, percebeu-se que a melhor opção é o 16º andar.
4. Filtrando o dataframe para conter apenas apartamentos de 16º andar, restaram as duas opções finais.

## Conclusão:
As opções restantes formam a indicação final do modelo. Sendo assim, o cliente pode escolher a que melhor lhe servir.

