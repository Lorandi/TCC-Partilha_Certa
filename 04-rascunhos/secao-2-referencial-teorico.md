# 2 Referencial Teórico

Esta seção reúne os fundamentos conceituais e normativos que sustentam o problema de pesquisa e delimitam o recorte teórico do trabalho. Seu papel é estabelecer, primeiro, a base jurídica mínima do direito sucessório brasileiro; em seguida, explicitar os elementos que compõem a partilha de bens; depois, evidenciar por que esse domínio produz dificuldades práticas de cálculo e conferência; por fim, situar o estudo tanto no contexto da tecnologia aplicada ao Direito quanto no campo da modelagem de domínio e da representação de regras de negócio em sistemas computacionais.

## 2.1 Fundamentos do direito sucessório brasileiro

O direito sucessório brasileiro disciplina a transmissão do patrimônio de uma pessoa após a sua morte, definindo quem pode suceder, em que condições essa sucessão se opera e quais limites jurídicos incidem sobre a destinação dos bens. Em síntese, trata-se do conjunto de regras que organiza a sucessão causa mortis, tanto na hipótese de sucessão legítima quanto na de sucessão testamentária, estabelecendo a continuidade das relações patrimoniais juridicamente transmissíveis (Hironaka 2010; Brasil 2002). Para este trabalho, esse ponto de partida é essencial porque a automação da partilha não lida apenas com operações matemáticas, mas com institutos jurídicos que delimitam a própria composição do problema.

No plano normativo, a abertura da sucessão é o marco jurídico que desencadeia a transmissão da herança. O Código Civil estabelece que, aberta a sucessão, a herança transmite-se desde logo aos herdeiros legítimos e testamentários, consagrando a lógica pela qual a morte do autor da herança produz efeitos imediatos na sucessão patrimonial (Brasil 2002). Na doutrina, esse mecanismo costuma ser relacionado ao princípio da saisine, por meio do qual a titularidade hereditária se projeta automaticamente aos sucessores, ainda que a individualização dos quinhões dependa de inventário e partilha posteriores (Hironaka 2010). Essa distinção é relevante para o TCC porque separa dois momentos que, embora correlatos, não se confundem: a transmissão jurídica da herança e o cálculo concreto de sua divisão.

A sucessão pode decorrer da vontade do autor da herança ou da disciplina legal aplicável ao caso concreto. Quando há testamento válido, a sucessão testamentária permite a manifestação de última vontade dentro dos limites admitidos pelo ordenamento; na ausência de disposição testamentária suficiente, incidem as regras da sucessão legítima, que organizam a chamada ordem de vocação hereditária (Brasil 2002). Nesse sentido, a legislação não apenas identifica os sucessores possíveis, mas também estrutura a precedência entre classes, de modo que descendentes, ascendentes, cônjuge e colaterais ocupam posições distintas conforme a configuração familiar existente (Brasil 2002; Lôbo 2024). Para um sistema computacional, essa ordem não pode aparecer como mera listagem normativa: ela precisa ser traduzida em critérios objetivos de elegibilidade e concorrência entre sujeitos.

Outro fundamento central do direito sucessório brasileiro é a proteção conferida aos herdeiros necessários. O Código Civil define como herdeiros necessários os descendentes, os ascendentes e o cônjuge, assegurando a eles, de pleno direito, metade dos bens da herança, isto é, a legítima (Brasil 2002). A outra metade corresponde, em regra, à parte disponível, sobre a qual pode recair a liberdade de disposição do autor da herança dentro dos limites legais. A literatura contemporânea observa que esse desenho normativo expressa uma tensão permanente entre autonomia privada e solidariedade familiar, pois a sucessão não se organiza exclusivamente em torno da vontade individual, mas também da proteção de vínculos familiares juridicamente qualificados (Tartuce 2020; Ribeiro 2020). Para este TCC, essa tensão importa diretamente porque delimita quais parcelas patrimoniais podem ser objeto de livre destinação e quais parcelas permanecem submetidas a reserva legal.

Assim, os fundamentos do direito sucessório brasileiro que interessam a este estudo podem ser resumidos em quatro eixos: a abertura da sucessão como fato jurídico desencadeador da transmissão hereditária; a distinção entre sucessão legítima e testamentária; a ordem legal de vocação hereditária; e a proteção da legítima dos herdeiros necessários. Esses elementos formam a base conceitual mínima para a etapa seguinte do argumento, que consiste em examinar como tais institutos repercutem sobre a estrutura da partilha de bens e, posteriormente, sobre sua tradução em regras de negócio. Em outras palavras, antes de modelar o cálculo, é necessário definir com precisão quais categorias jurídicas o cálculo deverá respeitar.

## 2.2 Estrutura da partilha de bens

A partilha de bens depende não apenas da identificação dos sucessores, mas também da definição do patrimônio que efetivamente será submetido à sucessão. Para este trabalho, isso é relevante porque o cálculo sucessório exige etapas anteriores à divisão entre herdeiros, especialmente a distinção entre meação, herança, dívidas e restrições legais incidentes sobre o acervo patrimonial.

### 2.2.1 Regimes de bens

Os regimes de bens influenciam diretamente a estrutura da partilha porque determinam como o patrimônio do casal se organiza e quais bens podem ser considerados comuns ou particulares. Em termos computacionais, isso afeta a identificação da parcela que pertence ao cônjuge por direito próprio e da parcela que integrará a herança (Brasil 2002).

#### 2.2.1.1 Comunhão parcial de bens

Na comunhão parcial, em regra, comunicam-se os bens adquiridos onerosamente durante o casamento, enquanto os bens particulares permanecem de titularidade individual. Para o cálculo da partilha, isso significa que parte dos bens pode gerar meação, enquanto outra parte pode compor diretamente a herança, exigindo classificação patrimonial prévia no sistema (Brasil 2002).

#### 2.2.1.2 Comunhão universal de bens

Na comunhão universal, a regra geral é a comunicação mais ampla do patrimônio do casal, ressalvadas as exceções legais. Isso amplia a relevância da meação na estrutura da partilha, pois uma parcela significativa do patrimônio pode pertencer previamente ao cônjuge sobrevivente antes mesmo da apuração da herança (Brasil 2002).

#### 2.2.1.3 Separação convencional de bens

Na separação convencional, o patrimônio de cada cônjuge permanece, em regra, individualizado. Ainda assim, a ausência de comunicação patrimonial não elimina automaticamente os efeitos sucessórios, de modo que a participação do cônjuge na herança deve ser analisada conforme as regras legais aplicáveis ao caso (Brasil 2002).

#### 2.2.1.4 Separação obrigatória de bens

A separação obrigatória de bens também produz efeitos específicos na estrutura sucessória. Para fins de modelagem, o mais importante é reconhecer que esse regime não pode ser tratado da mesma forma que os regimes comunicativos, pois altera a relação entre patrimônio do casal, meação e concorrência sucessória do cônjuge (Brasil 2002).

### 2.2.2 Meação e herança

A meação não se confunde com herança. A primeira decorre do regime de bens e corresponde à parcela patrimonial própria do cônjuge ou companheiro; a segunda corresponde ao acervo transmitido em razão da morte. Essa distinção é central para a automação da partilha porque impede que valores de naturezas jurídicas diferentes sejam tratados como se integrassem a mesma base de cálculo.

### 2.2.3 Concorrência do cônjuge

Em determinados cenários, o cônjuge sobrevivente não apenas recebe a meação, mas também concorre com descendentes ou ascendentes na sucessão. Isso aumenta a complexidade do cálculo porque o mesmo sujeito pode participar do processo em posições diferentes: como titular de patrimônio próprio e como herdeiro. Em um sistema computacional, essa diferença precisa estar explicitamente representada para evitar distorções no resultado final (Brasil 2002).

### 2.2.4 Monte hereditário e dívidas do espólio

Depois de separada a meação, é necessário apurar o monte hereditário, isto é, o patrimônio que será efetivamente submetido à sucessão. Nessa etapa, também devem ser consideradas as dívidas do espólio, que reduzem a base patrimonial disponível para partilha. Isso mostra que o cálculo sucessório depende de uma apuração patrimonial líquida, e não apenas de uma soma bruta de bens e direitos (Brasil 2002).

### 2.2.5 Colação

A colação corresponde ao mecanismo pelo qual determinadas liberalidades recebidas em vida por herdeiros necessários devem ser consideradas no momento da partilha, com o objetivo de preservar equilíbrio na distribuição da herança. Para este trabalho, o ponto mais importante não é aprofundar a discussão doutrinária do instituto, mas registrar que ele interfere diretamente no cálculo sucessório, pois altera a base considerada na definição das quotas entre sucessores. Em termos computacionais, isso significa que o sistema precisa prever situações em que valores anteriormente atribuídos a certos herdeiros influenciam a apuração final da partilha (Brasil 2002).

### 2.2.6 Legítima, parte disponível, testamento e quotas hereditárias

A definição das quotas hereditárias não depende apenas do valor do patrimônio e da quantidade de sucessores, mas também dos limites legais de disposição da herança. Quando houver herdeiros necessários, parte do acervo patrimonial fica reservada à legítima, enquanto a parte disponível pode ser objeto de destinação pelo autor da herança, inclusive por testamento, nos limites previstos em lei (Brasil 2002). Para este TCC, isso é relevante porque mostra que o cálculo sucessório não é uma simples divisão proporcional: ele depende da combinação entre composição patrimonial, posição dos herdeiros e restrições jurídicas que condicionam a distribuição final.

## 2.3 Desafios do cálculo sucessório

O cálculo sucessório apresenta dificuldades que vão além da simples divisão de valores entre herdeiros. A apuração da partilha depende da combinação de múltiplos fatores, como composição familiar, regime de bens, existência de meação, dívidas do espólio, hipóteses de representação, colação e eventuais disposições testamentárias. Isso faz com que o resultado final dependa de uma sequência de decisões interligadas, e não de uma operação isolada (Brasil 2002).

Além das regras jurídicas que afetam o cálculo, a partilha está inserida em um contexto procedimental reconhecido por sua burocracia e dificuldade operacional, o que reforça a importância de soluções que favoreçam organização, consistência e clareza na manipulação das informações sucessórias (Ávila e Mazzei 2021). Em contextos manuais ou pouco padronizados, essa complexidade pode favorecer omissões, inconsistências e retrabalho. Mesmo em atividades jurídicas mais amplas, o uso de planilhas e controles informais tende a apresentar fragilidades relacionadas à atualização dos dados, à inserção incorreta de informações e à dificuldade de conferência dos resultados (Fachini 2021).

Para este trabalho, o principal desafio não está apenas em calcular valores, mas em representar corretamente a lógica do domínio sucessório. Isso exige organizar dados, aplicar regras em ordem coerente e produzir resultados verificáveis. Sob a perspectiva da computação, trata-se de um problema de modelagem e consistência: o sistema precisa transformar regras jurídicas em operações claras, rastreáveis e passíveis de validação, reduzindo ambiguidades e erros operacionais.

## 2.4 Tecnologia aplicada ao Direito: Legaltechs e Lawtechs

A aplicação de tecnologia ao campo jurídico tem se intensificado nos últimos anos, especialmente por meio de soluções voltadas à organização de informações, automação de rotinas e apoio à tomada de decisão. Nesse contexto, os termos Legaltech e Lawtech são comumente utilizados para designar iniciativas tecnológicas direcionadas ao setor jurídico, ainda que a literatura nem sempre adote distinções rígidas entre eles (Santana et al. 2022).

De modo geral, essas soluções procuram responder a demandas por maior eficiência, padronização e acessibilidade em atividades tradicionalmente marcadas por volume informacional, repetição de tarefas e dependência de controle manual. Estudos sobre o tema destacam que a modernização do Direito envolve o surgimento de ferramentas digitais voltadas à gestão, à automação e ao apoio operacional, sem que isso elimine a necessidade de atuação humana na interpretação e validação jurídica (Gomes, Ferreira e Andrade 2022; Santana et al. 2022).

Nesse cenário, o Partilha Certa pode ser compreendido como uma ferramenta de apoio jurídico voltada à organização de dados e à automação de cálculos em um recorte específico do direito sucessório. Para este trabalho, esse enquadramento é importante porque posiciona o sistema no contexto mais amplo da tecnologia aplicada ao Direito, mas preserva a delimitação de escopo adotada no TCC: trata-se de uma solução de apoio à consistência e à precisão operacional, e não de substituição da análise jurídica profissional.

## 2.5 Modelagem de domínio e representação de regras de negócio

### 2.5.1 Modelagem de domínio

Para que um sistema consiga tratar um problema do mundo real, é necessário identificar quais elementos fazem parte desse problema e como eles se relacionam. No contexto deste trabalho, isso significa compreender quais componentes do direito sucessório precisam ser representados no software para que o cálculo da partilha possa ser realizado de forma coerente.

Em termos de desenvolvimento de software, a modelagem de domínio corresponde à organização dos conceitos centrais de um problema de forma compatível com a lógica da aplicação. Essa perspectiva é útil porque orienta a construção do sistema a partir dos elementos e regras que definem o domínio analisado, em vez de tratar a aplicação apenas como um conjunto de telas e operações isoladas (Evans 2003). Neste TCC, essa ideia é aplicada ao contexto da partilha de bens, em que categorias jurídicas e patrimoniais precisam ser traduzidas para uma estrutura lógica compreensível pelo software.

### 2.5.2 Entidades, atributos e relações

A construção de um sistema para partilha de bens exige organizar o domínio em elementos estruturados, como herdeiros, bens, dívidas, regimes de bens e disposições testamentárias. Além de identificar essas entidades, é necessário definir seus atributos e as relações existentes entre elas, como vínculos familiares, titularidade patrimonial e condições de participação na sucessão.

Essa etapa é relevante porque permite organizar o problema em uma estrutura de dados compatível com o sistema. Do ponto de vista da computação, isso significa trabalhar com entidades, relações e atributos que possam ser utilizados nas etapas de cálculo, em vez de depender apenas de descrições textuais do caso (Trujillo et al. 2021).

### 2.5.3 Regras de negócio no contexto sucessório

No caso da partilha, não basta apenas registrar informações. O sistema também precisa aplicar regras que determinam como essas informações devem ser interpretadas e processadas. Isso inclui, por exemplo, regras sobre identificação de sucessores, meação, monte hereditário, concorrência do cônjuge, legítima, colação e testamento.

Dessa forma, as regras de negócio representam a lógica que orienta o comportamento do sistema em cada situação analisada. No contexto deste trabalho, isso é importante porque o resultado do cálculo depende não apenas dos valores patrimoniais informados, mas também da ordem e das condições em que cada regra é aplicada.

### 2.5.4 Tradução das regras jurídicas para o software

A implementação do sistema depende da conversão das regras jurídicas em operações que possam ser executadas de forma clara e verificável. Para este trabalho, isso significa organizar a aplicação das regras em uma sequência coerente, de modo que os dados de entrada, as condições jurídicas e os resultados do cálculo permaneçam consistentes entre si.

Assim, a modelagem não serve apenas para estruturar dados, mas também para permitir que o sistema trate o domínio sucessório de forma operacional. Sob a perspectiva da computação, isso envolve explicitar condições, reduzir ambiguidades e tornar o processamento mais rastreável, o que é importante em um domínio no qual pequenas variações nas entradas ou nas regras podem alterar o resultado final.
