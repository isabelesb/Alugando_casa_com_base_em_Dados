# Escolhendo a melhor casa para alugar!

## Entendimento do negócio:
Nosso cliente deseja alugar uma casa ou apartamento, em Barcelona ou Madri. Ele tem algumas condições e nosso objetivo é ajudá-lo. 
Faremos isso reduzindo suas opções, para facilitar a tomada de decisão.

### Condições do cliente:
1.  Valor de aluguel, no máximo, de 4 mil euros.
2.  Aceitar pets.
3.  Ter 2 ou 3 quartos.
4.  Em prédios, dar preferência a andares superiores.

## Entendimento dos dados:
Para nossas análises e tratamentos, usaremos a biblioteca Pandas.

- Nosso dataframe contém 6080 entradas, com dados de localização, número de quartos e banheiros, disponibilidade de vagas para estacionamento e preço das moradias. Algumas dessas colunas precisam ser renomeadas, pois seus nomes contém espaços.
- Não há dados nulos.
- Alguns tipos de dados precisam ser alterados.
- De acordo com os dados de distribuição, não há outliers.

## Preparação dos Dados:
1. O primeiro tratamento foi realizado nos nomes das colunas do dataframe, pois havia espaço entre palavras de alguns deles.
2. A seguir, o tipo de alguns dados foi modificado.
3. Através de um filtro triplo, estipulamos
   a) 4000.00 como valor máximo do aluguel,
   b) que o local aceite animais de estimação, e
   c) que hajam dois ou três quartos.

## Modelagem:
Agora que nossos dados estão de acordo coma as condições do cliente, faremos uma análise mais aprofundada. Para isso, além do Pandas, utilisaremos a biblioteca Seaborn para visualizações.

1. Foi verificada a média de preços de aluguéis para cada cidade e percebemos que a diferença é pequena. Mas vimos também que a maior parte das casas de Barcelona é cara, enquanto em Porto é o contrário.
   <img src="https://github.com/isabelesb/Alugando_casa_com_base_em_Dados/blob/main/quantidade_de_casas_por_preco_por_cidade.png" alt="Falha no carregamento. Vide imagem: quantidade_de_casas_por_preco_por_cidade.png">
Por isso, decidimos continuar procurando apenas na Cidade do Porto.

2. O passo seguinte é escolher em qual andar focar. Relacionamos então o andar da casa/apartamento com o preço do aluguel.
   <img src="https://github.com/isabelesb/Alugando_casa_com_base_em_Dados/blob/main/valor_do_aluguel_pela_quantidade_de_andares.png" alt="Falha no carregamento. Vide imagem: valor_do_aluguel_pela_quantidade_de_andares.png">
Com o gráfico, percebemos que a melhor opção é o 16º andar, já que andares mais altos têm preferência para o cliente.

3. Com essa escolha, precebemos que restam agora apenas duas opções. E com isso podemos concluir o projeto.
   <img src="https://github.com/isabelesb/Alugando_casa_com_base_em_Dados/blob/main/opcoes_finais.png" alt="Falha no carregamento. Vide imagem: opcoes_finais.png">

## Avaliação:
Nosso objetivo aqui era facilitar a escolha do nosso cliente. Inicialmente, ele tinha 6080 opções de residência e nem todas estavam de acordo com seus critérios. Conseguimos reduzir essas opções a duas, que se cabem perfeitamente em suas exigências.

