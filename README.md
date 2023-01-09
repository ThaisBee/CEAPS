# ANALISANDO E TRATADO DADOS DO CEAPS  

Neste trabalho foi usado um dataset coletado do portal do CEAPS (Cota para Exercício da Atividade Parlamentar dos Senadores). Nesse DataSet temos informações a respeito dos gastos declarados dos senadores. O objetivo deste tralho foi limpar e tratar os dados para realizar análises relacionadas aos gastos dos senadores.

1. Lendo o dataset e concatenado em um único Data Frame
2. Explorando o DATASET
3. DATA Cleaning
    - Limpando a coluna COD_DOCUMENTO
    - Limpando a coluna DATA
    - Limpando a coluna VALOR_REEMBOLSADO
    - Transformando a coluna DOCUMENTO em dados booleanos
    - Convertendo variáveis categóricas em variáveis dummies da coluna TIPO_DESPESA
    - Removendo as colunas que não participarão da análise dos dados

4. Análise dos dados
    - Explorando os valores dos gastos ao longo do tempo
        * Teste ADF
        * Autocorrelation Function
        * Partial autocorrelation function
    - Modelo SARIMAX
        * Grid search e a métrica AIC
        * Efetuando previsões
        * Cross validation
