📊 Previsão de Estoque Inteligente na AWS com SageMaker Canvas
Este projeto foi desenvolvido como parte de um Bootcamp na DIO, focado em utilizar inteligência artificial para prever níveis de estoque de produtos. O objetivo principal é aplicar o conceito de No-Code ML utilizando o Amazon SageMaker Canvas.

🚀 Passo a Passo do Projeto
1. Preparação dos Dados
O dataset utilizado contém informações históricas de vendas e estoque, com as seguintes colunas principais:

ID_PRODUTO: Identificador único de cada item.

DATA_EVENTO: Carimbo de data/hora do registro.

PRECO: Valor unitário do produto.

QUANTIDADE_ESTOQUE: A variável alvo que desejamos prever.

2. Configuração do Modelo no SageMaker Canvas
Após realizar o upload do dataset, as seguintes configurações foram aplicadas:

Target Column: QUANTIDADE_ESTOQUE.

Model Type: Time Series Forecasting (Série Temporal).

Item ID: ID_PRODUTO.

Timestamp: DATA_EVENTO.

Forecast Horizon: Configurado para prever os próximos 9 dias.

3. Análise e Treinamento
O modelo foi treinado utilizando o modo "Standard Build" para garantir maior precisão. Durante a fase de análise, observamos as seguintes métricas de performance:

Avg. wQL (Weighted Quantile Loss): 0.271

MAPE (Mean Absolute Percentage Error): 1.546

WAPE (Weighted Absolute Percentage Error): 0.471

RMSE (Root Mean Square Error): 30.072

[!IMPORTANT] A análise de impacto das colunas mostrou que o PRECO teve uma influência de 100% nas oscilações do estoque, indicando uma forte correlação entre preço e demanda no dataset utilizado.

4. Resultados das Previsões
O modelo gera três cenários de previsão baseados em quantis:

P10 (Pessimista): Representa um cenário onde há 10% de chance da demanda ser menor que o valor mostrado.

P50 (Médio): O valor mediano da previsão.

P90 (Otimista): Cenário de alta demanda, útil para evitar a falta de estoque (Stockout).

🔍 Insights Obtidos
O modelo conseguiu captar as flutuações históricas e projetar uma tendência de estabilização para os próximos dias.

Produtos com IDs específicos (ex: Item 1 e Item 13) apresentam comportamentos de estoque distintos, permitindo uma gestão personalizada por SKU.

A alta influência do preço sugere que promoções ou alterações de valores podem ser usadas estrategicamente para gerenciar o volume de estoque.

🛠️ Tecnologias Utilizadas
AWS SageMaker Canvas (Machine Learning No-Code)
