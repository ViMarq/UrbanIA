# UrbanIA

Esse repositório foi criado com propósitos acadêmicos.
Aqui temos um grupo de estudantes que trabalharam juntos durante o 1º semestre de 2023 para aprender sobre Inteligência Artificial e como construir e desenvolvê-la a partir de uma base de dados, além disso, python é a linguagem de programação utilizada para fazer a análise dos dados.

# Fonte

O dataset escolhido pertence ao Kaggle e pode ser encontrado no link abaixo:

https://www.kaggle.com/datasets/crisparada/brazilian-cities

Como fontes de classificação base, o conteúdo estudado está presente nos links abaixo:

https://repositorio.ipea.gov.br/bitstream/11058/5167/6/PPE_v45_n02_%C3%8Dndice_de_Desenvolvimento_Humano.pdf

https://atlassocioeconomico.rs.gov.br/indice-de-desenvolvimento-humano-idh-e-idhm#:~:text=Conforme%20o%20relat%C3%B3rio%20de%20Desenvolvimento,86%C2%AA%2C%20com%20%C3%ADndice%20de%200%2C758

# Variável alvo e colunas consideradas para análise

Nosso projeto tem como objetivo determinar o quão ideal é viver em cada município, com isso em mente, escolhemos dentre as informações disponíveis no dataset "Brazilian Cities" as que definimos como relevantes, são elas: 

IDHM

● Indice de Desenvolvimento Humano

Indicador populacional dividido por intervalo numérico entre 0 e 1, o qual indica o grau de desenvolvimento da cidade baseado em três pilares fundamentais, dos quais tem-se educação, renda per capita e saúde.
A partir disso, definimos esta variável como alvo para nosso estudo de classificação das cidade, que indica quanto mais próximo de zero pior o seu índice e quanto mais próximo de um melhor seu índice.


COMP_E

● Número de instituições de saneamento por município.

Esse dado é escolhido como indicador de saúde populacional dado por saneamento básico, tendo em mente que quanto mais precário for o saneamento de um município, mais propício ele é a epidemias geradas por bactérias e vírus provindas de esgotos. 


COMP_O 

● Número de instituições de segurança social por município.

Usamos essa fonte como forma de medida de segurança municipal, assim podemos definir o quão seguro certo município é, influenciando assim, a qualidade de vida. Vale ressaltar que esses levantamentos foram feitos pelo IBGE desde de 1985 é conhecido pelo CEMPRE (Cadastro Central de Empresas) e não se estende a somente essas empresas, porém, essas são as que definimos como relevantes para o projeto por afetar de maneira direta a vivência em cada município. 


COMP_Q

● Número de companhias de saúde e serviços sociais

O número de hospitais presentes dentro de cada cidade é um importante parâmetro a se levar em consideração já que o IDH é um índice calculado pelo IPEA utilizando-se a qualidade e eficiência da saúde para com a população. Dessa forma, os modelos de IA classificarão os tipos de cidade com maiores dados base. 


GDP_CAPITA

● Produto Interno Bruto (PIB) per capita por município.

O PIB per capita, como o nome sugere, é a divisão do PIB municipal pelo número de habitantes que nele habitam, esse é responsável por definir a riqueza média dos moradores de cada município e, deve considerar porém, que essa média pode ser afetada por uma desigualdade exorbitante na divisão de riqueza. Assim, esse acaba sendo um dado crucial que o nosso projeto utiliza, pois, um país com uma média baixa pode não ser ideal para viver. 


IDHM_Educacao

● Índice de educação por município. 

Sendo essencial para o cálculo do IDH, esse índice foi selecionado como importante para o projeto, visto que este define a qualidade educacional municipal.


IDHM_Longevidade

● Índice de longevidade por município. 

Tal como o anterior, esse índice levantado no Atlas de Desenvolvimento Humano apresenta grande importância na qualidade de vida de um município, tendo em mente que este índice é a expectativa de vida, ele leva em consideração fatores como os apresentados em COMP_O e 
COMP_E, além de outros.

# Glossário

IBGE: Instituto Brasileiro de Geografia e Estatística.
CEMPRE: Cadastro Central de Empresas.
PIB: Produto Interno Bruto.
IDH: Índice de Desenvolvimento Humano.
Ipea: Instituto de Pesquisa Econômica Aplicada.
Pnud: Programa das Nações Unidas para o Desenvolvimento.
PEA: População Economicamente Ativa.

# Processo de desenvolvimento

Quanto a área de análise dos dados do dataset, fizemos o tratamento dos dados que estavam com campos vazios ou nulos para se ter uma melhor precisão para os cálculos e, além disso, a normalização desses dados antes de iniciar sua manipulação de fato.
A partir disso, foram calculadas as médias, medianas e moda, as quais também são conhecidas como medidas de tendência central. Não obstante, fez os cálculos das variações como, por exemplo, desvio padrão, variância, correlação entre outros.

Com o intuito de se verificar a exatidão e o rumo correto de nossa análise, colocamos os resultados em gráficos dos tipos boxplot, scatterplot, histograma, de barras e de linha.

Os três modelos de machine learning aplicados são Árvore de decisão, KNN e Naive Bayes.
Escolheu-se os modelos acima para que fosse possivel fazer a classificação das cidades como ruim, média ou boa para se viver com base nos resultados dos cálculos do IDH.

Quanto a Árvore de decisão, esta consiste geralmente em um começo com um único nó, que se divide em possíveis resultados. Cada um desses resultados leva a nós adicionais, que se ramificam em outras possibilidades.
Existem três tipos de nós: nós de probabilidade, nós de decisão e nós de término e, assim, têm-se a formação de uma árvore.
Ela permite que seja feita a comparação de possíveis ações com base em seus custos, probabilidades e benefícios, além de mapear um algoritmo que prevê a melhor escolha, matematicamente.

Já o K-Nearest Neighbors (KNN) é um modelo de aprendizagem supervisionada, ele é um classificador onde o aprendizado é baseado no quão próximo ou semelhante é um dado do outro. O treinamento é formado por vetores de n dimensões e, dessa forma, a partir do cálculo de distância entre um vetor e outro faz-se a rotulação.

Por último, o Naive Bayes é um algoritmo de classificação de dados, ou seja, a partir da análise da tabela de dados, ele cria classes e oferece uma resposta a partir de critérios estabelecidos. É recomendado para aplicação como filtro, que, no caso do UrbanIA, foi importante para contribuir na classificação das cidades.

Para finalizar, foi feito um comitê que com base nas respostas de cada um dos algoritmos aplicados acima, classificou-se o IDH como baixo, médio e alto e, com isso, apontou se a cidade era ruim, média ou boa.
Separamos em duas vertentes este comitê, na primeira, escreve-se o nome da cidade e a IA classificava com base nas colunas usadas acima especificadas neste readme e exibia seus valores. Na segunda, insere-se valores fictícios para cada uma das colunas acimas especificadas neste readme e a IA exibia a decisão quanto a classificação do IDH e apontamento da cidade com as mesmas três categorias explicadas anteriormente.


# Objetivo

Conforme exposto ao início deste readme, tem-se o objetivo de classificar as cidades brasileiras para decidir qual a melhor para se viver.
Entretanto, em quê isso ajudaria e contribuiria de alguma maneira para a sociedade?

Bem, a ideia é apontar os pilares importantes de infraestrutura para um cidadão viver, como educação, saúde, renda per capita etc, a fim de apresentar aos governantes, daquela cidade, por exemplo, qual desses itens necessitam de investimento para que não só mais pessoas fossem atraídas para certa cidade, como também melhorar as condições de vida das que já moram ali.
