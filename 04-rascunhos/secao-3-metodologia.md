# 3 Metodologia

A metodologia deste trabalho tem como referência o Design Science Research Process (DSRP), proposto por Peffers et al. (2007). A adoção desse modelo decorre do fato de que a pesquisa está centrada no desenvolvimento e na avaliação de uma solução computacional voltada a um problema prático do domínio sucessório.

## 3.1 Caracterização da pesquisa

Esta pesquisa é de natureza aplicada, pois tem como objetivo desenvolver e avaliar uma solução computacional voltada a um problema prático relacionado ao cálculo de partilha de bens no direito sucessório brasileiro (Wazlawick 2009).

Quanto aos objetivos, o trabalho possui caráter exploratório e descritivo (Wazlawick 2009). É exploratório porque investiga quais elementos do domínio sucessório precisam ser considerados na modelagem do sistema. É descritivo porque organiza esse recorte em termos operacionais, explicitando dados, regras e critérios de cálculo necessários ao funcionamento do Partilha Certa.

Quanto à abordagem, a pesquisa é predominantemente qualitativa na etapa de levantamento e tradução das regras do domínio, pois depende da interpretação de normas e conceitos jurídicos. Ao mesmo tempo, incorpora elementos quantitativos na avaliação, especialmente na comparação entre os resultados produzidos pelo sistema e os resultados obtidos por meios tradicionais de conferência.

## 3.2 Abordagem metodológica orientada por DSRP

O Design Science Research Process (DSRP) foi adotado como referência para organizar a condução deste trabalho, por se tratar de um modelo voltado ao desenvolvimento e à avaliação de soluções tecnológicas na área de sistemas de informação (Peffers et al. 2007; Hevner et al. 2004).

No contexto deste TCC, o uso do DSRP se mostra adequado porque o foco da pesquisa está na construção e validação do Partilha Certa como um sistema computacional aplicado a um problema prático. Com base nesse referencial, o trabalho foi estruturado a partir da identificação do problema, da definição dos objetivos da solução, do desenvolvimento do sistema, de sua demonstração e de sua avaliação.

A adoção do DSRP, contudo, não elimina a necessidade de procedimentos complementares. Como o Partilha Certa opera sobre um domínio jurídico específico, a pesquisa também depende de revisão bibliográfica e documental para delimitar as regras sucessórias consideradas, além da formalização dessas regras em termos computacionais e da avaliação do sistema por meio de cenários simulados.

## 3.3 Procedimentos metodológicos e etapas do trabalho

Os procedimentos metodológicos deste trabalho envolvem revisão bibliográfica e documental, tradução das regras sucessórias para critérios computacionais, desenvolvimento do sistema e avaliação por cenários simulados.

Essas atividades foram organizadas em etapas que acompanham a lógica do DSRP e o processo de desenvolvimento do Partilha Certa.

### 3.3.1 Identificação do problema e motivação

O ponto de partida deste trabalho foi a identificação de um problema prático no cálculo de partilha de bens no direito sucessório brasileiro. Esse processo envolve múltiplas regras jurídicas e cálculos patrimoniais interdependentes, o que pode gerar inconsistências, retrabalho e dificuldade de conferência quando realizado de forma manual ou com apoio limitado de planilhas e controles pouco padronizados.

A complexidade do problema não está apenas na divisão final entre os herdeiros, mas também na necessidade de considerar, em ordem adequada, elementos como regime de bens, meação, monte hereditário, legítima, parte disponível, dívidas do espólio e hipóteses de representação. Além disso, a etapa de distribuição concreta dos bens também pode exigir a comparação entre diferentes propostas de divisão, o que reforça a necessidade de um sistema capaz de organizar visualmente essas alternativas.

A motivação da pesquisa, portanto, está em investigar como esse conjunto de regras pode ser traduzido para um sistema computacional capaz de apoiar esse tipo de cálculo com maior consistência e precisão. Nesse contexto, o Partilha Certa foi definido como objeto de estudo e como sistema a ser desenvolvido e avaliado no trabalho.

### 3.3.2 Definição dos objetivos da solução

A partir do problema identificado, foram definidos os objetivos da solução proposta. De modo geral, o sistema deveria permitir o cadastro estruturado dos dados do inventário, a apuração das bases patrimoniais da partilha e a execução dos cálculos sucessórios necessários, além do apoio à simulação da divisão patrimonial.

Esses objetivos foram definidos com base no problema de pesquisa e nas funcionalidades que o Partilha Certa se propõe a oferecer.

Essa etapa também exigiu a definição do escopo do sistema. Nem toda a complexidade do direito sucessório brasileiro foi incorporada ao trabalho. Foram priorizadas as regras diretamente ligadas ao cálculo e à simulação da partilha, enquanto temas que dependem de validação formal, controvérsia judicial ou interpretação externa aos dados informados pelo usuário permaneceram fora do escopo inicial.

### 3.3.3 Levantamento e tradução das regras do domínio

Na etapa seguinte, foram levantadas as bases teóricas e normativas necessárias para a modelagem do sistema. Para isso, foram combinadas revisão bibliográfica e pesquisa documental.

A revisão bibliográfica forneceu a base conceitual sobre direito sucessório, estrutura da partilha, desafios do cálculo sucessório, modelagem de domínio e regras de negócio. A pesquisa documental concentrou-se principalmente na legislação aplicável e na documentação técnica do próprio Partilha Certa, utilizada para descrever o sistema e verificar quais regras e funcionalidades efetivamente fazem parte de seu escopo.

Com base nesse material, as regras selecionadas foram primeiro descritas em linguagem natural e depois traduzidas para critérios computacionais. Isso envolveu definir quais dados o sistema precisa receber, em que ordem determinadas regras devem ser aplicadas e quais resultados são esperados em diferentes composições patrimoniais e familiares.

Essa etapa é central no trabalho, pois é nela que ocorre a passagem do domínio jurídico para sua representação em lógica de sistema. É também nesse momento que são definidas decisões relevantes para o motor de cálculo, como os dados necessários para o processamento, a ordem de aplicação das regras e os critérios adotados nos cenários sucessórios considerados.

### 3.3.4 Design e desenvolvimento do sistema

Após o levantamento e a tradução das regras do domínio, será realizado o desenvolvimento do Partilha Certa, com foco na implementação do motor de cálculo e das funcionalidades necessárias para sua operação.

Nessa etapa, serão estruturados os principais elementos do sistema, como herdeiros, bens, dívidas, vínculos sucessórios, disposições testamentárias e regimes de bens. A partir dessa base, serão implementadas as rotinas relacionadas à separação patrimonial, à apuração da meação, do monte hereditário e das quotas hereditárias, bem como à simulação da divisão dos bens.

### 3.3.5 Demonstração do sistema

A etapa de demonstração prevê a execução do Partilha Certa em cenários sucessórios delimitados. Nessa etapa, serão observados o preenchimento dos dados, a aplicação das regras e a geração dos resultados, de modo a evidenciar o funcionamento do sistema antes da avaliação.

### 3.3.6 Avaliação do sistema

A avaliação do sistema será realizada a partir de cenários simulados de partilha, construídos para representar combinações plausíveis de composição familiar, bens, dívidas, regime patrimonial e disposições sucessórias dentro do escopo adotado no trabalho.

Em cada cenário, o resultado produzido pelo Partilha Certa será comparado com um cálculo realizado por meio tradicional, entendido neste trabalho como conferência manual estruturada e/ou planilha de apoio.

## 3.4 Estratégia de avaliação e critérios de análise

A estratégia principal de avaliação do Partilha Certa baseia-se na análise de cenários simulados. Essa escolha permite observar o comportamento do sistema em condições controladas, com entradas conhecidas e resultados passíveis de conferência (Peffers et al. 2007; Hevner et al. 2004).

Para cada cenário, deverão ser explicitados os dados de entrada, as premissas adotadas, o resultado esperado e o resultado efetivamente produzido pelo sistema. Também poderão ser observadas etapas intermediárias do cálculo, de modo a verificar a coerência do processamento realizado pelo sistema.

A análise dos cenários considera três critérios principais. O primeiro é a consistência jurídica, observada pela aderência do fluxo de cálculo às regras sucessórias selecionadas para o escopo do sistema. O segundo é a precisão, observada pela coincidência entre os valores produzidos pelo Partilha Certa e os valores obtidos por conferência tradicional. O terceiro é a eficiência operacional, observada pela redução de esforço e tempo na resolução dos cenários analisados, ainda que essa medida tenha caráter indicativo e não experimental em sentido estrito (Hevner et al. 2004).

De forma complementar, também poderão ser considerados os testes implementados no desenvolvimento do sistema, como evidência de verificação técnica de partes específicas da aplicação.

## 3.5 Síntese do percurso metodológico

Em síntese, a metodologia deste trabalho combina revisão bibliográfica e documental, tradução das regras sucessórias para critérios computacionais, desenvolvimento do sistema e avaliação por cenários simulados, tendo o DSRP como referência para a organização dessas etapas.

Essa estrutura permitiu organizar, de forma coerente, o percurso entre o levantamento do domínio, a implementação do sistema e sua avaliação.
