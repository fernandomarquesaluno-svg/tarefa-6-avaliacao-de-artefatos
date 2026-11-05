# Tabela técnica comparativa — Tarefa 6

Fernando Henrique de Souza Marques · 05/11/2026

**Objeto:** processos de avaliação de artefatos científicos de três eventos. As células sintetizam as regras publicadas nas fontes oficiais; vantagens e limitações ao final são análise do autor, não critérios oficiais. Os selos não são intercambiáveis.

## Escopo, entrada e fluxo

| Dimensão | SBSeg 2026 | USENIX Security 2025 | MODELS 2025 |
|:--|:--|:--|:--|
| Objeto | Artefato relacionado a artigo científico, com pacote e documentação para avaliação. | Artefato de artigo aceito; verificação de disponibilidade e avaliação posterior facultativa. | Artefato associado a artigo aceito, submetido à trilha de avaliação. |
| Entrada examinada | Artigo, repositório/pacote, documentação e instruções de instalação e execução. | Artigo aceito, artefato e local de preservação; para avaliação adicional, apêndice de artefato e instruções. | Pacote do artefato, README, arquivo STATUS e indicação dos selos solicitados. |
| Etapas | Revisão inicial **r1** → parecer por critério → rebuttal dos autores → **r2-decision** → decisão e divulgação. | **Fase 1:** disponibilidade antes da versão final do artigo, com exceções justificadas. **Fase 2:** avaliação facultativa de funcionamento/reprodução, com checagem, interação, execução e decisão. | Submissão → checagem inicial (“kick the tires”) → comunicação e eventuais correções → avaliação por pelo menos dois revisores → decisão. |
| Papel dos autores | Disponibilizar o pacote e responder ao parecer na fase de rebuttal. | Depositar material; esclarecer problemas durante a avaliação opcional. | Preparar pacote e STATUS; responder impedimentos apontados na checagem. |
| Natureza da execução | Revisores inspecionam e executam o que for necessário para fundamentar os selos pedidos. | Na fase 2, uso do artefato para testar funcionalidade e, se solicitado, resultados. | Revisores usam o artefato conforme as instruções para avaliar os critérios solicitados. |
| Saída | Recomendações e decisão para D, F, S e R, com justificativa. | Avaliação de disponibilidade e, conforme a fase 2, Functional e Results Reproduced. | Available e/ou Evaluated (Functional ou Reusable), conforme a decisão. |

## Critérios e evidências

| Dimensão | SBSeg 2026 | USENIX Security 2025 | MODELS 2025 |
|:--|:--|:--|:--|
| Disponibilidade | **D — Disponível:** acesso e documentação conforme as instruções da edição. | **Available:** artefato acessível por mecanismo duradouro; exceção de compartilhamento não concede automaticamente o selo. | **Available:** disponibilização duradoura do pacote; edição requer versão arquivada com DOI. |
| Funcionalidade | **F — Funcional:** evidências de execução de ao menos algumas funcionalidades; não exige, por si só, reproduzir todos os resultados. | **Functional:** funcionamento verificado na avaliação opcional. | **Evaluated—Functional:** o artefato funciona para o uso proposto; distinguido de Available. |
| Qualidade para uso futuro | **S — Sustentável:** organização e documentação que facilitem entendimento e continuidade. | Não há selo homônimo a S nesta comparação; evitar equivalência automática. | **Evaluated—Reusable:** considera potencial de reúso, distinto do S do SBSeg. |
| Reprodução de resultados | **R — Reprodutível:** reprodução das principais reivindicações do artigo com evidência. | **Results Reproduced:** resultados do artigo examinados na avaliação opcional. | **Results Validated** não é concedido nesta etapa de avaliação. |
| Evidência mínima de execução | Comandos, saídas e observação das funções ligadas ao selo F; experimentos principais para R. | Artefato usado pelos avaliadores, instruções e saídas que sustentem os selos solicitados. | Execução e documentação suficientes para o selo solicitado, registradas pelos avaliadores. |
| Preservação | Repositório estável pode atender à política da edição; seguir a instrução vigente. | Arquivo de preservação permanente; GitHub isolado não satisfaz essa exigência. | Arquivo permanente com DOI para a versão avaliada. |
| Impedimentos e correções | Parecer r1 e resposta dos autores antes da decisão r2. | Checagem e discussão de impedimentos com os autores na fase 2. | Checagem inicial comunica falhas de empacotamento/execução e admite correções. |

## Síntese crítica

| Perspectiva | SBSeg 2026 | USENIX Security 2025 | MODELS 2025 |
|:--|:--|:--|:--|
| Semelhança | Exige evidência verificável para fundamentar um selo. | Exige evidência verificável para fundamentar um selo. | Exige evidência verificável para fundamentar um selo. |
| Diferença marcante | Quatro dimensões D/F/S/R na mesma rubrica. | Disponibilidade anterior à versão final e etapa prática adicional opcional. | Separa Available de Evaluated e distingue Functional de Reusable. |
| Vantagem¹ | Rubrica explícita para disponibilidade, funcionamento, sustentabilidade e reprodução. | Diferencia preservação do exame prático e abre interação para resolver obstáculos. | Checagem inicial e consideração explícita do reúso. |
| Limitação¹ | A reprodução pode depender de ambiente, recursos e tempo dos avaliadores. | Arquivamento e execução experimental podem demandar mais esforço. | Nesta etapa, não há selo que valide resultados científicos. |
| Pergunta orientadora | O pacote está acessível, funciona, pode ser mantido e reproduz as principais alegações? | Está preservado e, caso avaliado, funciona e reproduz resultados? | Está disponível e pode ser usado ou reutilizado conforme sua proposta? |

¹ Interpretações analíticas desta comparação, não juízos oficiais dos eventos. **F ≠ R; S ≠ Reusable; R ≠ Results Reproduced por mera semelhança de nome.** É preciso aplicar a redação e o procedimento de cada edição.

## Fontes oficiais

- [SBSeg 2026 — instruções de revisão](https://doc-artefatos.github.io/sbseg2026/revinstrucoes.html) e [submissão](https://doc-artefatos.github.io/sbseg2026/subinstrucoes.html).
- [USENIX Security 2025 — Call for Artifacts](https://www.usenix.org/conference/usenixsecurity25/call-for-artifacts), [submissão](https://secartifacts.github.io/usenixsec2025/instructions) e [guia de avaliação](https://secartifacts.github.io/usenixsec2025/guide).
- [MODELS 2025 — Artifact Evaluation](https://conf.researchr.org/track/models-2025/models-2025-artifact-evaluation).
