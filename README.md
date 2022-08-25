# Projeto de Loan - PyCaret #

## Descrição Inicial

Durante o projeto, o meu objetivo foi passar pelas etapas de entendimento do problema, ideação da solução, análise dos fatores que poderiam influenciar e, por fim, a etapa de Machine Learning, com um deploy ao final. Com o foco na solução do problema de tomada de empréstimo, na visão da empresa que é responsável pelo empréstimo, busquei solucionar o problema da definição de qual seria o tomador de empréstimo mais adequado, dado os fatores que influenciavam essa decisão. Alguns questionamentos iniciais importantes são:

- Quais os fatores são mais importantes para determinar a decisão de emprestar ou não?

- Como decidir através desses fatores, qual é o tomador de decisão preterido?

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

