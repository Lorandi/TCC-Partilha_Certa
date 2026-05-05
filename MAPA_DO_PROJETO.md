# Mapa do Projeto TCC

Este arquivo é a memória operacional do TCC. Ele deve ser atualizado sempre que houver mudança relevante de tema, escopo, estrutura, orientação, referências, entregas ou decisões de escrita.

## Estado atual

- **Formato provável:** artigo de TCC.
- **Projeto:** Partilha Certa.
- **Título provisório:** Automação da partilha de bens no direito sucessório brasileiro: proposta e implementação de uma ferramenta de apoio jurídico.
- **Curso:** Tecnologia em Sistemas para Internet.
- **Instituição:** IFRS - Campus Porto Alegre.
- **Orientador:** Rodrigo Prestes Machado.
- **Tema:** Automação da partilha de bens no direito sucessório brasileiro.
- **Recorte:** Modelagem e implementação de regras sucessórias brasileiras em uma aplicação web para cálculo e simulação de partilha de bens.
- **Problema de pesquisa:** Como modelar e implementar regras do direito sucessório brasileiro em um sistema computacional de forma a favorecer a consistência jurídica e a precisão nos cálculos de partilha de bens?
- **TCC:** TCC1.
- **Documento oficial de escrita:** `05-artigo-latex/main.tex`, quando o template for preparado.
- **Memória de formato:** `09-referencias-formato/outros-tccs/resumo-formato.md`.

## Estrutura de pastas

| Pasta | Função |
| --- | --- |
| `00-orientacoes/` | Normas, feedbacks, atas de reunião e materiais enviados por orientador/professor. |
| `01-planejamento/` | Tema, problema, objetivos, justificativa, cronograma e decisões centrais. |
| `02-referencias-conteudo/` | Fontes que fundamentam o conteúdo do TCC. Ainda deve ser preenchida conforme o tema. |
| `03-fichamentos/` | Fichamentos das fontes de conteúdo. |
| `04-rascunhos/` | Escrita livre e versões preliminares antes de entrar no LaTeX. |
| `05-artigo-latex/` | Artigo oficial em LaTeX, modularizado por seções. |
| `06-sistema/` | Documentação técnica do sistema, caso o TCC envolva desenvolvimento. |
| `07-entregas/` | Versões enviadas para avaliação, orientação ou banca. |
| `08-revisoes/` | Pendências, checklists e histórico de ajustes. |
| `09-referencias-formato/` | Exemplos, templates e guias usados para entender estrutura/formatação, não conteúdo. |

## Referências de formato já mapeadas

### Outros TCCs

Local: `09-referencias-formato/outros-tccs/`

- `TCC2_-_Gestao_Financeira_MEI.pdf`
- `TCC_Serviço_para_FLUXOS_CONFIGURAVEIS.pdf`
- `TCC_William_Cardozo_ADORO_PET.pdf`
- `resumo-formato.md`

Uso: entender estrutura de artigo, seções, extensão, uso de figuras, apêndices, referências e estilo geral.

### Normas, guias e template em PDF

Local: `09-referencias-formato/normas-e-guias/`

- `Template_Artigo SSI.docx.pdf`
- `7. Como elaborar um artigo.pptx.pdf`
- `guia-de-boas-praticas-na-pesquisa-cientifica.pdf`
- `Manual-para-elaboracao-de-trabalhos-academicos.pdf`

Uso: regras de formatação, estrutura esperada, limites de páginas, resumo, palavras-chave, referências, anexos/apêndices, boas práticas contra plágio e padrões gerais de trabalhos acadêmicos.

### Template LaTeX

Local: `09-referencias-formato/template-latex/`

Uso: base técnica para preparar o artigo oficial em LaTeX.

Pendências antes de usar como base final:

- Corrigir typos identificados no template: `Conslusão` e `Metologia`.
- Revisar orientador/coorientador.
- Confirmar se a fonte deve ser Arial ou se o uso de `lmodern` será aceito.
- Configurar margens explicitamente, se necessário.
- Confirmar espaçamento correto: 1,15 ou 1,5.
- Remover textos explicativos em azul quando o artigo real começar.

## Decisões tomadas

| Data | Decisão | Motivo/impacto |
| --- | --- | --- |
| 2026-05-01 | Separar referências de formato e referências de conteúdo. | Evita misturar exemplos/templates com fontes teóricas do tema. |
| 2026-05-01 | Usar Markdown para planejamento, fichamentos e rascunhos. | Facilita escrita inicial e organização das ideias. |
| 2026-05-01 | Usar LaTeX para o artigo oficial em crescimento. | Evita deixar formatação, referências e estrutura para o fim. |
| 2026-05-01 | Criar este mapa como memória viva do projeto. | Centraliza estado, estrutura, decisões e próximos passos. |
| 2026-05-01 | Criar tres skills de apoio ao TCC. | Simplifica o fluxo em backlog/escrita, revisao e LaTeX. |
| 2026-05-01 | Definir tema, título, problema, hipótese e objetivos iniciais do TCC. | Permite iniciar protocolo de pesquisa, backlog, levantamento de fontes e escrita da introdução. |
| 2026-05-01 | Registrar fontes externas do software Partilha Certa. | Permite consultar README.md e CLAUDE.md do sistema sem copiar o projeto para o repositório do TCC. |
| 2026-05-02 | Definir estrutura prevista do referencial teórico. | Orienta levantamento de fontes e escrita da seção 2 do artigo. |
| 2026-05-02 | Confirmar que a etapa atual é TCC1. | Ajusta o planejamento para artigo de 7 a 10 páginas, com foco em proposta, fundamentação, metodologia e considerações parciais. |
| 2026-05-02 | Usar `C:\projetos\Herança+\heranca-app\CLAUDE.md` como fonte da verdade técnica do Partilha Certa. | Garante que o escopo jurídico e a descrição do sistema no TCC sejam validados contra o comportamento real documentado do software. |
| 2026-05-02 | Consolidar escopo jurídico inicial em `06-sistema/requisitos/escopo-juridico.md`. | Separa regras centrais, secundárias e fora do escopo, com aderência ao sistema real. |
| 2026-05-02 | Criar quadro resumido do escopo do sistema em `06-sistema/requisitos/quadro-escopo-sistema.md`. | Fornece uma versão compacta do escopo para adaptação à metodologia ou seção do sistema no artigo. |
| 2026-05-02 | Confirmar Rodrigo Prestes Machado como orientador. | Permite preparar a identificação do artigo e remover pendência de autoria/orientação. |
| 2026-05-02 | Confirmar que o artigo terá Abstract e Keywords, mas que serão redigidos ao final. | Evita antecipar tradução antes de estabilizar resumo, objetivos, metodologia e resultados esperados. |
| 2026-05-02 | Manter cronograma fora do artigo até segunda ordem. | O cronograma permanece como planejamento interno, salvo solicitação posterior do orientador ou da disciplina. |
| 2026-05-02 | Usar `Considerações Parciais` como seção final do TCC1. | Deixa claro que o TCC1 fecha a proposta e prepara a continuidade da validação e análise no TCC2. |
| 2026-05-04 | Registrar `Manual-para-elaboracao-de-trabalhos-academicos.pdf` como guia de apoio à criação e formatação do trabalho. | Complementa as normas e guias usados para estrutura, apresentação e padronização acadêmica, sem misturar com fontes de conteúdo. |
| 2026-05-04 | Gerar material preliminar em PDF para envio ao orientador. | Consolida tema, problema, objetivos, justificativa, introdução preliminar, estrutura do referencial, metodologia prevista, escopo do sistema e referências iniciais em `07-entregas/tcc1/2026-05-04-material-preliminar-orientador.pdf`. |

## Pontos a confirmar

- Tema do TCC.
- Se a entrega final será somente PDF ou também arquivos-fonte LaTeX.



## Sistema Partilha Certa

As informações técnicas do software Partilha Certa ficam em fontes externas registradas em:

`06-sistema/fontes-do-sistema.md`

Fonte principal do sistema:

- **Caminho local:** `C:\projetos\Herança+\heranca-app`
- **Repositório remoto:** `https://github.com/Lorandi/heranca-app`

Essas fontes devem ser usadas como documentação técnica do sistema, não como referência acadêmica. Conteúdos extraídos delas devem ser sintetizados e adaptados ao texto do TCC.

Arquivos derivados já criados:

| Arquivo | Uso |
| --- | --- |
| `06-sistema/requisitos/escopo-juridico.md` | Matriz detalhada do escopo jurídico, com aderência ao sistema real. |
| `06-sistema/requisitos/quadro-escopo-sistema.md` | Quadro resumido do escopo para adaptação ao artigo. |

## Skills de apoio

As seguintes skills foram criadas em `C:\Users\rodri\.codex\skills` para apoiar o fluxo do TCC:

| Skill | Quando usar | Responsabilidade |
| --- | --- | --- |
| `tcc-backlog-escrita` | Planejamento, backlog, próximos passos, estruturação e escrita inicial. | Organizar o avanço do TCC, quebrar tarefas, apoiar escrita em Markdown e atualizar a memória do projeto. |
| `tcc-revisor` | Revisão de trechos, seções ou versões antes de evoluir ou enviar ao orientador. | Avaliar coerência, clareza, formato, lacunas, citações, referências e sugerir melhorias. |
| `tcc-latex` | Qualquer tarefa ligada ao artigo oficial em LaTeX. | Preparar e editar `main.tex`, seções, `referencias.bib`, figuras, quadros, tabelas, anexos, apêndices e compilação. |

## Próximas ações

1. Validar problema, hipótese e objetivos com o orientador.
2. Confirmar nome do orientador ou orientadora.
3. Levantar referências de conteúdo sobre direito sucessório, Lawtech, modelagem de domínio e validação de software.
4. Criar fichamentos das fontes principais em `03-fichamentos/por-fonte/`.
5. Revisar e amadurecer o rascunho da introdução em `04-rascunhos/introducao.md`.
6. Escrever rascunho da metodologia em `04-rascunhos/metodologia.md`, usando `06-sistema/requisitos/quadro-escopo-sistema.md`.
7. Preparar o template LaTeX oficial em `05-artigo-latex/`.

## Convenções de organização

- Usar `09-referencias-formato/` apenas para documentos sobre formato, normas e exemplos.
- Usar `02-referencias-conteudo/` apenas para fontes que sustentam o conteúdo do TCC.
- Registrar toda fonte aproveitada em `02-referencias-conteudo/fontes.md`.
- Criar um fichamento para cada fonte relevante em `03-fichamentos/por-fonte/`.
- Manter entregas com data no nome, por exemplo: `2026-05-01-tcc1-v1.pdf`.
- Registrar feedbacks importantes em `08-revisoes/historico-feedbacks.md`.
- Atualizar este arquivo sempre que a estrutura, o tema ou o escopo mudar.
