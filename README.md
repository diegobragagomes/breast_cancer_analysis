# Projeto Breast Cancer Analysis

## Descrição Inicial

Durante o projeto, o meu objetivo foi passar pelas etapas de entendimento do problema, ideação da solução, análise dos fatores que poderiam influenciar e, por fim, a etapa de Machine Learning. Com o foco na solução do problema de avaliação do tumor, na visão da empresa que é responsável pelo diagnóstico, busquei solucionar o problema de avaliação se o tumor é maligno ou benigno, dada as características que ele apresentava. Alguns questionamentos iniciais importantes são:

- Como avaliar se dado tumor é benigno ou maligno dado as características?

- Essas características são influenciadas pelas demais? Se sim, como?

Disponibilizei ao final do projeto o modelo preditivo para a verificação se o tumor é benigno ou maligno, baseado nas diversas características físicas apresentadas nos dados do problema.

Para que a solução fosse entregue, foram utilizadas algumas tecnologias na Análise de Dados e Machine Learning, tais como **Pandas, Matplotlib, Seaborn, Scikit-Learn, Pandas-Profiling**.

Para as etapas de análise e Machine Learning, utilizou-se extensamente as possibilidades das bibliotecas **Pandas e Scikit-learn**, passando pelo entendimento dos dados, através dos dataframes, transformações nesses dados e por fim a separação e tratamento deles para que os algoritmos de machine learning fossem utilizados. Ainda foi usada a ferramenta **Pandas-Profiling**, que assim como AutoViz e o SweetViz, possibilita a análise gráfica de forma rápida e dinâmica, através de relatório HTML ou pelo próprio notebook. Ademais, foram utilizados o **Matplotlib e o Seaborn** para a realização da parte gráfica do estudo.

## Etapas do Projeto

**Descrição das Variáveis**

id  - ID único

diagnonis - Diagnóstico (M (Maligno), B (Benigno))

Além dessas duas, existem 30 variáveis que descrevem características físicas, enrtre elas raio, textura, perímetro, área, etc. Por conta disso, não serão descritas aqui uma a uma, mas podem ser visualizadas no notebook.

#
**Durante a etapa de Análise de Dados foram descobertos diversos insights**

- Correlação positiva entre diversas características

- Separação bastante nítida entre Maligno e Benigno, de acordo com a distância, entre diferentes características

Para a estimativa com o objetivo de predizer se o tumor é maligno ou benigno foi implementado o modelo de **Regressão Logística** que atingiu uma performance de **Recall em 0.98**. Escolhi o Recall, pois se tratando de um caso médico, é mais interessante para a empresa responsável pelo diagnóstico lidar com os Falsos Negativos, visto que poderiam causar problemas legais quanto a decisões equivocadas.

## Conclusão

Através desse projeto foi possível praticar e implementar conceitos importantes da **Ciência de Dados** e propor uma solução para um problema em empresas de diagnóstico que prestam serviço para a população, através da **Análise de Dados** dos dados de características médicas de um tumor, com a criação de um modelo de **Machine Learning**.

Analisando possíveis melhorias, poderia haver uma inspeção dos outliers utilizando o Isolation Forest, além de uma Feature Selection para reduzir os componentes e gerar um deploy mais adequado com menos features. Outro ponto seria uma automação desse processo como um todo.
