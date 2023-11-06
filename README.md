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
- [Características Clínicas dos Sintomas](#características-clínicas-dos-sintomas)
- [Características da População](#características-da-população)
- [Características Economicas da Sociedade](#características-economicas-da-sociedade)
- [Conclusão](#conclusão)


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

A fonte de dados utilizada no projeto se encontra disponível em :(https://covid19.ibge.gov.br/pnad-covid/).<br></p>
O estudo foi realizado pelo IBGE coletando informações entre maio/2020 e novembro/2020, e possuía o objetivo de medir a influência da pandemia do coronavírus no mercado de trabalho brasileiro, além de produzir </p>informações relacionadas aos sintomas de gripe, e às comorbidades que a população apresentava na época. </p>
A pesquisa apresentou resultado relevante a respeito da importancia do auxílio emergencial do governo, do modelo de trabalho e como a população lidou com os sintomas apresentados.</p>
</p>
</p>

Ela contou com mais de 200 perguntas a cada entrevistado, separadas pelas categorias: </p>

- Identificação e Controle (Perguntas gerais a respeito da UF do entrevistado, região, data da entrevista, etc);
- Características gerais dos moradores (Perguntas gerais a respeito de idade, sexo, etnia, escolaridade, etc);
- COVID19 - Todos os moradores (Questionário a respeito de sintomas que o entrevistado sentiu na última semana, se houve procura de estabeleicmento de saúde, se haviam comorbidades, etc);
- Características de trabalho das pessoas de 14 anos ou mais de idade;
- Rendimento de outras fontes dos moradores de 14 anos ou mais de idade;
- Empréstimos;
- Características da habitação.

Para o projeto, poderíamos escolher perguntas ilimitadas a respeito das categorias:  Identificação e Controle e Características gerais dos moradores, e até 20 perguntas das demais categorias.</p>

Assim, as perguntas utilizadas foram:</p>

- Ano de referência do estudo;
- UF (unidade de federação do entrevistado);
- Semana do mês em que a entrevista ocorreu;
- Número do domicílio;
- Número da entrevista no domicílio;
- UPA;
- Situação do domicílio;
- Idade do Morador;
- Etnia;
- Escolaridade;
- Na semana passada teve febre? (Pergunta 1);
- Na semana passada teve tosse? (Pergunta 2); 
- Na semana passada teve dificuldade para respirar? (Pergunta 3); 
- Por causa disso, foi a algum estabelecimento de saúde? (Pergunta 4); 
- Local que buscou atendimento foi pronto socorro do SUS/UPA? (Pergunta 5); 
- Ao procurar o hospital, teve que ficar internado por um dia ou mais?; (Pergunta 6); 
- Durante a internação, foi sedado, entubado e colocado em respiração artificial com ventilador? (Pergunta 7); 
- Tem algum plano de saúde médico, seja particular, de empresa ou de órgão público? (Pergunta 8); 
- O(A) Sr(a) fez algum teste para saber se estava infectado(a) pelo coronavírus?  (Pergunta 9); 
- Qual o resultado do teste SWAB? (Pergunta 9); 
- Qual o resultado teste de sangue através de furo no dedo? (Pergunta 9);
- Qual o resultado teste de sangue através da veia da braço? (Pergunta 9);
- Algum médico já lhe deu o diagnóstico de asma/bronquite/enfisema/doenças respiratória crônica ou doença de pulmão? (Pergunta 10);
- Qual foi o resultado do teste?  Na semana passada, devido à pandemia do Coronavírus, em que medida o(a) Sr(a) restringiu o contato com as pessoas? (Pergunta 11);
- Na semana passada, por pelo menos uma hora, trabalhou ou fez algum bico? (Pergunta 12);
- Na semana passada, estava temporariamente afastado de algum trabalho? (Pergunta 13);
- No trabalho (único ou principal) que tinha nessa semana, era: (Pergunta 14); 
- Quanto recebia (ou retirava) efetivamente em todos os seus trabalhos?(Pergunta 15);
- Número da faixa do rendimento/retirada em dinheiro;(Pergunta 15);
- Na semana passada, o(a) Sr(a) estava em trabalho remoto (home office ou teletrabalho)?(Pergunta 16);
- Auxílios emergenciais relacionados ao coronavirus? (Pergunta 17);
- Durante o período da pandemia alguém deste domicílio solicitou algum empréstimo?  (Pergunta 18);
- No seu domicílio há os seguintes itens básicos de limpeza e proteção: máscaras ? (Pergunta 19);
- No seu domicílio há os seguintes itens básicos de limpeza e proteção: sabão ou detergente? (Pergunta 20);



Observações: conforme apontado pelos professores nas Lives realizadas, nós poderíamos utilizar a pergunta "Realizou o teste de covid?; Qual foi o resultado?" como uma pergunta só;
Mas como na base havia a pergunta genérica se o entrevistado realizou o teste, mas ela não havia resposta direta, utilizamos um compliado das respostas de cada teste indivual, para poder respondê-la;

Além disso, consideramos que a pergunta "Recebia pela atividade remuerada realizada " e "Faixa Valor da atividade" também podem ser consideradas como uma só.


# Organização do Banco de dados

O banco de dados escolhido para armazenar os dados foi o Google BigQuery.</p>

Inicialmente fizemos o download dos arquivos mensais do IBGE de: set/20,out/20 e nov/20.</p>
Tratamos os 3 arquivos para que ficassem com a mesma quantidade de colunas e com os dados padronizados.</p>
Importamos os arquivos para um Bucket criado na Google Cloud Storage. </p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Bucket-Google-cloud-Storage.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Depois, criamos um conjunto de dados no BigQuery, e posteriormente incluimos os dados do Google Storage em uma tabela nesse conjunto de dados.

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_tabela_BigQuery.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_tabela_BigQuery_2.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

A tabela criada com os dados brutos, ficou com as seguintes configurações:

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_tabela_BigQuery_3.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_tabela_BigQuery_4.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Depois disso, utilizando do editor de querys, criamos uma view a partir da tabela de dados brutos.
A view já possuía as colunas com uma nomenclatura mais adequada e até algumas transformações de dados realizadas.

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_view_BigQuery.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Criando_view_BigQuery2.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Posteriormente, conectamos o banco de dados no Python, para algumas analises.

<p align="center">
  <a href=" ">
    <img src="Imagens\Conexao-Python-BigQuery.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Conexao-Python-BigQuery2.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Conexao-Python-BigQuery2.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

E por fim, conectamos o BigQuery em uma ferramenta de BI (PowerBi):

<p align="center">
  <a href=" ">
    <img src="Imagens\Conexao-Powerbi-BigQuery.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Conexao-Powerbi-BigQuery2.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

# Características Clínicas dos Sintomas

A respeito da ánalise clínica dos sintomas, começamos com a distribuição da população que teve algum dos seguintes sintomas: Febre, tosse ou dificuldades respiratórias.</p>
Cerca de 1.83% da população relata ter tido pelo menos um dos sintomas descritos acima.</p>
Como podemos observar no gráfico abaixo, não houve concentração de sintomas por idade.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\Grafico_sintomas_idade.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

O segundo aspecto analisado foi o número de pessoas que procuraram um atendimento médico. </p>
Analisamos se as pessoas que possuiam plano de saúde procuraram atendimento em pronto socorro da UPA ou do SUS (público).</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_plano_saude_atendimento.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

- 98.98% dos entrevistados não procuraram atendimento;
- 0.81% dos entrevistados procuraram atendimento em estabelecimento privado ou relacionado às forças armadas;
- 0.21% procuram atendimento em pronto socorro do SUS/UPA (sendo que 15% dessas pessoas possuíam plano de saúde e poderiam ter recorrido à um hospital privado);

Se considerarmos apenas as pessoas que possuíam manifestaram algum dos sintomas (febre, tosse ou dificuldade em respirar), 61% não procurou um estabelecimento de saúde para resolver seu problema. Isso pode ter ocorrido devido alguns fatores: </p>
-Individuo não possuía plano de saúde (representavam 49% dos 61%) e não quis procurar hospital público;  
-individuo não sentiu que seus sintomas eram significativos o sucifiente ou, pode ter sentido que a coparticipação do convênio não valeria a pena.</p>

  <p align="center">
  <a href=" ">
    <img src="Imagens\grafico_plano_saude_atendimento_sintomas.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

A próxima característica analisada foi a % de pessoas que testaram positivo por UF:</p>

 <p align="center">
  <a href=" ">
    <img src="Imagens\grafico_teste_positivo.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>
Pelo gráfico, podemos ver que os estados que mais tiveram testes positivos para COVID foram: São Paulo (6.82%), Rio de Janeiro (6.61%), Maranhão (6.59%),  Goiás (6.24%).</p>
Relacionando esses dados com os estados que mais fizeram teste, vemos que a taxa de casos positivos/população testada de Roraima é uma das mais altas, sendo que 49% da população testada, tiveram um resultado positivo. E São Paulo, tendo umas taxas mais baixas, provavelmente devido seu investimento na compra de testes, que aumentou o número de pessoas que podiam realizá-lo.</p>
Além disso, observamos que os estados com as maiores taxas de casos positivos sobre a população testada, são os etados do Norte: Roraima, Amapá, Acre. Esses estados, segundo IBGE (https://www.ibge.gov.br/explica/pib.php)
possuíram os menores PIB em 2020. Assim, podemos entender que não havia investimento disponível para compra de teste, e portanto apenas casos prioritários eram testados.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_taxa.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Posteriormente, analisamos se as pessoas respeitaram a restrição da quarentena.</p>
Sabemos que a COVID foi uma doença viral que se espalhava através do ar, e que uma das medidas para sua contenção foi a quarentena, onde era indicado à população que permanecessem em casa, evitando a disseminação do vírus.</p>
Os resultados observados indicam que a população seguiu, quando possível, as orientações de restrição.</p>
Apenas 4% dos entrevistados não se preocuparam em permanecer na quarentena. E embora 2.35% dos entrevistados tenha saído de casa para trabalho ou necessidades básicas, mesmo após testando positivo para a doença, 53.3% da população ficou rigorosamente em casa, ou saiu apenas em necessidade essencial.</p>
<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_restricao_resultado.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>


# Características da População

Sobre a amostra de população, começamos analisando sexo e idade:</p>
<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_restricao_resultado.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>
Podemos ver pelo gráfico acima, que nossa amostra está bem distibuída entre ambos os genêros e possuí concentração de idade entre 20 e 60 anos. Sendo que a média de idade é próxima dos 40 anos, em ambos os sexos.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\BoxPlot.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

A escolaridade da amostra também foi outro fator analisado. Vemos que cerca de 33% da amostra não possuía ensino fundamental completo.</p>
22% haviam concluído o ensino médio e 1.6% haviam realizado algum tipo de especialização. </p>
Além disso, 41% dos entrevistados eram pessoas brancas, 49% eram pardas, 8% eram pretas e 0.59% eram indígenas. </p>
Esses dados vão de encontro com os reportados pelo IBGE. Segundo estudo realizado pelo órgão (https://educa.ibge.gov.br/jovens/conheca-o-brasil/populacao/18319-cor-ou-raca.html), em 2022 42,8% da população era branca, 10.6% era preta e 45.3% era parda.
Assim, vemos que a entrevista não foi tendenciosa e relatou a realidade da população brasileira.

<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_escolaridade_etnia.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

As regiões que possuíam mais coincidiam com as regiões com mais populosas do Brasil: Sudeste, Nordeste e Sul, sendo que o Nordeste apresentou quase metade de sua população em zona rural.</p>
Segundo o IBGE, o nordeste é uma das regiões com a taxa de urbanização mais baixa do país (https://www.ibge.gov.br/estatisticas/sociais/populacao/17374-indicadores-sociais-minimos.html).
<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_regiao_situacao_domiciliar.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Analisando a renda das pessoas com atividade remunerada com base no sexo, 65% recebiam renda de até R$1600,00. Sendo salário mínimo na época cerca de R$1045,00, vemos que a grande maioria da população tinha cerca de 1 salário minimo como renda. Além disso também observamos que a % de homens no mercado de trabalho é maior do que a de mulher. 58% das pessoas com atividade remunerada eram homens e 42% eram mulheres.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_renda_sexo.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Outros aspecto analisado foi o plano de saúde da população. Dado que o plano de saúde possibilita acesso a hospitais de iniciativa privada, observamos que cerca de 22% da população, sem concentração de idade, possuíam algum tipo de convênio médico. Isso significa que pelo menos mais de 70% dos entrevistados iriam procurar atendimento em hospitais públicos, sobrecarregando assim o sistema de saúde.

<p align="center">
  <a href=" ">
    <img src="Imagens\Grafico_plano_saude_idade.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>


Além disso, devemos levar em conta os estados em que estão mais concentrados a poplação que conta com convênios. 
Os estados do sudeste (São Paulo, Rio de Janeiro Distrito Federal) possuem taxa maior de pessoas com planos de saúde, enquanto que os estados do norte (Roraima, Maranhão e Amazonas) são os estados com os menores indices.
É um fator que pode ser associado ao IDH dos estados (https://socientifica.com.br/estados-brasileiros-com-os-maiores-idh/), quanto maior o indice de desenvolvimento humano, maior a taxa de população com acesso a condições melhores de saúde, por exemplo.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\grafico_uf_plano_saude.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>
Finalizando a analise das caracteristicas da população, temos um gráfico onde mostramos que mais de 99% da população possuía acesso a itens fundamentais de higiene, para contenção do vírus: Mascaras e Sabão/detergente.</p>
Na época da pandemia, a sociedade era não só instruída a não sair sem mascara e utilizar detergente/sabão para lavar as mãos, como haviam leis que tornavam a utilização da macára obrigatória em diversos estados, como forma de prevenir a disseminação do vírus. 
<p align="center">
  <a href=" ">
    <img src="Imagens\Grafico_higiene.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>


# Características Economicas da Sociedade
Sobre as caracteríticas econômicas da sociedade, inciamos os estudos analisando a % da população que teve acesso ao auxilio emergencial que o governo proporcionou durante a época do COVID.</p>
O auxilio foi distribuído pelo governo, e para o cidadão receber precisava cumprir os requisitos abaixo: ter mais de 18 anos, ser de família com renda mensal per capita (por pessoa) de até meio salário mínimo (R$ 522,50) ou renda familiar mensal total de até três salários mínimos (R$ 3.135), além de não ter tido rendimentos tributáveis, em 2018, acima de R$ 28.559,70.</p>

Através do gráfico, podemos ver que diversas pessoas que não realizavam atividade remunerada ou que possuíam salário com menos de R$1600,00 não receberam auxilio. Vale lembrar que o auxilio não contemplava pessoas que recebiam mais de meio salário minimo, que já eram beneficiários do bolsa família e o auxilio era de apenas um integrante por família.
Ou seja, poderíamos ter estudo a distribuição do auxilio para um público maior de pessoas que principalmente trabalhavam por conta própria, ou que estavam fora do mercado de trabalho por cuidarem de pessoas com condições especiais em casa, ou ainda que fossem trabalhadores domésticos que poderiam ter tido um impacto maior com as medidas de quarentena impostas na época.</p>

<p align="center">
  <a href=" ">
    <img src="Imagens\auxilio_emergencial_governo.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Sobre a taxa de descoupação na época, cerca de 14% das pessoas entrevistadas (e consideramos apenas maiores de 14 anos, assim como o IBGE), estavam sem realizar atividade remunerada na época.</p>
<p align="center">
  <a href=" ">
    <img src="Imagens\taxa_descoupação.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Devido as medidas de restrição social, muitas das empresas tiveram que recorrer à mediadas extremas para sobreviver como: afastar funcionários ou demití-los. Muitas das pessoas que trabalhavam de forma autonoma ouq ue dependiam de doações tiveram que suspender suas atividades. 
Abaixo realizamos uma comparação entre as pessoas que pediram um empréstimo durante a época da pandemia.</p>
A maioria se encontrava sem realizar atividades remuneradas e conseguiram ter o empréstimo aprovado.</p>
<p align="center">
  <a href=" ">
    <img src="Imagens\emprestimo.PNG" alt="webapp-architecture">
  </a>
  <caption style="font-size: smaller; text-align: center;">Figura 1</caption>
</p>

Por último, analisamos 

# Conclusão
