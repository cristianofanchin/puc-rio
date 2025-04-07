![Brasao Puc-Rio](https://www.puc-rio.br/imagens/bras_83x140_reduzido.png)
# Puc-Rio - Pós-Graduação em Ciência de Dados e Analytics
Aluno: Cristiano Weiber Fanchin
<br/><br/>

## Sprint 3 - Engenharia de Dados - MVP
O trabalho aqui apresentado tem por objetivo construir e documentar um pipeline de dados utilizando tecnologia em nuvem.
A plataforma adotada foi a Databricks Comunity Edition, de uso gratuito.

A apresentação do trabalho inicia nesta página, onde temos a introdução ao tema, o relato da busca pelos dados e a descrição de um problema de análise de dados que se deseja resolver.

Na sequência, você deverá navegar por cada um dos quatro notebooks que detalharão as etapas realizadas na plataforma Databricks, com apresentação do código executado e evidências dos resultados obtidos. Os notebooks também contém relatos e conclusões parciais referentes aos passos desse MVP.

<br/><br/>
Haverá ao final de cada notebook um link para o próximo, mas se preferir, pode acessá-los diretamente por aqui:
<br/><br/>

**[📘 Notebook 1 - Fazer o download do dataset e salvar os arquivos no DBFS](https://github.com/cristianofanchin/puc-rio/blob/main/engenhariadados/1-Download_Dataset_ZIP.ipynb)**
<br/><br/>
**[📘 Notebook 2 - Catálogo de Dados e Análise da Qualidade](https://github.com/cristianofanchin/puc-rio/blob/main/engenhariadados/2-Catalogo_e_Analise_de_Dados.ipynb)**
<br/><br/>
**[📘 Notebook 3 - Processos ETL nas camadas Bronze, Silver e Gold](https://github.com/cristianofanchin/puc-rio/blob/main/engenhariadados/3-ETL_Bronze_Silver_Gold.ipynb)**
<br/><br/>
**[📘 Notebook 4 - Solução do Problema e Autoavaliação](https://github.com/cristianofanchin/puc-rio/blob/main/engenhariadados/4-Solucao_do_Problema_e_Autoavaliacao.ipynb)**


<br/><br/>

## 📌Introdução

Para esse trabalho, buscou-se um dataset de assunto de relevante interesse para o autor e cujos dados pudessem ser trabalhados de forma a cumprir o escopo do MVP.
Dessa forma, após uma busca em bases gratuitas de dados disponíveis na internet, chegou-se a um dataset contendo registros de visitas hospitalares do Hospital Geral de Massashuseets dos anos compreendidos entre 2011 e 2022, incluindo dados demográficos dos pacientes, cobertura de seguradoras de saúde, visitas hospitalares e custos.

O dataset é fornecido pela Maven Analytics, em um ambiente chamado de "Data Playground", nesse endereço:
[https://mavenanalytics.io/data-playground](https://mavenanalytics.io/data-playground).
<br/><br/>
O datasete em questão pode ser encontrado buscando por "Hospital Patient Records". O link direto ao arquivo ZIP do dataset é:

[Dataset: Hospital Patient Records](https://maven-datasets.s3.amazonaws.com/Hospital+Patient+Records/Hospital+Patient+Records.zip)
<br/><br/>

O portal Maven Analytics sugere algumas perguntas a serem respondidas a partir dos dados ali contidos:

- Quantos pacientes foram admitidos os readmitidos ao longo do tempo?

- Qual é o tempo médio de permanência dos pacientes no hospital?

- Qual é o custo médio por visita?


A essas perguntas, acrescentamos mais algumas para compor o nosso problema:

- Qual o percentual de visitas de homens ou de mulheres?

- Quais os maiores motivos de visitas hospitalares?

- Qual é o gasto hospitalar dos casos em que não há cobertura de seguro?

- Em que localidades moravam os pacientes que procuraram atendimento nos anos de 2020 e 2021, auge da pandemia por COVID-19?

<br/>
Por meio de processos ETL usando a proposta de Arquiterura Medallion, os dados do dataset Hospital Patient Records foram extraídos, carregados em ambiente de nuvem, transformados e armazenados em BD em nuvem ao longo do pipeline da arquitetura: 🥉 Bronze 🥈 Silver 🥇 Gold.
<br/><br/>
A partir da camada Gold, consultas SQL foram realizadas e juntamente com técnicas de vizualização de dados, foi possível chegar às respostas para as questões acima.
<br/><br/>

Navegue para o [📘 Notebook 1](https://github.com/cristianofanchin/puc-rio/blob/main/engenhariadados/1-Download_Dataset_ZIP.ipynb) e acompanhe a jornada do MVP.



