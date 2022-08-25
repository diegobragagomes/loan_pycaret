# Projeto de Loan - PyCaret #

## Descrição Inicial

Durante o projeto, o meu objetivo foi passar pelas etapas de entendimento do problema, ideação da solução, análise dos fatores que poderiam influenciar e, por fim, a etapa de Machine Learning, com um deploy ao final. Com o foco na solução do problema de tomada de empréstimo, na visão da empresa que é responsável pelo empréstimo, busquei solucionar o problema da definição se o empréstimo deveria ser aceito ou não, dado os fatores que influenciavam essa decisão. Alguns questionamentos iniciais importantes são:

- Quais os fatores são mais importantes para determinar a decisão de emprestar ou não?

- Como decidir através desses fatores, o empréstimo deve ser aprovado ou não??

Disponibilizei ao final do projeto o modelo preditivo para a verificação se é um tomador viável de empréstimo ou não, baseado nos diversos atributos como gênero, estado civil, quantidade que quer tomar de empréstimo, histórico de crédito, entre outros.

Para que a solução fosse entregue, foram utilizadas algumas tecnologias na Análise de Dados e Machine Learning, tais como **Pandas, Scikit-Learn, PyCaret, AutoViz, Gradio**.

Para as etapas de análise e Machine Learning, utilizou-se extensamente as possibilidades das bibliotecas **Pandas e Scikit-learn**, passando pelo entendimento dos dados, através dos dataframes, transformações nesses dados e por fim a separação e tratamento deles para que os algoritmos de machine learning fossem utilizados. Ainda foi usada a ferramenta **AutoViz**, que assim como Pandas-Profiling e o SweetViz, possibilita a análise gráfica de forma rápida e dinâmica, através de relatório HTML ou pelo próprio notebook. Houve, ainda, o uso do **PyCaret**, ferramenta interessante no que tange o AutoML (processos de machine learning mais automatizados), no qual pude comparar diversos algoritmos de machine learning de maneira bastante ágil e prática. Finalizando o projeto com a implementação do **Gradio**, criando um mini app para que se pudesse interagir com novos dados e ver o modelo escolhido de machine learning funcionando, além de possuir uma integração simples com o **PyCaret**.

## Etapas do Projeto

**Descrição das Variáveis**:

Loan_ID	 - ID único

Gender - 	Gênero( Masculino / Feminino)

Married	 - Aplicante é casado? (Sim/Não)

Dependents -	Número de Dependentes

Education	 - Grau de Educação do Aplicante (Pós-graduação/ Graduação)

Self_Employed	 - Autônomo (Sim/Não)

ApplicantIncome	- Receita do Aplicante

CoapplicantIncome -	Receita do Coaplicante

LoanAmount	- Valor do empréstimo (em milhares)

Loan_Amount_Term	- Tempo de empréstimo (em meses)

Credit_History	- Histórico de crédito

Property_Area	- Urbana/ Semi Urbana/ Rural

Loan_Status	- Empréstimo Aprovado (Sim/Não)

*
**Durante a etapa de Análise de Dados foram descobertos diversos insights**:

- Correlação positiva entre a Receita do Aplicante e o Valor do Empréstimo

- Correlação negativa entre o Empréstimo ser aprovado ou não e o Histórico de Crédito

- Corroborando com a questão anterior, os que tem Histórico de Crédito positivo, possuem maior chance de ter seu empréstimo aprovado

- A maioria das pessoas nos dados não possui dependentes e não estão trabalhando como autônomos

- Dos dados observados, há uma maioria de casados e pós-graduados

- Os casados apresentam valores maiores de Receita do Aplicante do que os solteiros

- Os Valores de Empréstimo e de Receita do Aplicante são maiores em homens do que em mulheres

Para a estimativa com o objetivo de predizer se o empréstimo será aceito ou não foi implementado um modelo utilizando um blend (mistura) dos algoritmos **KNN e Logistic Regression** que atingiu uma performance de **Precisão em 0.835**. Escolhi a Precisão, pois a Acurácia, em modelos desbalanceados, nem sempre entrega resultados muito bons. Além disso, o foco na Precisão se faz por conta do resultado que se deseja obter, já que deixar um falso positivo passar é muito custoso para o banco ou unidade que está disponibilizando o empréstimo, por isso o foco na redução desses falsos positivos nos leva a utilizar o valor de Precisão nos modelos.

Através desse projeto foi possível praticar e implementar conceitos importantes da **Ciência de Dados** e propor uma solução para um problema latente e recorrente em bancos e empresas que prestam o serviço de empréstimo para a população, através da **Análise de Dados** dos dados financeiros e pessoais e criação de um modelo de **Machine Learning**.

Como um processo de melhoria contínua pode ser desenvolvido uma automação para executar pipeline de coleta e transformação de dados como automatizar os passo da etapa de Machine Learning e Deploy. ALém disso, poderia ser incluído todo o processamento na nuvem.

