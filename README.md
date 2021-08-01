# TCC 
### PONTIFÍCIA UNIVERSIDADE CATÓLICA DE MINAS GERAIS
#### NÚCLEO DE EDUCAÇÃO A DISTÂNCIA
#### Pós-graduação Lato Sensu em Ciência de Dados e Big Data


#### Aluno: Geraldo Augusto de Morais Figueiredo

## O USO DE DADOS DE VARIAÇÃO DE MOBILIDADE URBANA NA PREVISÃO DE NÚMEROS DE CASOS DE COVID-19 


### Entendimento do problema
#### É possível prever aumento ou diminiução de número de casos confirmados de Covid a partir dos dados de mobilidade e média móvel de 14 dias de número de casos confirmados de um município?

Nesse trabalho espera-se que, a partir dos dados de mobilidade de municípios do Brasis, possa ser possível prever aumento ou diminuição de número de casos de Covid-19. 

Os dados de mobilidade são obtidos nos datasets do [Relatórios de mobilidade da comunidade do Goolge](https://www.google.com/covid19/mobility/). Nele são mostrados a variação percentual de mobilidade ao esperado pela médias que o dataset tem.

Já os dados de notificações de casos de Covid-19 são do [Ministério da Saúde](https://dados.gov.br/dataset/casos-nacionais).

Nesse trabalho, o corte feito foi do Brasília-DF, Belo Horizonte-BH, Porto Alegre-RS, Manaus-AM e Salvador-BA e foi utilizado a informação de variação da mobilidade de transporte público, locais de trabalho e locais residênciais.


### Importação das bases
As bases foram obtidas nos seguintes links<br>
- [dados-mg-1](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-mg-1.csv) <br>
- [dados-mg-2](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-mg-2.csv)<br>
- [dados-mg-3](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-mg-3.csv)<br>
- [dados-mg-4](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-mg-4.csv)<br>
- [dados-df](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-df.csv)<br>
- [dados-rs-1](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-rs-1.csv) <br>
- [dados-rs-2](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-rs-2.csv)<br>
- [dados-rs-3](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-rs-3.csv)<br>
- [dados-rs-4](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-rs-4.csv)<br>
- [dados-am](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-am.csv)<br>
- [dados-ba-1](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-ba-1.csv) <br>
- [dados-ba-2](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-ba-2.csv)<br>
- [dados-ba-3](https://s3-sa-east-1.amazonaws.com/ckan.saude.gov.br/dados-ba-3.csv)<br>

Foi selecionado o período de 19/02/2020 até 30/06/2021 das notificações de Covid-19<br>
O dado de mobilidade selecionado foi a variação percentual de mobilidade das estações de tranporte público
