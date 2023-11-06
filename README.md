# TechChallenge3
Repositório criado para o tech challenge 3 do curso de data analytics da FIAP


<h1 align="center">Análise do PNAD COVID19 - IBGE </h1>


<p align="center">
  <a href="">
    <img src="Imagens\covid-cover.jpg"
         alt="version">
  </a>

</p>




## Sumário

- [Objetivo Tech Challenge](#objetivo-do-tech-challenge)
- [Estudo PNAD COVID 19-IBGE](#estudo-pnad-covid-19-ibge)
- [Organização do Banco de dados](#organização-do-banco-de-dados)
- [Características Clínicas dos Sintomas](#métodos-aplicados)
- [Características da População](#modelos-preditivos)
- [Características Economicas da Sociedade](#resultados)
- [Conclusão](#resultados)


# Objetivo do Tech Challenge
Este projeto foi criado para atender os requisitos do projeto Tech Challenge da [Faculdade de Tecnologia - FIAP](https://postech.fiap.com.br/?gclid=Cj0KCQjwnf-kBhCnARIsAFlg49228y9z3y6lf_mWZEekgcxZRZBDavxtRT-zAUNs33TZOJtXpGVMNlAaAue5EALw_wcB).<br>
O Desafio consistia em analisar uma base de dados do IBGE a respeito da COVID 19, e trazer os principais indicadores de planejamento que um hospital deveria ter, mediante um novo surto da doença.
A respeito do estudo, o IBGE entrevistou milhares de brasileiros, afim de obter informações clínicas/socioeconômicas a respeito da população durante a pandemia da covid-19 que ocorreu em 2020.
O desafio precisava cumprir os critérios abaixo:
- Analise da base histórica disponibilizada no site do IBGE;
- Escolha de até 20 perguntas da base extraída;
- Organização da base em um banco de dados de BigData;
- Estudo e apresentação das características clínicas dos sintomas/ da população e da ecônomia da sociedade na época.
- E ainda, precisava responder à seguinte pergunta: "Quais as principais medidas que o hospital deverá tomar em caso de um novo surto de COVID-19?" 

# Estudo PNAD COVID 19-IBGE

A fonte de dados utilizada no projeto se encontra disponível em :(https://covid19.ibge.gov.br/pnad-covid/).<br>
O estudo foi realizado pelo IBGE coletando informações entre maio/2020 e novembro/2020, e possuía o objetivo de medir a influência da pandemia do coronavírus no mercado de trabalho brasileiro, além de produzir informações relacionadas aos sintomas de gripe, e às comorbidades que a população apresentava na época. 
A pesquisa apresentou resultado relevante a respeito da importancia do auxílio emergencial do governo, do modelo de trabalho e como a população lidou com os sintomas apresentados.

Ela contou com mais de 200 perguntas a cada entrevistado, separadas pelas categorias: 

-Identificação e Controle (Perguntas gerais a respeito da UF do entrevistado, região, data da entrevista, etc);
-Características gerais dos moradores (Perguntas gerais a respeito de idade, sexo, etnia, escolaridade, etc);
-COVID19 - Todos os moradores (Questionário a respeito de sintomas que o entrevistado sentiu na última semana, se houve procura de estabeleicmento de saúde, se haviam comorbidades, etc)
-Características de trabalho das pessoas de 14 anos ou mais de idade;
-Rendimento de outras fontes dos moradores de 14 anos ou mais de idade;
-Empréstimos;
-Características da habitação.

Para o projeto, poderíamos escolher perguntas ilimitadas a respeito das categorias:  Identificação e Controle e Características gerais dos moradores, e até 20 perguntas das demais categorias.

Assim, as perguntas utilizadas foram:

-Ano de referência do estudo;
-UF (unidade de federação do entrevistado);
-Semana do mês em que a entrevista ocorreu;
-Número do domicílio;
-Número da entrevista no domicílio;
-UPA;
-Situação do domicílio;
-Idade do Morador;
-Etnia;
-Escolaridade;
-Na semana passada teve febre? (Pergunta 1);
-Na semana passada teve tosse? (Pergunta 2); 
-Na semana passada teve dificuldade para respirar? (Pergunta 3); 
-Por causa disso, foi a algum estabelecimento de saúde? (Pergunta 4); 
-Local que buscou atendimento foi pronto socorro do SUS/UPA? (Pergunta 5); 
-Ao procurar o hospital, teve que ficar internado por um dia ou mais?; (Pergunta 6); 
-Durante a internação, foi sedado, entubado e colocado em respiração artificial com ventilador? (Pergunta 7); 
-Tem algum plano de saúde médico, seja particular, de empresa ou de órgão público? (Pergunta 8); 
-O(A) Sr(a) fez algum teste para saber se estava infectado(a) pelo coronavírus?  (Pergunta 9); 
-Qual o resultado do teste SWAB? (Pergunta 9); 
-Qual o resultado teste de sangue através de furo no dedo? (Pergunta 9);
-Qual o resultado teste de sangue através da veia da braço? (Pergunta 9);
-Algum médico já lhe deu o diagnóstico de asma/bronquite/enfisema/doenças respiratória crônica ou doença de pulmão? (Pergunta 10);
-Qual foi o resultado do teste?  Na semana passada, devido à pandemia do Coronavírus, em que medida o(a) Sr(a) restringiu o contato com as pessoas? (Pergunta 11);
-Na semana passada, por pelo menos uma hora, trabalhou ou fez algum bico? (Pergunta 12);
-Na semana passada, estava temporariamente afastado de algum trabalho? (Pergunta 13);
-No trabalho (único ou principal) que tinha nessa semana, era: (Pergunta 14); 
-Quanto recebia (ou retirava) efetivamente em todos os seus trabalhos?(Pergunta 15);
-Número da faixa do rendimento/retirada em dinheiro;(Pergunta 15);
-Na semana passada, o(a) Sr(a) estava em trabalho remoto (home office ou teletrabalho)?(Pergunta 16);
-Auxílios emergenciais relacionados ao coronavirus? (Pergunta 17);
-Durante o período da pandemia alguém deste domicílio solicitou algum empréstimo?  (Pergunta 18);
-No seu domicílio há os seguintes itens básicos de limpeza e proteção: máscaras ? (Pergunta 19);
-No seu domicílio há os seguintes itens básicos de limpeza e proteção: sabão ou detergente? (Pergunta 20);



Observações: conforme apontado pelos professores nas Lives realizadas, nós poderíamos utilizar a pergunta "Realizou o teste de covid?; Qual foi o resultado?" como uma pergunta só;
Mas como na base havia a pergunta genérica se o entrevistado realizou o teste, mas ela não havia resposta direta, utilizamos um compliado das respostas de cada teste indivual, para poder respondê-la;

Além disso, consideramos que a pergunta "Recebia pela atividade remuerada realizada " e "Faixa Valor da atividade" também podem ser consideradas como uma só.


# Organização do Banco de dados



<p align="center">
  <a href=" ">
    <img src="Imagens\Fechamento Ibovespa últimos 10 anos.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>



# Métodos aplicados


# Modelos preditivos
