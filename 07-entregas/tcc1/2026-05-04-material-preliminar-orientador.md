# Material preliminar para orientação - TCC1

**Título provisório:** Automação da partilha de bens no direito sucessório brasileiro: proposta e implementação de uma ferramenta de apoio jurídico

**Projeto:** Partilha Certa

**Curso:** Tecnologia em Sistemas para Internet

**Instituição:** IFRS - Campus Porto Alegre

**Orientador:** Rodrigo Prestes Machado

**Etapa:** TCC1

## Observação inicial

Este documento reúne o material preliminar já organizado para discussão com o orientador. O conteúdo ainda não corresponde à versão final do artigo, mas apresenta o recorte do trabalho, o problema de pesquisa, os objetivos, a justificativa, um rascunho inicial de introdução, a estrutura prevista do referencial teórico, a metodologia prevista e a delimitação inicial do sistema Partilha Certa.

## Tema e recorte

O tema do trabalho é a automação da partilha de bens no direito sucessório brasileiro.

O recorte proposto consiste na modelagem e implementação de regras sucessórias brasileiras em uma aplicação web voltada ao cálculo e à simulação de partilha de bens, com atenção à consistência jurídica, à precisão dos cálculos e à rastreabilidade dos resultados.

## Objeto de estudo

O objeto de estudo é a aplicação web Partilha Certa, uma ferramenta voltada à modelagem e automação de cálculos de partilha de bens no direito sucessório brasileiro.

A aplicação funciona como um motor de cálculo sucessório, permitindo cadastrar bens, herdeiros e dívidas, separar bens comuns e particulares, calcular meação, monte hereditário, legítima, parte disponível, quotas hereditárias e simular a divisão real dos bens, incluindo eventual cálculo de torna.

## Problema de pesquisa

Como modelar e implementar regras do direito sucessório brasileiro em um sistema computacional de forma a favorecer a consistência jurídica e a precisão nos cálculos de partilha de bens?

## Hipótese

A modelagem e implementação computacional das regras do direito sucessório brasileiro possibilitam a realização de cálculos de partilha de bens com maior consistência, menor ocorrência de erros e menor tempo de execução em comparação aos métodos tradicionais.

## Objetivo geral

Desenvolver e validar um sistema computacional capaz de modelar e implementar as regras do direito sucessório brasileiro, com o objetivo de realizar cálculos de partilha de bens de forma consistente, precisa e eficiente.

## Objetivos específicos

1. Analisar os conceitos e regras do direito sucessório brasileiro relevantes para o cálculo de partilha de bens.
2. Identificar e formalizar as principais regras jurídicas envolvidas no processo de partilha, como meação, legítima, ordem de vocação hereditária e representação.
3. Modelar o domínio sucessório em termos computacionais, definindo entidades, atributos e regras de negócio.
4. Desenvolver um sistema computacional capaz de aplicar automaticamente as regras de partilha de bens.
5. Implementar funcionalidades para cadastro de bens, herdeiros e dívidas, bem como para simulação da divisão patrimonial.
6. Validar os resultados do sistema por meio de cenários simulados, comparando-os com cálculos realizados por métodos tradicionais.
7. Analisar a consistência, precisão e eficiência dos resultados obtidos pelo sistema.

## Justificativa

A partilha de bens no direito sucessório brasileiro envolve regras jurídicas complexas e cálculos patrimoniais suscetíveis a erro quando realizados manualmente ou por métodos pouco padronizados. A correta distinção entre bens comuns e particulares, a apuração da meação, a identificação do monte hereditário, a aplicação da legítima, a ordem de vocação hereditária e a representação por estirpe exigem interpretação jurídica e precisão matemática.

Nesse contexto, a automação pode apoiar profissionais do meio jurídico ao reduzir inconsistências, aumentar a eficiência e tornar os cálculos mais claros, rastreáveis e verificáveis. O estudo também é relevante para a área de Sistemas para Internet por demonstrar como regras de um domínio jurídico especializado podem ser modeladas em software, separando regra de negócio, interface e mecanismos de validação.

O projeto Partilha Certa permite aplicar conhecimentos de desenvolvimento web, modelagem de regras de negócio, testes e validação em um problema real do domínio jurídico, com potencial de uso prático e evolução futura como solução Lawtech.

## Rascunho inicial da introdução

A partilha de bens no direito sucessório brasileiro envolve a aplicação de regras jurídicas e cálculos patrimoniais que exigem precisão, organização e rastreabilidade. Elementos como a identificação dos herdeiros, a distinção entre bens comuns e particulares, a apuração da meação, a definição do monte hereditário, a legítima, a parte disponível, as dívidas do espólio e a ordem de vocação hereditária decorrem de regras previstas no Código Civil brasileiro e influenciam diretamente o resultado da divisão patrimonial (BRASIL, 2002). Quando esse processo é conduzido manualmente ou com apoio de instrumentos pouco padronizados, há maior risco de inconsistências, retrabalho e dificuldade de conferência dos valores obtidos.

No contexto da Tecnologia da Informação, esse problema permite investigar como regras de um domínio jurídico especializado podem ser representadas em estruturas computacionais. A construção de uma aplicação web para apoio ao cálculo de partilha de bens exige transformar conceitos jurídicos em entidades, atributos, relações e regras de negócio, preservando o escopo jurídico definido e tornando explícitos os limites da automação. Dessa forma, o sistema não substitui a interpretação profissional do Direito, mas pode apoiar a organização dos dados, a execução dos cálculos e a conferência dos resultados.

Este trabalho tem como objeto de estudo o Partilha Certa, uma aplicação web voltada à modelagem e automação de cálculos de partilha de bens no direito sucessório brasileiro. A proposta parte da seguinte questão de pesquisa: como modelar e implementar regras do direito sucessório brasileiro em um sistema computacional de forma a favorecer a consistência jurídica e a precisão nos cálculos de partilha de bens?

O objetivo geral é desenvolver e validar um sistema computacional capaz de modelar e implementar regras do direito sucessório brasileiro, com o objetivo de realizar cálculos de partilha de bens de forma consistente, precisa e eficiente. Para isso, o trabalho busca analisar conceitos jurídicos relevantes, identificar e formalizar regras aplicáveis à partilha, modelar o domínio sucessório em termos computacionais, desenvolver funcionalidades de cadastro e simulação, e planejar a validação dos resultados por meio de cenários simulados.

Como TCC1, este artigo concentra-se na delimitação do problema, na fundamentação teórica, na definição do escopo do sistema e na metodologia prevista para desenvolvimento e validação. A validação completa dos cenários e a análise dos resultados deverão ser aprofundadas em etapa posterior, no TCC2, a partir da comparação entre os resultados produzidos pelo sistema e cálculos realizados por métodos tradicionais.

Metodologicamente, a pesquisa prevê revisão bibliográfica e documental sobre direito sucessório, tecnologia aplicada ao Direito, modelagem de domínio e validação de software. Também prevê a análise do sistema Partilha Certa, a documentação das regras de negócio implementadas ou planejadas e a definição de cenários simulados que permitam verificar a consistência jurídica, a precisão dos cálculos e a eficiência do processo.

O artigo está organizado da seguinte forma: a seção 2 apresenta o referencial teórico, abordando fundamentos do direito sucessório brasileiro, estrutura da partilha de bens, desafios do cálculo sucessório, Legaltech e modelagem de domínio. A seção 3 descreve a metodologia prevista para o desenvolvimento e validação do sistema. A seção 4 apresenta o escopo e a proposta do sistema Partilha Certa. Por fim, a seção 5 reúne as considerações parciais, limitações e próximos passos para continuidade no TCC2.

## Estrutura prevista do referencial teórico

### Fundamentos do Direito Sucessório Brasileiro

Esta subseção deve apresentar os conceitos jurídicos mínimos necessários para compreender o problema da partilha de bens e o escopo jurídico do sistema Partilha Certa. Devem ser abordados conceito de sucessão, abertura da sucessão, herdeiros necessários, herdeiros facultativos e Código Civil Brasileiro como base legal.

### Estrutura da Partilha de Bens

Esta subseção deve explicar os elementos jurídicos que influenciam diretamente o cálculo sucessório e que precisam ser formalizados para implementação computacional. Devem ser abordados meação, monte hereditário, legítima, parte disponível, ordem de vocação hereditária, concorrência do cônjuge, representação por estirpe e dívidas do espólio.

### Complexidade e Desafios do Cálculo Sucessório

Esta subseção deve demonstrar o problema prático que justifica a automação, destacando por que a partilha de bens exige precisão, rastreabilidade e padronização. Devem ser considerados risco de erro, dificuldade dos cálculos manuais, falta de padronização e diferença entre interpretação jurídica e cálculo matemático.

### Legaltech e Automação no Direito

Esta subseção deve posicionar o Partilha Certa dentro do contexto de tecnologia aplicada ao Direito, sem afirmar que o sistema substitui a atuação profissional jurídica. O sistema pode ser classificado como uma ferramenta de apoio jurídico voltada à automação de cálculos sucessórios.

### Modelagem de Domínio e Regras de Negócio

Esta subseção deve criar o elo conceitual entre o domínio jurídico e a implementação computacional, mostrando como regras jurídicas podem ser representadas como entidades, atributos, relações e regras de negócio.

## Metodologia prevista

A pesquisa deve combinar revisão bibliográfica e documental, modelagem computacional do domínio, desenvolvimento de uma aplicação web e validação por cenários simulados.

A revisão bibliográfica e documental deve abordar direito sucessório brasileiro, tecnologia aplicada ao Direito, modelagem de domínio, regras de negócio e validação de software. A modelagem computacional deve transformar as regras sucessórias delimitadas em entidades, atributos, relações e regras implementáveis. O desenvolvimento do sistema deve materializar essa modelagem em uma aplicação web capaz de cadastrar informações sucessórias e calcular a partilha de bens.

A validação deverá comparar os resultados produzidos pelo sistema com cálculos realizados por métodos tradicionais, observando consistência jurídica, precisão dos valores calculados, tempo de execução, explicabilidade dos resultados e cobertura dos cenários analisados.

## Escopo inicial do sistema Partilha Certa

O Partilha Certa delimita seu escopo à modelagem computacional de regras sucessórias necessárias ao cálculo e à simulação da partilha de bens. O sistema considera os dados fornecidos pelo usuário sobre bens, dívidas, regime de bens, herdeiros, testamento, colações e vínculos sucessórios, aplicando regras de vocação hereditária, meação, legítima, parte disponível, representação, colação e abatimento de dívidas.

Entre os pontos tratados no escopo atual estão ordem de vocação hereditária, cônjuge ou companheiro sobrevivente, descendentes, ascendentes, colaterais, herdeiros necessários, legítima, parte disponível, testamento com escopo delimitado, representação sucessória, regime de bens, meação, dívidas do espólio, colação, união estável condicionada à informação do usuário, ITCMD como funcionalidade complementar e divisão prática dos bens com cálculo de tornas.

O sistema não valida requisitos formais do testamento, existência jurídica de união estável, comunicabilidade de dívidas, nem controvérsias jurídicas externas aos dados informados pelo usuário. Também ficam fora do escopo inicial temas como aceitação e renúncia da herança, herança jacente e vacante, petição de herança, indignidade, deserdação, substituições testamentárias, fideicomisso, direito de acrescer e discussões processuais de inventário.

## Referências iniciais levantadas

BRASIL. Lei nº 10.406, de 10 de janeiro de 2002. Código Civil. Disponível em: https://www.planalto.gov.br/Ccivil_03/leis/2002/L10406compilada.htm.

SANTANA, Davi; JORDAN, Diana Carina Macedo; NOGUEIRA, Joaquim Lucas Cruz; RAMALHO, Maria Antônia Sena dos Santos; RAMALHO, Maria Clara Sena dos Santos; LIMA, Maria Eduarda Torres Moraes Dias. Legaltechs e Lawtechs: considerações no direito brasileiro. Res Severa Verum Gaudium, Porto Alegre, v. 7, n. 1, 2022. Disponível em: https://seer.ufrgs.br/resseveraverumgaudium/article/view/124640.

GOMES, Letícia Beatriz Arruda; FERREIRA, Kilvia Souza; ANDRADE, Fabiano Souza. Modernização do Direito: a criação de Startups Jurídicas. Revista Direito em Debate, v. 31, n. 57, e12073, 2022. DOI: 10.21527/2176-6622.2022.57.12073. Disponível em: https://www.revistas.unijui.edu.br/index.php/revistadireitoemdebate/article/view/12073.

RODRIGUES, Rildenesbraz. A importância das startups jurídicas: a contribuição das Lawtechs e Legaltechs para a inovação do sistema judiciário brasileiro. Repositório Institucional do Unifip, v. 7, n. 1, 2024. Disponível em: https://editora.unifip.edu.br/repositoriounifip/article/view/4680.

SILVA, Tobias Oliveira e. O imposto de herança e o problema da sucessão no Brasil. Repositório Institucional da UCS, 2025. Disponível em: https://repositorio.ucs.br/items/3fc931d6-a76e-46bf-b331-370175058204.

## Pontos para validação com o orientador

1. Confirmar se o problema de pesquisa está adequado ao escopo de TCC1.
2. Confirmar se o título provisório está claro ou se deve ser reduzido.
3. Validar se o referencial teórico deve manter a divisão proposta.
4. Confirmar se a seção sobre o sistema deve aparecer como seção própria ou dentro da metodologia.
5. Confirmar se o TCC1 deve incluir cronograma no artigo.
6. Indicar fontes jurídicas ou técnicas prioritárias para fortalecer o referencial teórico.

## Pendências de escrita

1. Complementar o Código Civil com doutrina de direito sucessório e partilha de bens.
2. Inserir fontes acadêmicas sobre Legaltech, automação jurídica e limites da automação.
3. Inserir fontes sobre modelagem de domínio, regras de negócio e validação de software.
4. Escrever a seção de metodologia em versão final.
5. Preparar o artigo oficial em LaTeX após validação do recorte pelo orientador.
