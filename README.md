# Projeto de Engenharia de Dados da Udacity

Este projeto utiliza o pyspark para extrair dados e organizá-los em um banco de dados com esquema snowflack composto por tabelas de fatos e dimensões.
Ele extrai dados de arquivos parquet e csv.



# Dados de Imigração dos EUA

### Projeto Final de Engenharia de Dados

#### Resumo do Projeto
Este projeto tem como objetivo usar as técnicas aprendidas no curso Nanodegree da Udacity sobre Engenharia de Dados para criar tabelas de fatos e dimensões relacionadas aos dados de imigração dos EUA, juntamente com análises sobre temperatura e características dos aeroportos. Aqui, usaremos dois formatos de dados (SAS e .csv) para construir tabelas de FATOS e dimensões, dividindo o conjunto de dados de imigração dos EUA em relação ao que são suas informações (voo? passageiro?) e adicionar informações sobre a temperatura nas datas observadas.

# Conjunto de dados 1: Dados de imigração I94 do Escritório Nacional de Turismo e Comércio dos EUA

- São os dados que serão usados para construir nossa tabela de FATOS. Eles contêm informações sobre companhia aérea, tipo de visto e destino das pessoas que imigram para os EUA.

- Primeiramente, verificaremos se há dados faltando, se os dados estão se comportando conforme o esperado e transformaremos os dados quando necessário.
- Este conjunto de dados tem cerca de 3 milhões de linhas e 28 colunas. Limitaremos as colunas àquelas que nos interessam e exploraremos como dividi-las em novas tabelas quando relevante.
- Esses dados são atualizados mensalmente.
- Para este projeto, optei por excluir colunas com mais de 30% de seus valores nulos. No entanto, é esperado que casos com valores nulos ocorram em projetos de engenharia de dados, e está é uma das muitas abordagens possíveis.
- Neste conjunto de dados, temos muitas informações, podemos dividi-lo de acordo com o tipo de informação.
- Utilizamos o draw.io para criar uma visualização do esquema
- Permitirei que os valores nan continuem como nan, sem técnicas de substituição



# Conjunto de dados 2: Temperatura
- Temperatura por cidade e data


# Conjunto de dados 2: Aeroporto 
- Código
- Localização
- Estado


# Tecnologias e ferramentas 

Aqui, optei por usar o pyspark e aproveitar o processamento paralelo.

# Passos:

- Crie um ambiente para o projeto.
- Instale os seguintes pacotes: Pandas, Re, Pyspark, Numpy.
- Execute o Capstone Project Template.ipynb (exemplo: usando o Vscode e verificando se o kernel se refere ao ambiente diserd).

# Objetivo:

Crie este modelo de dados a partir dos conjuntos de dados iniciais descritos acima:

![alt_text](new_datamodel.PNG)

## Exemplo de análise com modelo de dados:
- Verifique a temperatura na data de chegada de um passageiro
- Verifique a temperatura no porto na data
- Correlacione os passageiros e descubra se há indícios de preferência em relação à temperatura para a escolha da data do voo



