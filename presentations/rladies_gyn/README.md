# Sobre

O curso de ggplot2 foi um curso expositivo e o objetivo era responder duas perguntas sobre a redução da movimentação aérea durante a crise do Covid. A idéia é que essas perguntas sejam respondidas utilizando visualização de dados. Os scripts foram desenvolvidos usando o R e bibliotecas do tidyverse. As perguntas eram: 
1. Qual o percentual de queda da movimentação dos aeroportos na crise covid?
2. Houveram aeroportos com maior queda de movimentação do que outros?

# Informações

- Os dados foram extraídos através de script de webscrapping do site oficial da [infraero](). Os scripts de webscrapping estão disponíveis na pasta **download_data/**. 
- Os slides estão disponivéis no [link](https://docs.google.com/presentation/d/1QL9epxVU3Gu12i14IPLTQ3_enEF9NPpzoUxZREL6d_g/edit#slide=id.g4c68a97855_1_104)
- Durante o curso, tivemos problema com a base de dados pois estavam faltando informações de alguns meses. O banco de dados atualizado e completo está disponível na pasta **redefined/**.

# Respostas

## 1. Qual o percentual de queda da movimentação dos aeroportos na crise covid?

Utilizamos o modelo de série temporal que leva em consideração o erro, tendẽncia e sazonalidade para predizer o que deveria ter acontecido com o movimento dos aeroportos se não houvesse covid e predizer o que vai acontecer pós crise. A diferença do que aconteceria vs o que aconteceu é justamente a redução da movimentação.
Os scripts das análises para pergunta 1 estão disponíveis na pasta **analysis/**. O script **pergunta1.R** foi construído durante o curso. O script **pergunta1_generalizacao.R** generaliza as análises para que elas sejam rodadas para todas as métricas da base de dados.

**GRÁFICO: Redução da movimentação nos aeroportos administrados pela infraero durante crise do covid19, Janeiro de 2012 a Julho de 2020.
![plot1](Rplot.png)

Algumas conclusões:
1. Houve uma redução de 96% na movimentação de pessoas, 71% de redução do número total de voos e 35% de redução nas cargas do correios.
2. Nos últimos meses, antes da crise covid havia um tendência de queda no número de voos e aumento do número de pessoas, indicando um possível correlação positiva entre essas duas métricas. Em outras palavras, os voos estavam ficando mais lotados.
3. O número de cargas do correios já estava com um comportamento de queda nos meses pré-covid e foi a métrica menos impactada. Houve uma recuperação na movimentação das cargas em maio na seguida de queda brusca em julho (por que será? greve dos correios? ninguem mais quer comprar com entrega pelos correios?).