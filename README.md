# Sistema_de_recomandacao
 
## SISTEMAS DE RECOMENDAÇÃO UTILIZANDO MACHINE LEARNING

Contexto:
Movielens, um site pertencente ao Grouplens que tem um sistema de avaliação de vários filmes - ou seja, as pessoas podem dar notas de alguma maneira e encontrar outros filmes que lhes interessam, tudo muito ligado à questão de recomendação.
No Movielens, é possível baixar um conjunto de dados enorme contendo 20 milhões de avaliações dos usuários, ou outras duas variações desse conjunto, contendo 27 milhões ou 100 mil avaliações. Usaremos a última, que é uma versão menor e mais simples.
Onde foi extrtaido os dados https://grouplens.org/datasets/movielens/latest/

Nosso Objetivo:
Construir um modelo de sistema de recomendação e utilizá-lo para gerar recomendações em um conjunto de dados de filmes, no caso as avaliações dos filmes do site MovieLens, que usaremos para gerar um sistema de recomendações para os usuários; e implementar algoritmos de machine learning.
Utilizaremos duas heurísticas. A primeira heurística de recomendação é: com base nas informações que outros usuários e usuárias passaram (o número de votos), podemos indicar os cinco filmes mais populares (que definimos como sendo os mais avaliados) para uma pessoa sobre quem não sabemos nada.
A segunda heurística que utilizamos para nos trazer resultados satisfatórios é ordenar os filmes pela nota média. 
O resultado são diversos filmes que se encaixam com o perfil de usuário que nós criamos no projeto. 
A ideia desse projeto é aprender um pouco sobre sistemas de recomendações, que também são comumente chamados de RecSys (recomendation systems). É possível encontrar muita literatura em inglês pesquisando pelo termo.
Existem diversos sistemas de recomendação, e nós aprendemos alguns critérios que podem ser utilizados neles, tentando implementar por baixo dos panos um algoritmo chamado k-NN ("os k vizinhos mais próximos"). 
Durante o projeto vimos, para o k-NN, temos uma implementação que é baseada na distância e no teorema de Pitágoras, que aprendemos na escola. Essa função de distância pode ficar cada vez mais complicada à medida em que são inseridas outras características. Depois, fizemos uma filtragem dos usuários mais próximos para tirarmos uma média das notas que eles atribuíram aos filmes.
Todas essas partes são customizáveis e otimizáveis.
Com base em algoritmos de recomendação como o k-NN, você pode procurar bibliotecas, como a Surprise em Python, que implementam esses algoritmos e podem ser utilizadas de maneira muito mais simples. Quando você for usar esses algoritmos efetivamente em produção, você poderá utilizar o conhecido pipeline de separação de dados para treino, teste do algoritmo e validação do conjunto de dados para verificar o quanto você errou nas avaliações, além de outras opções que essas bibliotecas fornecem.
