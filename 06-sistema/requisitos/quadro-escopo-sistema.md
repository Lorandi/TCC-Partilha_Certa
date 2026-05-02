# Quadro Resumido do Escopo do Sistema

Este arquivo sintetiza o escopo jurídico e funcional do Partilha Certa em formato adequado para adaptação ao artigo de TCC1. A versão detalhada está em `06-sistema/requisitos/escopo-juridico.md`, e a fonte da verdade técnica do sistema é `C:\projetos\Herança+\heranca-app\CLAUDE.md`.

## Quadro para uso no artigo

| Dimensão | Tratamento no Partilha Certa | Situação no escopo |
| --- | --- | --- |
| Ordem de vocação hereditária | Identifica a classe sucessória aplicável ao caso, considerando descendentes, ascendentes, cônjuge ou companheiro e colaterais. | Implementado |
| Cônjuge ou companheiro sobrevivente | Calcula a participação conforme regime de bens, concorrência sucessória e classificação informada pelo usuário. | Implementado |
| Descendentes | Calcula quotas por cabeça e, quando aplicável, por representação. | Implementado |
| Ascendentes | Calcula cenários sem descendentes, inclusive concorrência com cônjuge ou companheiro. | Implementado |
| Colaterais | Calcula sucessão colateral quando não há descendentes, ascendentes, cônjuge ou companheiro com direito sucessório. | Implementado |
| Herdeiros necessários | Identifica a existência de herdeiros necessários para fins de proteção da legítima. | Implementado |
| Legítima e parte disponível | Calcula a legítima e a parte disponível; na sucessão colateral, considera legítima igual a zero e parte disponível igual à herança. | Implementado |
| Testamento | Considera disposições testamentárias informadas pelo usuário, limitadas à parte disponível. | Implementado com escopo delimitado |
| Representação sucessória | Trata cadeias de representação em casos de herdeiro pré-morto, como filho para neto e irmão para sobrinho. | Implementado |
| Regime de bens e meação | Calcula a meação conforme o regime de bens e separa essa parcela da herança. | Implementado |
| Dívidas do espólio | Abate as dívidas do patrimônio inventariável antes da herança líquida, sem reduzir a meação. | Implementado |
| Colação | Considera colações informadas pelo usuário, aplicadas a herdeiros necessários na legítima. | Implementado |
| União estável | Considera companheiro sobrevivente quando o usuário informa união estável no caso concreto, sem validar judicialmente sua existência. | Condicionado à entrada do usuário |
| ITCMD | Calcula o imposto conforme regras estaduais cadastradas no sistema. | Funcionalidade complementar |
| Divisão prática dos bens | Apoia a distribuição concreta dos bens, com sugestão automática e cálculo de tornas. | Funcionalidade complementar |

## Limitações declaradas

O sistema não valida requisitos formais do testamento, existência jurídica de união estável, comunicabilidade de dívidas, nem controvérsias jurídicas externas aos dados informados pelo usuário. Também ficam fora do escopo inicial temas como aceitação e renúncia da herança, herança jacente e vacante, petição de herança, indignidade, deserdação, substituições testamentárias, fideicomisso, direito de acrescer e discussões processuais de inventário.

## Texto de apoio para o artigo

O Partilha Certa delimita seu escopo à modelagem computacional de regras sucessórias necessárias ao cálculo e à simulação da partilha de bens. O sistema considera os dados fornecidos pelo usuário sobre bens, dívidas, regime de bens, herdeiros, testamento, colações e vínculos sucessórios, aplicando regras de vocação hereditária, meação, legítima, parte disponível, representação, colação e abatimento de dívidas. Determinados temas jurídicos permanecem fora do escopo inicial, especialmente aqueles que exigem validação formal, decisão judicial ou interpretação jurídica externa aos dados informados.

## Notas de uso

- Usar o quadro na seção de metodologia, proposta do sistema ou desenvolvimento.
- Antes de inserir no artigo final, revisar a terminologia com doutrina jurídica e orientação.
- Não tratar `CLAUDE.md` como referência acadêmica; usá-lo apenas como documentação técnica do objeto de estudo.
