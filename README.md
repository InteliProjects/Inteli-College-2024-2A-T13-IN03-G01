# Inteli - Instituto de Tecnologia e Liderança 

<p align="center">
<a href= "https://www.inteli.edu.br/"><img src="assets/inteli.png" alt="Inteli - Instituto de Tecnologia e Liderança" border="0"></a>
</p>

# DIPA - DuoÍmpar Predictive Analysis

## DuoÍmpar

## Integrantes: 
- <a href="https://www.linkedin.com/in/anacdejesus/">Ana Carolina Jesus Pacheco da Silva</a>
- <a href="https://www.linkedin.com/in/anna-riciopo/">Anna Giulia Marques Riciopo</a>
- <a href="https://www.linkedin.com/in/gabriel-scarpelin-diniz-425258144/">Gabriel Scarpelin Diniz</a> 
- <a href="https://www.linkedin.com/in/iasmim-/">Iasmim Santos Silva de Jesus</a> 
- <a href="https://www.linkedin.com/in/pauloheribeiro">Paulo Henrique Ribeiro</a>
- <a href="https://www.linkedin.com/in/pedro-pinheiro-rodrigues-b129b62b7/">Pedro Pinheiro Rodrigues</a> 
- <a href="https://www.linkedin.com/in/kesneylucas/">Kesney Lucas Ferro de Oliveira</a>
- <a href="https://www.linkedin.com/in/yanom%C3%A3/">Yanomã Fernandes Konwski</a>

## Professores:
### Orientador(a) 
- <a href="https://www.linkedin.com/in/juliastateri/">Julia Stateri</a>
### Instrutores
- <a href="https://www.linkedin.com/in/geraldo-magela-severino-vasconcelos-22b1b220/">Geraldo Magela Severino Vasconcelos</a>
- <a href="https://www.linkedin.com/in/egondaxbacher/">Egon Daxbacher</a> 
- <a href="https://www.linkedin.com/in/bruna-mayer/">Bruna Mayer</a> 
- <a href="https://www.linkedin.com/in/filipe-gon%C3%A7alves-08a55015b/">Filipe Gonçalves</a>
- <a href="https://www.linkedin.com/in/kizzyterra/">Kizzy Terra</a> 


## 📝 Descrição

&emsp;Este projeto da Unipar tem como objetivo aprimorar os programas de saúde dos colaboradores através de modelos não supervisionados de clusterização. Com base em dados históricos de sinistralidade, o foco é identificar padrões de utilização dos planos de saúde e segmentar os colaboradores em grupos com características de saúde semelhantes. Essa segmentação é essencial para personalizar os programas de saúde, ajustando-os de acordo com as necessidades específicas de cada grupo, como o manejo de doenças crônicas ou a promoção de hábitos saudáveis.

&emsp;A implementação desse modelo permitirá à Unipar otimizar o uso de seus recursos, oferecendo programas de saúde mais eficientes e direcionados. A tecnologia de clusterização facilita a detecção de padrões que, de outra forma, passariam despercebidos, proporcionando uma visão mais estratégica da utilização dos planos de saúde pelos colaboradores. Além disso, a solução proposta busca manter a sustentabilidade dos programas ao longo do tempo, garantindo que eles continuem eficazes e economicamente viáveis.

&emsp;Com essa abordagem inovadora, a Unipar poderá ajustar seus programas de saúde com base em dados reais, promovendo um impacto positivo na qualidade de vida dos colaboradores e na eficiência dos recursos destinados à gestão de saúde.

<b>Link para vídeo demonstrativo: </b> <a href="https://inteli.edu.br">https://youtu.be/WBXwFL2daOo</a>


## 📁 Estrutura de pastas

Dentre os arquivos presentes na raiz do projeto, definem-se:

- <b>readme.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

- <b>assets</b>: todas as imagens e mídias utilizadas nos notebooks e documentação são posicionadas aqui.

- <b>documents</b>: aqui estarão todos os documentos do projeto. Há também uma pasta denominada <b>extras</b> onde estão presentes documentos complementares.

- <b>notebooks</b>: todos os Jupyter Notebooks criados para desenvolvimento do projeto.

A estrutura de pastas segue a seguinte estrutura:

```
├── readme.md
├── assets/
│   └── imagem2.png
├── documents/
│   ├── documentacao.md
│   └── extras/
│       └── instrucao.txt
├── notebooks/
│   ├── sprint2/
│   │   ├── analise-exploratoria.ipynb
│   │   └── pre-processamento.ipynb
│   ├── sprint3/
│   │   └── kmeans-model-cluster.ipynb
│   ├── sprint4/
│   │   └── comparacao-modelos.ipynb
│   ├── sprint5/
│   │   └── analise-clusters.ipynb
│   ├── feriados_2023.json
│   ├── feriados_2024.json
│   └── orientacao.md
├── .gitattributes
├── .gitignore
└── README
```


## 💻 Execução dos projetos

### Arquivos necessários

* ```data.xlsx```

### Passo a passo

1. **Clonar o repositório**

&emsp;No terminal, clone o repositório do projeto que contém tanto os notebooks em _Python_. Use o comando:

HTTPS:
```bash
git clone https://github.com/Inteli-College/2024-2A-T13-IN03-G01.git
```

SSH:
```bash
git clone git@github.com:Inteli-College/2024-2A-T13-IN03-G01.git
```

2.  **Instalar o _Python_ e o gerenciador de pacotes _pip_**

Caso ainda não tenha Python instalado, baixe e instale a versão 3.13.0 no site <https://www.python.org/>. Após a instalação, certifique-se de que o pip também está instalado.

3. **Instalar dependências do _python_**

Certifique-se de ter as seguintes versões instaladas para rodar os notebooks Python:

- **Python**: 3.13.0
- **NumPy**: 2.2.0
- **Pandas**: 2.2.3
- **Matplotlib**: 3.9
- **Scikit-learn**: 1.5
- **Jupyter**: 7.2.2

Para instalar as dependências acima, você pode rodar no terminal:

```bash
pip install numpy==1.21.x pandas==1.3.x matplotlib==3.4.x scikit-learn==0.24.x jupyter==1.0.x
```

3. **Executar os notebooks**

Agora, você pode abrir e rodar os notebooks em um ambiente como o _Jupyter_.

```bash
pip install jupyter
jupyter notebook
```

Isso abrirá uma interface no navegador onde você poderá interagir com seus notebooks.

Outra opção é rodar os notebooks através de um ambiente de desenvolvimento como o _VSCode_, no _VSCode_ você pode instalar a extensão [_Jupyter_](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) e rodar os notebooks diretamente no ambiente.

Os notebooks requerem um arquivo chamado ```data.xlsx``` que deve ser colocado na pasta ```notebooks/```. Além disso, vale ressaltar que uma ordem também é sugerida para a execução dos notebooks, que é a seguinte:
1. ```analise-exploratoria.ipynb```
2. ```pre-processamento.ipynb```
3. ```kmeans-model-cluster.ipynb```
4. ```comparacao-modelos.ipynb```
5. Notebooks com as análises de cada cluster


## 🗃 Histórico de lançamentos

* 1.0.0 - 11/10/2024
    * [sprint 5] Lançamento da primeira versão do modelo preditivo com documentação.
* 0.4.0 - 27/09/2024
    * [sprint 4] Comparação de modelos preditivos
* 0.3.0 - 13/09/2024
    * [sprint 3] Preparação de dados e modelo preditivo preliminar
* 0.2.0 - 30/08/2024
    * [sprint 2] Análise exploratória e levantamento de hipóteses
* 0.1.0 - 16/08/2024
    * [sprint 1] Documentação de entendimento do negócio

## 📋 Licença/License

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/Inteli-College/2024-1B-T13-IN02-G04/blob/main/README.md">DuoÍmpar</a> by Inteli is licensed under <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>