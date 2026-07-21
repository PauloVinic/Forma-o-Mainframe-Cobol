# Prompt 023 — Desenvolvimento da Aula 01 da Fase 1

## Objetivo

Desenvolver integralmente a **Aula 01 — O que é pensamento computacional**, primeira aula da **Fase 1 — Pensamento Computacional: De problemas informais a soluções estruturadas**, e criar sua prática associada. O trabalho permanece conceitual, introdutório e independente de linguagem de programação.

## Escopo executado

Foram criados:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-01-o-que-e-pensamento-computacional.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-01-reconhecendo-pensamento-computacional.md`;
- `prompts/023-desenvolvimento-aula-01-fase-01.md`.

Foram atualizados apenas para registrar o desenvolvimento:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`.

## Documentos lidos

Foram lidos integralmente:

- `DIRETRIZES_DO_PROJETO.md`;
- `DIRETRIZES_EDITORIAIS.md`;
- `MANIFESTO_PEDAGOGICO.md`;
- `planejamento/criterios-de-qualidade.md`;
- `templates/TEMPLATE_AULA.md`;
- `templates/TEMPLATE_EXERCICIO.md`;
- os 12 documentos de planejamento da Fase 1: README, ementa, plano da fase, matriz de competências, critérios de domínio, roteiro, mapa conceitual, guia de estudo, glossário, plano de práticas, plano de avaliação e referências.

O arquivo solicitado `templates/TEMPLATE_ESTUDO.md` não existe no repositório. Foram lidos integralmente os equivalentes disponíveis `templates/TEMPLATE_ESTUDO_DIRIGIDO.md` e `templates/TEMPLATE_ESTUDO_DE_CASO.md`, sem criar ou renomear templates fora do escopo.

Para continuidade conceitual, foram lidas as sínteses e os critérios de domínio das Aulas 01, 02, 04, 05, 07 e 12 da Fase 0.

## Decisões conceituais

- Tratar pensamento computacional como família de práticas e perspectivas, não como método linear ou taxonomia fechada.
- Diferenciar pensamento computacional de programação, uso de computador e qualquer raciocínio organizado.
- Usar os quatro pilares como porta didática, qualificando-os como modelo popular, não consenso universal.
- Dar visibilidade equivalente a representação, dados, estados, automação, verificação, avaliação e revisão.
- Manter pessoas, processos e tecnologia na análise por meio da perspectiva sociotécnica da Fase 0.
- Limitar decomposição, abstração, padrões, procedimentos e algoritmos ao reconhecimento introdutório, preservando o desenvolvimento formal das Aulas 02 a 07.
- Exigir apenas reconhecimento, explicação e aplicação guiada inicial, sem cobrar Nível 4 ou domínio de C01 e C02.

## Definição operacional adotada

Pensamento computacional foi definido como uma família de práticas e perspectivas usada para formular problemas e representar soluções de modo que dados, estados, relações, regras, partes, resultados e limites se tornem explícitos e analisáveis, e que procedimentos ou estratégias possam ser executados, verificados e aprimorados por pessoas, máquinas ou sistemas sociotécnicos, com automatização quando pertinente.

A aula declara que essa é uma definição operacional do curso, inspirada pela literatura e aberta a refinamento, não uma definição acadêmica final.

## Tratamento histórico

O texto distingue antecedentes intelectuais, uso anterior da expressão e difusão contemporânea. Registra com cautela que a expressão aparece pelo menos em *Mindstorms*, de Seymour Papert, em 1980, sem atribuir invenção incontestável. Wing é apresentada como figura central da difusão contemporânea a partir de 2006. National Research Council, Shute e colaboradoras e Denning sustentam a pluralidade, os refinamentos e as críticas posteriores.

## Fontes efetivamente utilizadas

1. Papert, *Mindstorms: Children, Computers, and Powerful Ideas* (1980), para o registro histórico do uso da expressão.
2. Wing, *Computational Thinking* (2006).
3. Wing, *Computational Thinking: What and Why?* (2010).
4. National Research Council, *Report of a Workshop on the Scope and Nature of Computational Thinking* (2010).
5. Denning, *Remaining Trouble Spots with Computational Thinking* (2017).
6. Shute, Sun e Asbell-Clarke, *Demystifying Computational Thinking* (2017).
7. Kumar et al., *Computer Science Curricula 2023*.

## Casos e exercícios

O caso progressivo principal é controle de estoque e reposição, apresentado como solicitação vaga, procedimento informal e formulação estruturada inicial. A aula também usa conciliação de cobranças, rotas, planilha sem formulação, escolha tecnológica prematura, mediação, benefício sociotécnico e pagamentos duplicados.

Foram criados 15 exercícios: três questões objetivas, um exercício adicional de reconhecimento, cinco questões de explicação, três análises de casos, duas reflexões/transferências e uma construção de contraexemplo. Não há gabarito integral dentro da aula; há orientações de autocorreção.

## Prática associada

A prática apresenta quatro situações — estoque, benefício, atendimento e compra cotidiana — com três níveis de descrição cada. O aluno preenche tabela de análise, justifica uma classificação, cria contraexemplo e melhora uma descrição sem completar a especificação. A solução comentada separa evidência, inferência e escolha e aceita classificações alternativas justificadas.

## Métricas

As palavras foram contadas com `Measure-Object -Word`; as linhas, pela leitura do arquivo com `Get-Content` no PowerShell.

### Aula

- 6.495 palavras;
- 468 linhas;
- 31 seções de segundo nível;
- 15 exercícios;
- 3 versões do caso progressivo, 6 exemplos e contraexemplos e 2 descrições da prática guiada, além de 3 casos nos exercícios;
- 7 fontes efetivamente utilizadas;
- leitura estimada em 2 h 30 min a 3 h 15 min;
- carga total sugerida de 7 h 45 min a 9 h 45 min.

### Prática

- 2.456 palavras;
- 198 linhas;
- quatro situações e 12 descrições;
- duração estimada de 2 h 30 min a 3 h.

## Verificações realizadas antes do commit

- a aula ficou dentro da faixa solicitada, com métricas recalculadas após a revisão;
- não há código, notação executável, ensino de sintaxe ou COBOL; pseudocódigo aparece somente como conteúdo futuro, sem exemplo;
- o diretório de aulas contém apenas a Aula 01, além do arquivo `.gitkeep`;
- o diff contém exatamente os cinco caminhos autorizados, sem alteração na Fase 0 ou nos documentos estruturais proibidos;
- os cinco arquivos passaram por leitura UTF-8 estrita;
- os caminhos internos existem e os seis links externos responderam com HTTP 200;
- `git diff --check` não encontrou erro;
- o diff completo foi inspecionado e não há artefatos temporários.

## Pendências

Após esta entrega, a Aula 01 deve passar por revisão técnica e pedagógica antes do desenvolvimento da Aula 02. Nenhum conteúdo da Aula 02 foi produzido antecipadamente.
