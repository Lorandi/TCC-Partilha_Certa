# Código Civil Brasileiro

## Identificação

- **Fonte:** BRASIL. Lei nº 10.406, de 10 de janeiro de 2002. Código Civil.
- **Tipo:** Legislação.
- **Página oficial:** https://www.planalto.gov.br/Ccivil_03/leis/2002/L10406compilada.htm
- **Status:** registrada como fonte normativa principal.

## Uso no TCC

Esta fonte deve sustentar a delimitação jurídica do trabalho, especialmente os conceitos e regras de direito sucessório usados para modelar o sistema Partilha Certa.

O mapeamento de uso no sistema deve ser conferido contra `C:\projetos\Herança+\heranca-app\CLAUDE.md`, que é a fonte da verdade técnica do comportamento atual do Partilha Certa.

## Pontos a consultar

- Abertura da sucessão.
- Herdeiros necessários.
- Legítima e parte disponível.
- Ordem de vocação hereditária.
- Representação sucessória.
- Regras relacionadas à partilha e às dívidas do espólio.

## Matriz inicial de artigos sucessórios

| Tema | Artigos iniciais | Regra jurídica resumida | Uso no Partilha Certa | Entra no TCC1? | Observações |
| --- | --- | --- | --- | --- | --- |
| Abertura da sucessão | Arts. 1.784 a 1.787 | A herança transmite-se com a abertura da sucessão; a sucessão e a legitimação para suceder observam a lei vigente no momento da abertura. | Base conceitual para definir o momento jurídico de início da partilha e a existência do espólio. | Sim | Conferir se o sistema precisa registrar data de falecimento para efeitos legais ou apenas para documentação do caso. |
| Aceitação e renúncia da herança | Arts. 1.804 a 1.813 | A herança pode ser aceita ou renunciada, com efeitos sobre quem participa da sucessão. | Não será implementado no Partilha Certa. | Não | Registrar como fora do escopo do TCC e do sistema. |
| Excluídos da sucessão | Arts. 1.814 a 1.818 | Determinadas condutas podem excluir herdeiros ou legatários da sucessão. | Pode afetar elegibilidade de herdeiros. | Não, salvo escopo explícito | Provável limitação do sistema no TCC1; depende de decisão jurídica e processual. |
| Herança jacente e vacante | Arts. 1.819 a 1.823 | Regula situações em que não há herdeiro certo ou aceitação da herança. | Não parece central para o motor inicial de cálculo. | Não | Registrar como fora do escopo, salvo se houver necessidade futura. |
| Petição de herança | Arts. 1.824 a 1.828 | Trata da pretensão de reconhecimento do direito sucessório. | Não é regra de cálculo patrimonial direto. | Não | Tema processual/material mais adequado para limitações. |
| Ordem de vocação hereditária | Art. 1.829 | Define a ordem de chamamento dos herdeiros: descendentes, ascendentes, cônjuge sobrevivente e colaterais, conforme condições legais. | Regra central para identificar quem participa da partilha. | Sim | Um dos principais artigos para modelagem de regras de negócio. |
| Direito sucessório do cônjuge ou companheiro | Arts. 1.829, 1.830, 1.831, 1.832, 1.837 e 1.838; arts. 1.723 a 1.727 para união estável | Define condições de participação do cônjuge ou companheiro, direito real de habitação e concorrência com descendentes ou ascendentes. | Base para cálculo da quota do cônjuge ou companheiro e separação entre meação e herança, conforme classificação informada pelo usuário. | Sim | O sistema não validará a existência jurídica da união estável; considerará a informação fornecida pelo usuário no caso concreto. |
| Sucessão dos descendentes | Arts. 1.833 a 1.835 | Descendentes da mesma classe têm mesmos direitos, observadas regras de representação. | Base para dividir quotas entre filhos, netos e demais descendentes. | Sim | Necessário modelar divisão por cabeça e por estirpe quando houver representação. |
| Sucessão dos ascendentes | Art. 1.836 | Na falta de descendentes, são chamados ascendentes em concorrência com cônjuge, conforme grau e linhas. | Base para cenários sem descendentes. | Sim | Pode ser tratado em cenários específicos de validação. |
| Sucessão do cônjuge isolado e colaterais | Arts. 1.838 a 1.844 | Na ausência de descendentes e ascendentes, regula participação do cônjuge e, em sua falta, dos colaterais. | Define regras para cenários sem descendentes e ascendentes, incluindo sucessão de colaterais já calculada pelo Partilha Certa. | Sim | Tratar como regra central do escopo inicial. |
| Herdeiros necessários | Art. 1.845 | Define descendentes, ascendentes e cônjuge como herdeiros necessários. | Base para identificar proteção da legítima. | Sim | Fundamental para explicar limites da disposição patrimonial. |
| Legítima e parte disponível | Arts. 1.846 a 1.850 | Metade dos bens da herança pertence aos herdeiros necessários; há regras para cálculo da legítima e restrições à parte disponível. | Base para cálculo de legítima, parte disponível e disposições testamentárias dentro dos limites legais. | Sim | Conceito central para compatibilizar herdeiros necessários e testamento. |
| Representação sucessória | Arts. 1.851 a 1.856 | Permite que descendentes de herdeiro pré-morto sucedam no lugar dele em hipóteses previstas. | Base para divisão por estirpe em caso de herdeiro pré-morto. | Sim | Importante para validar cenários com netos representando filho falecido. |
| Sucessão testamentária | Arts. 1.857 a 1.990 | Regula testamento, capacidade testamentária, legados, direito de acrescer, substituições e deserdação. | Base para tratar disposições testamentárias informadas pelo usuário, respeitando legítima e parte disponível. | Sim | No Partilha Certa, `testamentoEfetivo = min(totalTestamento, parteDisponivel)`; testamento só pode apontar para herdeiro vivo, e vínculo com herdeiro pré-morto é ignorado ou removido. |
| Inventário e partilha | Arts. 1.991 a 2.027 | Trata da administração da herança, pagamento de dívidas, colação, sonegação e partilha. | Base para explicar partilha, dívidas do espólio, colação e formação do monte partilhável. | Sim | No Partilha Certa, dívidas reduzem o Patrimônio Inventariável antes da herança líquida e não reduzem a meação; colação entra para herdeiros necessários na legítima. |
| Regime de bens e meação | Arts. 1.639 a 1.688 | Define regimes patrimoniais do casamento e seus efeitos sobre bens comuns e particulares. | Base para separar meação e herança antes do cálculo sucessório. | Sim | Não está no Livro de Sucessões, mas é essencial para o cálculo de partilha. |
| União estável | Arts. 1.723 a 1.727 | Define união estável e seus efeitos gerais no direito de família. | Permite tratar companheiro sobrevivente quando o usuário informar união estável no caso concreto. | Sim | O Partilha Certa não validará a configuração jurídica da união estável; essa definição será entrada do usuário. |

## Priorização para o TCC1

### Núcleo central

- Abertura da sucessão.
- Ordem de vocação hereditária.
- Cônjuge sobrevivente.
- Descendentes e ascendentes.
- Colaterais.
- Herdeiros necessários.
- Legítima e parte disponível.
- Representação sucessória.
- Regime de bens e meação.
- Dívidas do espólio como abatimento do monte hereditário.
- Colação informada pelo usuário.
- ITCMD, divisão prática dos bens e torna como funcionalidades complementares do sistema.

### Escopo secundário

- Legados de bem específico.

### Fora do escopo inicial

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

### Não entra no escopo

- Redução de disposição testamentária.
- Múltiplos beneficiários testamentários.
- Capacidade testamentária.
- Validade formal do testamento.
- Caducidade.
- Revogação.
- Rompimento de testamento.
- Substituição testamentária.
- Fideicomisso.
- Direito de acrescer.
- Deserdação.

## Observações

- Usar como base normativa, não como única explicação doutrinária.
- Complementar com doutrina de Direito Civil/Sucessões para interpretação dos conceitos.
- Conferir os artigos específicos antes de citar no texto final.
- Conferir cada artigo diretamente na página oficial antes de transformar a matriz em citação final.
- Validar com o orientador se a delimitação de testamento é suficiente para o TCC1.
- Conferir comportamento técnico no `CLAUDE.md` antes de afirmar que determinada regra está implementada no Partilha Certa.
