# Analise-Sentimentos-em-Tweets-Relacionados-Desmatamento-Floresta-Amazonica-
Repositorio publico referente a execução do artigo "Analise de Sentimentos em Tweets Relacionados ao Desmatamento da Floresta Amazonica " - Paes, Vinicius.

O projeto visa fazer uma analise sobre os sentimentos dos usuarios do twitter sobre o tema do desmatamento da floresta amazonica, nos periodos de janeiro de 2018 á junho 2021. 

O estudo foi dividido em 3 etapas:

* Coleta e processamento dos dados:

Os dados foram coletados em Agosto de 2021 e foram reunidos aproximadamente 252 mil tweets, datados entre 1 de Janeiro de 2019 a 21 de Agosto de 2021. A coleta foi realizada utilizando a biblioteca para Python Twint [Twint 2021],
 juntamente com a biblioteca Jupyter Notebook [Jupyter 2021]. Para a coleta, foram filtrados os tweets que contivessem os termos “Amazonia” em conjunto com os termos “desmatamento” ou “queimadas”.
Essa decisao foi tomada para filtrar ˜ tweets nao relacionados a floresta Amazõnica, uma vez que o nome Amazonia estâ presente em produtos e marcas diversas. Essa regra res tringe a pesquisa, porem garante que os resultados estão de acordo com o esperado para o escopo.  [Paes, Vinicius 2021]

Vale ressaltar o Twitter possui medidas restritivas em realação a coleta de dados por BOTs, assim foi necessario fazer uma busca "partida", os dados foram coletados em periodos de 2 semanas, dessa forma evitando o bloqueio por parte do Twitter.

* Classificação

Para a classificac¸ao dos sentimentos dos tweets, escolheu-se utilizar a classificação com NRC sentiment da biblioteca Syuzhet [Syuzhet 2021] em R. 
Essa biblioteca foi escolhida porque e uma das poucas que pode ser utilizada em portugues sem a necessidade de ferramentas adicionais, alem de possibilitar a analise de emoções mais complexas como “medo” e “alegria”. 
Um dos maiores desafios durante essa fase foi encontrar uma biblioteca capaz de trabalhar com analise léxica de sentimentos sem a necessidades de ferramentas de tradução e durante a pesquisa apenas a Syuzhet se mostrou eficaz.
 Alem disso, de acordo com [Misuraca et al. 2020], Syuzhet possui uma das melhores acurarias em termo de predição dos sentimentos. [Paes, Vinicius 2021]


* Analise

Para realizar a analise, o primeiro passo foi organizar os resultados das análises de sentimento e polaridade em graficos. Com esses resultados organizados, foram definidos e identificados períodos em que existiram um aumento significativo na frequencia de tweets
sobre o assunto em foco. Esses per´ıodos foram Janeiro de 2019, Agosto de 2019, Abril a Maio de 2020 e Abril a Maio de 2021.
Esses agrupamentos foram utilizados para definir em quais per´ıodos seriam geradas as nuvens de palavras e os graficos com emoções. Para a geração de nuvens de palavras, foram identificados os termos mais frequentes dentro do período determinado. 
Termos sao considerados até duas palavras que aparecem frequentemente em conjunto. Um exemplo e o termo “impedir desmatamento”, o qual aparece como um dos termos mais frequentes em todos os períodos analisados. Para essa analise e criação das nuvens de palavras foram utilizadas as bibliotecas TextBlob [TextBlob 2021] para processar a frequencia dos termos dentro dos textos e wordcloud [WordCloud 2021] para gerar as nuvens de palavras, ambas bibliotecas Python. Com os graficos e as nuvens de palavras geradas, foi realizada uma pesquisa traçando paralelos entre os resultados demonstrados nos graficos com notçcias e acontecimentos reportados pela mídia. De forma a comprovar a relação entre o aumento da frequencia dos tweets e o aumento de emoções especificas com as notícias e os eventos. [Paes, Vinicius 2021]


![alt text](https://github.com/viiniciuspaes/Analise-Sentimentos-em-Tweets-Relacionados-Desmatamento-Floresta-Amazonica-/blob/Main/frequencia_tweets_destacado_amarelo.jpg?raw=true)


Publicação em revisão. (Março 2022)