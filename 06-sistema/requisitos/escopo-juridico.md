# Escopo Jurídico Inicial

Este arquivo traduz a matriz normativa do Código Civil em decisões preliminares de escopo para o sistema Partilha Certa. A fonte da verdade técnica para o comportamento atual do sistema é `C:\projetos\Herança+\heranca-app\CLAUDE.md`.

## Escopo central do TCC1

| Tema | Situação no sistema | Aderência ao sistema real | Uso previsto |
| --- | --- | --- | --- |
| Abertura da sucessão | Conceitual/documental | Conceitual | Explicar o momento de referência da sucessão e do cálculo. |
| Ordem de vocação hereditária | Regra central | Implementado em `CalculoService` e arquivos de vocação hereditária | Identificar classes de herdeiros chamadas à sucessão. |
| Cônjuge ou companheiro sobrevivente | Regra central | Implementado conforme classificação informada pelo usuário | Calcular participação conforme concorrência, regime de bens e classificação informada pelo usuário no caso concreto. |
| Descendentes | Regra central | Implementado | Calcular quotas por cabeça e, quando aplicável, por representação. |
| Ascendentes | Regra central | Implementado, inclusive concorrência com cônjuge | Calcular cenários sem descendentes, com ou sem cônjuge. |
| Colaterais | Regra central | Implementado | Calcular sucessão de colaterais quando não houver descendentes, ascendentes, cônjuge ou companheiro com direito sucessório. |
| Herdeiros necessários | Regra central | Implementado no cálculo de legítima | Fundamentar a existência da legítima. |
| Legítima e parte disponível | Regra central | Implementado; na sucessão colateral, legítima = 0 e parte disponível = herança | Calcular limites patrimoniais protegidos por lei. |
| Testamento | Regra central delimitada | Implementado; `testamentoEfetivo = min(totalTestamento, parteDisponivel)` | Considerar disposições testamentárias informadas pelo usuário, limitadas à parte disponível. |
| Representação sucessória | Regra central | Implementado para cadeias `Filho(a) -> Neto(a) -> Outro` e `Irmão/Irmã -> Sobrinho -> Outro` | Tratar herdeiro pré-morto e divisão por estirpe. |
| Regime de bens e meação | Regra central | Implementado para comunhão parcial, comunhão universal, separação convencional e separação obrigatória | Separar bens comuns e particulares antes da herança. |
| Dívidas do espólio | Regra central | Implementado; dívidas reduzem o Patrimônio Inventariável antes da herança líquida e não reduzem a meação | Abater as dívidas do monte hereditário, preservando a meação; considerar que as dívidas informadas são exclusivas do falecido. |
| Colação | Regra central condicionada à entrada do usuário | Implementado; colação entra para herdeiros necessários na legítima e pode descer pela cadeia de representantes finais ativos | Considerar colações quando o usuário informar doações ou valores sujeitos à colação no caso concreto. |
| ITCMD | Regra complementar do sistema | Implementado em `domain/itcmd` | Usar como funcionalidade técnica do Partilha Certa, não como eixo jurídico principal do TCC1. |
| Divisão prática dos bens e torna | Funcionalidade central do sistema | Implementado em `DistribuicaoService` e aba `Divisao` | Descrever como etapa prática posterior ao cálculo das quotas. |

## Escopo secundário

| Tema | Situação no sistema | Aderência ao sistema real | Uso previsto |
| --- | --- | --- | --- |
| União estável | Regra condicionada à entrada do usuário | Tratada pela classificação informada pelo usuário | Considerar companheiro quando o usuário informar união estável no caso concreto, sem validar judicialmente a existência da união. |
| Legado de bem específico | Regra secundária | A UI possui testamento na aba `Bens`; o `CLAUDE.md` registra que testamento aponta para herdeiro vivo e saneia vínculos inválidos | Permitir indicar disposição testamentária sem resolver regras testamentárias especiais. |

## Fora do escopo inicial

- Herança jacente e vacante.
- Aceitação e renúncia da herança.
- Petição de herança.
- Exclusão da sucessão por indignidade.
- Deserdação.
- Redução de disposição testamentária.
- Múltiplos beneficiários testamentários.
- Capacidade testamentária.
- Validade formal do testamento.
- Caducidade, revogação e rompimento de testamento.
- Substituição testamentária.
- Fideicomisso.
- Direito de acrescer.
- Discussões processuais de inventário.
- Reembolso, pois o conceito está temporariamente desativado no sistema e é ignorado por regras de negócio e UI.

## Decisão de escopo sobre testamento

O sistema considerará disposições testamentárias informadas pelo usuário em valor ou percentual, limitadas à parte disponível, sem validar requisitos formais do testamento nem tratar regras testamentárias especiais.

### Entra no escopo

- Existência de testamento.
- Percentual ou valor destinado por testamento.
- Beneficiário testamentário.
- Legado de bem específico.
- Testamento com valor fixo.
- Beneficiário testamentário que também é herdeiro.
- Inexistência ou insuficiência da parte disponível.
- Caducidade operacional de testamento vinculado a herdeiro pré-morto, porque o sistema ignora ou remove esse vínculo inválido.

### Não entra no escopo

- Redução de disposição testamentária como procedimento jurídico autônomo.
- Múltiplos beneficiários testamentários como regra testamentária especial.
- Capacidade testamentária.
- Validade formal do testamento.
- Caducidade, revogação e rompimento de testamento como institutos jurídicos gerais.
- Substituição testamentária.
- Fideicomisso.
- Direito de acrescer.
- Deserdação.

## Decisão de escopo sobre dívidas

As dívidas informadas no sistema serão consideradas dívidas exclusivas do falecido. Elas serão abatidas do Patrimônio Inventariável antes da herança líquida, preservando a meação quando houver bens comuns. Se as dívidas excederem a herança, a herança vai a zero. O sistema não tratará, no escopo inicial, discussão sobre comunicabilidade da dívida, responsabilidade patrimonial de terceiros ou classificação detalhada da origem da obrigação.

## Decisão de escopo sobre colação

O sistema considerará colações quando o usuário informar doações ou valores sujeitos à colação no caso concreto. O Partilha Certa não validará, no escopo inicial, se determinado ato jurídico deveria ou não ser colacionado; essa classificação será responsabilidade da entrada informada pelo usuário.

## Pontos de atenção para escrita

- Diferenciar regras jurídicas implementadas de funcionalidades auxiliares, como ITCMD, divisão prática dos bens, torna e geração de PDF.
- Declarar que o sistema usa entradas fornecidas pelo usuário para união estável, colação, testamento, bens, dívidas e classificação patrimonial.
- Não afirmar que o sistema valida requisitos formais ou controvérsias jurídicas externas aos dados informados.
- Usar o `CLAUDE.md` para confirmar comportamento técnico antes de escrever sobre o Partilha Certa.
