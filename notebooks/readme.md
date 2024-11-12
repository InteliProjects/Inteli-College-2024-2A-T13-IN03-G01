# Tutorial de Como Executar Os Notebooks e Suas Respectivas Utilidades

&emsp;Este guia explica a função de cada notebook, e fornece as instruções necessárias para que qualquer pessoa saiba como executá-los em seu PC.

&emsp;Os notebooks estão organizados por nome, primeiro temos a analise exploratória e pré-processamento, o arquivo de pré-processamento gerará um arquivo que será utilizado nos outros notebooks (comparação modelos e kmeans-model-cluster). Já o arquivo final do "kmeans-model-cluster" será utilizado em todos os notebooks dentro da pasta "/analise-clusters". **O não cumprimento dessa ordem pode gerar erros de execução.**

&emsp;Além disso, na pasta "notebooks", há um arquivo no formato CSV que será utilizado nos notebooks. **A primeira etapa antes de executar qualquer análise de dados nos notebooks é garantir que o arquivo de dados seja carregado nessa pasta, assim o caminho do arquivo fica padronizado, garantindo que os códigos funcionem corretamente**.

## 1. Análise Exploratória e Pré-processamento

&emsp;No notebook de pré-processamento, localizado no caminho notebooks, deve ser executado primeiro, pois ele gerará um arquivo limpo e pronto para ser utilizado como base pelos outros notebooks.

### 1.1 Análise Exploratória

**Função:** Realiza a análise exploratória dos dados para entender suas características principais, identificar padrões e problemas.

**Instruções de Execução e Requisitos:**

**Arquivo:** O arquivo de dados a ser utilizado deve estar na pasta "notebooks", e com nomenclatura igual a "data", exemplo: data.xlsx.

**Bibliotecas Necessárias:** pandas, numpy, matplotlib, seaborn, scikit-learn.

**Passos:**

1. Instale as bibliotecas necessárias usando `import`.
2. Coloque o arquivo de dados na pasta correta.
3. Execute o notebook para carregar o arquivo e gerar visualizações e estatísticas descritivas.
   
### 1.2 Pré-processamento de Dados

**Função:** Prepara os dados para análise e modelagem, corrigindo erros e normalizando variáveis.

**Instruções de Execução e Requisitos:**

**Arquivo:** O arquivo "data.xlsx" deve estar acessível.

**Bibliotecas Necessárias:** pandas, scikit-learn.

**Passos:**

Execute o notebook para corrigir erros de dados, tratar valores nulos e normalizar variáveis. Ao executá-lo, você deve conseguir:

- Identificar e tratar valores extremos (outliers) para evitar que eles distorçam a análise e a modelagem.
- Corrigir inconsistências entre códigos de serviço e suas descrições para assegurar a precisão dos dados.
- Gerar um novo arquivo tratado, que poderá ser utilizado nos outros notebooks.



## 2. Análise Exploratória

&emsp;No notebook de Análise Gráfica, localizado no caminho notebooks, você realizará uma análise visual dos dados para identificar padrões, tendências e anomalias. É importante executar este notebook após o pré-processamento, pois ele depende dos dados limpos gerados anteriormente.

**Bibliotecas Necessárias:** pandas, numpy, matplotlib, seaborn.

**Arquivo:** O arquivo de dados deve estar disponível na pasta "notebooks" com a nomenclatura "data.xlsx".

### 2.1 Os 10 Serviços Mais Utilizados no Plano de Saúde

**Função:** Visualiza os 10 serviços mais utilizados no plano de saúde, permitindo identificar quais serviços são mais frequentes.

**Instruções de Execução e Requisitos:**

**Passos:** Certificar-se de que o arquivo de dados está corretamente nomeado e localizado na pasta "notebooks". Execute o notebook para gerar o gráfico de barras mostrando os 10 serviços mais utilizados. Analise o gráfico para identificar os serviços mais frequentes e quaisquer anomalias significativas.

### 2.2 Valor Total Pago pelos 5 Serviços Mais Utilizados no Plano de Saúde

**Função:** Analisa o valor total pago pelos cinco serviços mais utilizados, ajudando a identificar quais serviços geram maiores custos.

**Instruções de Execução e Requisitos:**

**Passos:** Execute o notebook para gerar o gráfico de barras mostrando o valor total pago pelos cinco serviços mais utilizados.

### 2.3 Gastos por Faixa Etária e Elegibilidade

**Função:** Examina os gastos por faixa etária e tipo de elegibilidade (dependente ou titular), proporcionando uma visão sobre como os gastos variam com a idade e a elegibilidade.

**Instruções de Execução e Requisitos:**

**Passos:** Execute o notebook para gerar o gráfico de dispersão mostrando os gastos por faixa etária. Analise o gráfico para identificar padrões de gastos relacionados à idade e tipo de elegibilidade.

### 2.4 Quantidade de Sinistros por Mês ao Longo do Tempo

**Função:** Avalia a quantidade de sinistros ao longo do tempo, agrupados por bimestres, para identificar padrões sazonais e tendências.

**Instruções de Execução e Requisitos:**

**Passos:** Execute o notebook para gerar o gráfico de linha mostrando a quantidade de sinistros ao longo dos bimestres. Revise o gráfico para identificar quaisquer tendências sazonais ou eventos específicos que influenciam a quantidade de sinistros.

### 2.5 Três Serviços Mais Utilizados por Titulares em Cada Mês

**Função:** Visualiza os três serviços mais utilizados por titulares em cada mês, destacando variações sazonais e tendências de uso.

**Instruções de Execução e Requisitos:**

**Passos:** Execute o notebook para gerar o gráfico de barras empilhadas mostrando os três serviços mais utilizados por titulares em cada mês. Analise o gráfico para identificar variações mensais na utilização dos principais serviços.

## 3. Kmeans-model

&emsp; No notebook de *kmeans model*, localizado no caminho notebooks, será realizado uma técnica de clusterização não supervisionada com K-Means com o objetivo de agrupar usuários de um plano de saúde em clusters baseados em similaridades nos dados. O processo envolve a definição do número ideal de clusters usando o método do cotovelo (Elbow Method), a visualização dos clusters com a Análise de Componentes Principais (PCA) e a interpretação dos centróides que representam as características médias de cada cluster.

**Bibliotecas Necessárias:** pandas, numpy, matplotlib, seaborn, sklearn, plotly.

**Instruções de Execução e Requisitos:** 

**Passos:**

**1. Leitura dos Dados:** Carrega o arquivo data_updated.csv para o DataFrame df e exibe informações para compreensão da estrutura dos dados.

**2. Definição do K Ideal:** O método do cotovelo (Elbow Method) é utilizado para determinar o número ótimo de clusters, calculando o WCSS para diferentes valores de K e identificando o ponto onde a redução no WCSS se estabiliza.

**3. Aplicação do Algoritmo K-Means:** Com o valor de K definido, o algoritmo K-Means é treinado com as variáveis numéricas padronizadas, e o DataFrame é atualizado com uma nova coluna cluster, contendo os valores de cada cluster.

**4. Análise de Componentes Principais (PCA):** O PCA reduz as dimensões dos dados para dois componentes principais, facilitando a visualização dos clusters.

**5. Visualização dos Clusters:** Disponíveis em gráficos 2D e 3D.

**6. Interpretação dos Centrões:** Analisa os centróides de cada cluster para identificar características comuns.

**Passos de Execução:**

- Certifique-se de que o arquivo data_updated.csv esteja na pasta "notebooks".
- Execute todas as células em sequência.
- O gráfico de cotovelo determinará o valor ideal de K.
- Interprete os clusters pelos gráficos e análise dos centróides.

## 4. Comparação de Modelos

&emsp; No notebook de *comparação de modelos*, localizado no caminho notebooks, será realizado uma comparação entre diferentes modelos de clusterização. O objetivo é identificar qual modelo é mais adequado para agrupar usuários de um plano de saúde com base em suas características. Os modelos avaliados são K-Means, DBSCAN e Agglomerative Clustering, e a comparação é feita com base em métricas de avaliação de clusterização.

**Bibliotecas Necessárias:** pandas, numpy, matplotlib, seaborn, sklearn, plotly.

**Instruções de Execução e Requisitos:**

**Arquivos** O arquivo `data_updated_clusters_agg_50.csv` deve estar na pasta "notebooks". Como algumas células são extremamente pesadas e precisam de alto poder computacional, caso não consiga executar o Agglomerative Clustering, esse arquivo trará os clusters já gerados com uma porcentagem da base de dados.

## 5. Análise de Clusters
&emsp; Todos os notebooks dentro da pasta "analise-clusters" utilizam o arquivo gerado pelo notebook "data_updated_clustered_kmeans.csv". Portanto, é necessário executar o notebook "kmeans-model-cluster" antes de executar qualquer um dos notebooks dentro da pasta "analise-clusters". O KMeans é um algoritmo de clusterização que agrupa os dados em clusters com base em similaridades. O notebook "kmeans-model-cluster" aplica o algoritmo KMeans aos dados do plano de saúde para agrupar os usuários em clusters com base em suas características. Os clusters são identificados por números inteiros e representam grupos de usuários com características semelhantes.

O notebook "kmeans-model-cluster" já conta com os hiperparâmetros ajustados e o número de clusters definido.

**Bibliotecas Necessárias:** pandas, numpy, matplotlib, seaborn, sklearn.