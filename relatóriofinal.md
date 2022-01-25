# Inferência-Estatistica-Sobre-Hábitos-Saudáveis-e-Depressão
DESAFIO INFERÊNCIA HÁBITOS SAUDÁVEIS X DEPRESSÃO

- Introdução:

Realizei esse desafio durante o bootcamp da Tera em Data Science e Machining Learning. Os bancos de dados são provenintes de uma pesquisa feita nos Estados Unidos chamada "National Health and Nutrition Examination Survey (NHANES)". Nesse sentido, os objetivos principais da análise são: avaliar o perfil de indivíduos (adultos maiores de 18 anos) com sintomas depressivos nos EUA no período de 2005-2006, e se hábitos saudáveis de alimentação e atividade física estão associados a menores índices de depressão nesta população. Para isso, foi necessário a análise de vieses e da possível causalidade entre hábitos e a doença referendada. Escrever aqui a conclusão da análise

- Sobre os bancos de dados:
  
 -NHANES:

O National Health and Nutrition Examination Survey (NHANES) é uma pesquisa anual conduzida pelo National Center for Health Statistics (NCHS) do Centro de Controle e Prevenção de Doenças (Centers for Disease Control - CDC) para avaliar a saúde e nutrição de adultos e crianças dos Estados Unidos. Dados coletados incluem questões demográficas, socioeconômicas, dietéticas e relacionadas à saúde, com o componente de exame contendo medidas médicas, odontológicas, fisiológicas e exames laboratoriais.

A pesquisa examina uma amostra de cerca de 5.000 pessoas a cada ano, selecionada à partir de amostragem complexa a fim de selecionar uma amostra representativa da população civil não institucionalizada dos EUA. Sendo assim, as análises utilizando este estudo devem ser realizadas utilizando técnicas e ferramentas que levem em conta a amostragem complexa.

Neste desafio, no entanto, iremos assumir que os dados foram obtidos usando uma amostra aleatória da população de interesse e utilizaremos técnicas e ferramentas de análise usuais para amostras aleatórias para fins didáticos.
  
  -PHQ_9:

O Patient Health Questionnaire-9 (PHQ-9) é um instrumento utilizado para avaliar o grau de depressão em pacientes. O questionário consiste de 9 itens em que os respondentes indicam a frequência (0 = “nenhuma vez”, 1 = “menos de uma semana”, 2 = “uma semana ou mais” e 3 = “quase todos os dias”) de sintomas de depressão nas duas últimas semanas.
O PHQ-9 inclui os seguintes itens para a pergunta “Nas últimas 2 semanas, com que frequência você ficou incomodado por algum dos problemas a seguir?” (0 = “nenhuma vez”, 1 = “menos de uma semana”, 2 = “uma semana ou mais” e 3 = “quase todos os dias”):
1 - Pouco interesse ou pouco prazer em fazer as coisas
2 - Se sentiu para baixo, deprimido(a) ou sem perspectiva
3 - Dificuldade para pegar no sono ou permanecer dormindo ou dormiu mais do que o costume
4 - Se sentiu cansado(a) ou com pouca energia
5 - Falta de apetite ou comeu demais
6 - Se sentiu mal consigo mesmo(a) ou achou que é um fracasso ou que decepcionou sua família ou a você mesmo(a)
7 - Dificuldade para se concentrar nas coisas (como ler o jornal ou ver televisão)
8 - Teve lentidão para se movimentar ou falar (a ponto de outras pessoas perceberem), ou ao contrário, esteve tão agitado(a) que você ficava andando de um lado para o outro mais do que costume
9 - Pensou em se ferir de alguma maneira ou que seria melhor estar morto(a)
O escore total é calculado à partir da soma dos itens 1-9 e varia de 0 a 27, em que maiores valores do escore indicam maiores frequências de sintomas de depressão. Aqueles com pontuação maior ou igual a 5 para o escore total de PHQ-9 são considerados como tendo sintomas leves (5-9), moderados (10-14), moderadamente severos (15-19) e severos de depressão (>= 20). 
  
  -HEI:

O Healthy Eating Index (HEI) é uma medida de qualidade da dieta baseado nas orientações dietéticas do governo federal americano (Dietary Guidelines for Americans). O HEI utiliza diferentes grupos alimentares para o cálculo do escore, variando de 0 a 100, em que maiores valores do escore refletem dietas mais próximas das orientações alimentares em vigor.
O índice é composto por 13 componentes baseados nos grupos alimentares descritos nas recomendações dietéticas.
  -Conclusão:
  
Não foi possível achar correlação positiva entre práticas de exercício, hábitos alimentares e sintomas de depressão. Dessa forma, pode-se entender que o sedentarismo e os hábitos alimentares não são necessariamente os causadores da depressão, mas podem intensificar seus sintomas. Isso pode ser uma das possíveis interpretações para a regressão linear aplicada que retornou "P" valor menor que 0,05 confirmando a existência de efeito entre exercícios físicos e os sintomas, mas não causalidade. A dificuldade de determinar esse tipo de relação entre essas variáveis mencionadas (PHQ9, PAG_MINW, ADHERENCE, HEI2015_TOTAL_SCORE) procede do tipo de estudo feito pelo NHANES que é observacional. Para uma análise ainda mais assertiva, seria interessante aumentar o tempo de observação para as variáveis, bem como avaliar a incidência da doença na família de cada indivíduo e verificar se as pessoas do estudo são ou foram acompanhadas pro profissionais da saúde mental
