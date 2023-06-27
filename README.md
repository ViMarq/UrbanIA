# UrbanIA

This repository is for academic proposes.
Here we have a group of people that worked together during the semester to learn about Artificial Inteligence and how to build it
from a database, furthermore, python is the programming language applied to analysing data.

The dataset that our group chose belongs to Kaggle and may be found in https://www.kaggle.com/datasets/crisparada/brazilian-cities.

As source to do our classification base may be found in https://repositorio.ipea.gov.br/bitstream/11058/5167/6/PPE_v45_n02_% C3%8Dndice_de_Desenvolvimento_Humano.pdf

https://atlassocioeconomico.rs.gov.br/indice-de-desenvolvimento-human o-idh-e-idhm#:~:text=Conforme%20o%20relat%C3%B3rio%20de%20De senvolvimento,86%C2%AA%2C%20com%20%C3%ADndice%20de%20 0%2C758.

# Our targets to analyse

Nosso projeto tem como objetivo determinar o quão ideal é viver em cada município, com isso em mente, escolhemos dentre as informações disponíveis as que definimos como relevantes, são elas: 


COMP_E

● Número de instituições de saneamento por município.

Esse dado é escolhido como indicador de saúde populacional dado por saneamento básico, tendo em mente que quanto mais precário for o saneamento de um município, mais propício ele é a epidemias geradas por bactérias e vírus provindas de esgotos. 


COMP_O 

● Número de instituições de segurança social por município.

Usamos essa fonte como forma de medida de segurança municipal, assim podemos definir o quão seguro certo município é, influenciando assim, a qualidade de vida. Vale ressaltar que esses levantamentos foram feitos pelo IBGE desde de 1985 é conhecido como CEMPRE (Cadastro Central de Empresas) e não se estende a somente essas empresas, porém, essas são as que definimos como relevantes para o projeto por afetar de maneira direta a vivência em cada município. 


COMP_Q

● Número de companhias de saúde e serviços sociais

O número de hospitais presentes dentro de cada cidade é um importante parâmetro a se levar em consideração já que o IDH é um índice calculado pelo IPEA utilizando-se a qualidade e eficiência da saúde para com a população. Dessa forma, os modelos de IA classificarão os tipos de cidade com maiores dados base. 


GDP_CAPITA

● Produto Interno Bruto (PIB) per capita por município.

O PIB per capita, como o nome sugere, é a divisão do PIB municipal pelo número de habitantes que nele habitam, esse é responsável por definir a riqueza média dos moradores de cada município, se deve considerar porém que essa média pode ser afetada por uma desigualdade exorbitante na divisão de riqueza. Assim, esse acaba sendo um dado crucial que o nosso projeto utiliza, pois, um país com uma média baixa pode não ser ideal para viver. 


IDHM_Educacao

● Índice de educação por município. 

Sendo essencial para o cálculo do IDH, esse índice foi selecionado como importante para o projeto, visto que este define a qualidade educacional municipal.


IDHM_Longevidade

● Índice de longevidade por município. 

Tal como o anterior, esse índice levantado no Atlas de Desenvolvimento Humano apresenta grande importância na qualidade de vida de um município, tendo em mente que este índice é a expectativa de vida, ele leva em consideração fatores como os apresentados em COMP_O e 
COMP_E, além de outros. 


Glossary: 

IBGE: Instituto Brasileiro de Geografia e Estatística. 
CEMPRE: Cadastro Central de Empresas. 
PIB: Produto Interno Bruto. 
IDH: Índice de Desenvolvimento Humano. 
Ipea: Instituto de Pesquisa Econômica Aplicada. 
Pnud: Programa das Nações Unidas para o Desenvolvimento.
PEA: População Economicamente Ativa.
