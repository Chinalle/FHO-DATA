# Escolha do dataset

Resolvi escolher um dataset do Kaggle que utilizam para competição, denomina 'House Price'. Nela contem 81 colunas como 'SalePrice', 'GarageYrBlt', 'GrLivArea', 'GarageArea', '1stFlrSF', 'GarageCars' e outros. A finalidade da analise desse modelo é prever o possivel valor
da casa para cada caracteristica que contem no dataset de treino.

# Data wrangling

Nessa etapa do processo da analise, utilizando a regressão linear, importei a base de treino e verifiquei os tipos de dados que contém nesse dataset e se estão legiveis a analise. Algumas tratativas que realizei foi a exclusão de colunas que não contia valores númericos.
Nas colunas que conteve valores númericos, retirei todas as linhas que se encontrava valores nulos, para não afetar a analise nos proximos processos.

# Correlação entre cada variável

Com a base já preparada para as analises, realizei o calculo da correlação, porém eram 38 colunas e a grande maioria contia uma fraca correlação. Com isso decide fazer um filtro e manter somente as colunas que contiam correlações fortes. Para que isso seja possivel
realizei um for para cada linha da matriz de correlação criada, e fui adicionando as colunas em outra lista que contia a correlação maior que 0.70 ou menor que -0.70.

# Regressão Linear

Contendo o X (colunas com correlações maiores) e o y que será a coluna de 'SalePrice', criei o modelo fit e seus coeficientes para ser possivel a utilização da formula da reta. Após isso plotei na tela os graficos de cada coluna que representa o x em função de y. 

# Conclusão

Os resultados não foram bons, ocasionou em um underfitting já que as retas ficaram bem distantes dos pontos das instâncias. Pretendo trabalhar mais nesse modelo e fazer alterações no momento do data wrangling e no filtro da correlação das varáiveis, ja que 10 colunas 
são um grande número de dados e isso pode ser uma das causas do underfitting.
