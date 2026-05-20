# Painel do TCC

## Identificação

- **Projeto:** Partilha Certa
- **Título provisório:** Automação da partilha de bens no direito sucessório brasileiro: proposta e implementação de uma ferramenta de apoio jurídico
- **Tema:** Automação da partilha de bens no direito sucessório brasileiro
- **Curso:** Tecnologia em Sistemas para Internet
- **Instituição:** IFRS - Campus Porto Alegre
- **Autor:** A definir
- **Orientador:** Rodrigo Prestes Machado
- **TCC1 ou TCC2:** TCC1

## Objeto de estudo

O objeto de estudo é a aplicação web Partilha Certa, uma Lawtech voltada à modelagem e automação de cálculos de partilha de bens no direito sucessório brasileiro.

A aplicação funciona como um motor de cálculo sucessório, permitindo cadastrar bens, herdeiros e dívidas, separar bens comuns e particulares, calcular meação, monte hereditário, legítima, parte disponível, quotas hereditárias e simular a divisão real dos bens com eventual cálculo de torna.

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

## Metodologia prevista

A pesquisa deve combinar revisão bibliográfica e documental sobre direito sucessório brasileiro, modelagem computacional do domínio, desenvolvimento de uma aplicação web e validação por cenários simulados.

A validação deverá comparar os resultados produzidos pelo sistema com cálculos realizados por métodos tradicionais, observando consistência jurídica, precisão dos valores calculados e tempo de execução.


## Estrutura prevista do referencial teórico

A estrutura detalhada do referencial teórico está registrada em:

`01-planejamento/estrutura-referencial-teorico.md`

Subseções previstas:

1. Fundamentos do Direito Sucessório Brasileiro.
2. Estrutura da Partilha de Bens.
3. Complexidade e Desafios do Cálculo Sucessório.
4. Legaltech e Automação no Direito.
5. Modelagem de Domínio e Regras de Negócio.

## Documentação do sistema

| Arquivo | Função | Status |
| --- | --- | --- |
| `06-sistema/fontes-do-sistema.md` | Índice das fontes técnicas externas do Partilha Certa. | Criado |
| `06-sistema/requisitos/escopo-juridico.md` | Escopo jurídico detalhado, validado contra o comportamento real do sistema. | Criado |
| `06-sistema/requisitos/quadro-escopo-sistema.md` | Quadro resumido do escopo para uso na metodologia ou seção do sistema no artigo. | Criado |

## Estado da escrita

| Parte | Status | Observações |
| --- | --- | --- |
| Introdução | Rascunho inicial | Primeira versão salva em `04-rascunhos/introducao.md`; requer fontes e revisão. |
| Referencial teórico | Finalizado em rascunho | Seção 2 consolidada em `04-rascunhos/secao-2-referencial-teorico.md`, com os subtópicos 2.1 a 2.5 estruturados, revisados e limpos para uso na versão do artigo. |
| Metodologia | Rascunho inicial | Primeira versão salva em `04-rascunhos/secao-3-metodologia.md`, com separação entre abordagem, procedimentos, etapas de desenvolvimento e estratégia de validação. |
| Resultados e discussão | Não iniciado | Depende dos cenários de validação. |
| Considerações Parciais | Não iniciado | Deve fechar o TCC1 indicando limites atuais e continuidade prevista para o TCC2. |
| Referências | Não iniciado | Precisa iniciar levantamento de conteúdo. |

## Decisões de estrutura

- O artigo terá `Abstract` e `Keywords`, mas esses itens serão redigidos ao final.
- O cronograma ficará fora do artigo até segunda ordem.
- A seção final do TCC1 será `Considerações Parciais`.
