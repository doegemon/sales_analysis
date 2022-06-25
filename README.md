# sales_analysis
Projeto de Análise Exploratória de Dados de clientes, produtos, pedidos e vendas de uma empresa de varejo no segmento de vestuário, com foco no e-commerce e sediada na Austrália. 

# 1. Contexto
Inicialmente, quero destacar que esse conjunto de dados é proveniente do Kaggle (link abaixo), composto por 04 arquivos em .csv. Como o intuito era praticar os comandos e recursos do SQL, usei o DB Browser (SQLite) para compilar os 04 arquivos .csv em um arquivo do tipo .db.

Feito isso, ainda usei o DB Browser (SQLite) para realizar algumas análises iniciais do conjunto de dados de cunho mais técnico, tais como: os atributos/colunas de cada tabela, o tipo dos registros (INT, TEXT, DATE etc.), verificar a existência de valores nulos, entre outras. 

Durante essas análises, procedi com as seguintes mudanças:

 a) Formatação das colunas de datas da tabela 'orders' para DATE, já que estavam em formato TEXT; 
 
 b) Criação de uma coluna/atributo novo na tabela 'orders', denominada 'order_month' (para facilitar posterior análise); e
 
 c) Criação de novas tabelas com base nas antigas para atribuir Chaves Primárias e Chaves Estrangeiras à determinados atributos/colunas, criando um banco de dados relacional e possibilitando 'queries' utilizando o comando JOIN.

Por fim, para guiar esse projeto, elaborei algumas perguntas fictícias de negócio para serem respondidas através de queries no banco de dados. 

# 2. Perguntas de Negócio
 a) Qual a faixa etária que mais comprou? (Número de Pedidos e Receita)
  
 b) Qual o gênero que mais comprou? (Número de Pedidos e Receita)
  
 c) Qual o Estado que mais comprou? (Número de Pedidos e Receita)
  
 d) Quais foram os meses com o maior número de pedidos? (Número de Pedidos e Receita)
  
 e) Quais os produtos mais vendidos? (Número de Pedidos e Receita)
  
 f) Qual o tempo médio entre a data do pedido e a data de entrega?
  
 g) Qual o desempenho de vendas por trimestre? (Número de Pedidos e Receita)
  
# 3. Respostas
 a) 56.85% das vendas são feitas para Adultos (idade entre 25 e 59 anos), 31.63% para Idosos (idade acima de 60 anos), e 11.51% para Jovens (idade abaixo de 24 anos).
 
 b) Tratando de gêneros, não existe uma discrepância muito grande entre as vendas, mas são as mulheres que mais compram, representando 14.09% das vendas.
 
 c) Da mesma forma que os gêneros, não temos uma discrepância muito grande entre as vendas, sendo o Estado que mais comprou o Estado de South Australia, representando 14.33% das vendas.
 
 d) Considerando que o conjunto de dados possui registros de Janeiro a Outubro, os três melhores meses de venda (até agora) foram Março, Janeiro e Julho.
 
 e) O produto mais vendido no período foi a Jaqueta de Denim, representado 5.08% das vendas da empresa. Em seguida, temos a Camisa Slim Fit, a Jaqueta Trench, a Jaqueta Shearling e a Jaqueta Puffer.

Esses 05 produtos, somados, representam 18.89% das vendas da empresa no período.
 
 f) O número médio de dias entre o pedido e a entrega do produto para o cliente é de 14 dias.
 
 g) O Primeiro Trimestre (Janeiro a Março) foi o melhor período de vendas para a empresa.

Todavia, cabe ressaltar que o Quarto Trimestre tem somente as vendas do mês de Outubro, sendo esse o último mês que temos registros no conjunto de dados.

# 4. Conclusões
Através da análise dos dados de clientes, produtos, pedidos e vendas da empresa, pude extrair algumas informações e gerar insights que podem influenciar em estratégias de vendas e publicidade, visando o aumento da receita e crescimento do negócio.

# Referências

### Dataset
https://www.kaggle.com/datasets/ruchi798/shopping-cart-database?select=sales.csv

### DB Browser (SQLite)
https://sqlitebrowser.org/
