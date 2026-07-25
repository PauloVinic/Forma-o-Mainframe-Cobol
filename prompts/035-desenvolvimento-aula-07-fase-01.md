# Prompt 035 — Desenvolvimento da Aula 07 da Fase 1

## Objetivo e escopo

Desenvolver a Aula e a Prática 07, introduzindo C07 nos níveis 2 e 3 e início do 4. O P3 começa com contrato e algoritmo inicial independente de linguagem, sem rastreamento detalhado, decisões completas ou repetição.

## Documentos lidos

Foram lidos integralmente diretrizes, manifesto, critérios, templates, documentos da Fase 1, Aulas 01–06 revisadas, Prática 06 e Prompt 034. Também foram consultadas partes pertinentes da Fase 0 sobre programa, código, execução, entrada, processamento, saída, requisito, especificação, estado, erro e comportamento esperado.

## Definição e contrato

Algoritmo foi definido operacionalmente como descrição finita, precisa e independente de linguagem de procedimento efetivo que transforma, para cada instância admissível de uma classe declarada, entradas em saídas conformes à especificação e termina em passos finitos.

A definição foi qualificada como convenção do curso para algoritmos terminantes, compatível com fontes clássicas sem pretensão de universalidade. Classe, instância, universo, domínio, entrada, saída, pré-condição, pós-condição, contrato e limites foram diferenciados.

## Efetividade, precisão, ordem e término

Efetividade foi separada de rapidez, automação e implementação. Precisão foi tratada no passo e na coerência do conjunto. Dependências externas precisam de contrato. Ordem foi reconhecida sem rastreamento de estados.

Descrição finita foi separada de execução finita. O argumento de término cobre toda entrada admissível, uma instância por execução, verificações limitadas e ausência de espera indefinida.

## Correção, determinismo e entidades próximas

Correção intuitiva relaciona grupos do domínio às pós-condições e limites; exemplos não são prova. Contraexemplo exige instância admissível e produz revisão versionada.

Determinismo foi apresentado sem transformá-lo em requisito universal. Não determinismo introdutório foi separado de ambiguidade, aleatoriedade e concorrência. Algoritmo foi distinguido de representação, pseudocódigo, fluxograma, código, programa, implementação, solução de instância, procedimento, processo organizacional e heurística.

## Matemática e P3

Foram usados domínio `D`, saídas `S`, relação de especificação `E ⊆ D × S`, função `f: D → S` quando existe saída única, pares `(d, s)`, sequência finita de passos e propriedade `P(d, s)`. Relação e função não foram confundidas com algoritmo.

O estoque recebeu contrato e algoritmo inicial para preparar uma ocorrência por execução. Desconhecidos, ausência de causalidade, autoridade e limites foram preservados. O caso fica preparado para rastreamento na Aula 08.

## Prática e exercícios

A prática contém sete candidatos, duas instâncias iniciais, contrato, linguagem estruturada, pseudocódigo, análise de efetividade, término, correção intuitiva, quatro casos, contraexemplo T5, revisão e transferência metodológica ao P3.

Há 14 exercícios essenciais e cinco opcionais. Gabarito interno das objetivas: 1-B; 2-C; 3-B.

## Fontes e limites

Foram usadas fontes já registradas: CS2023; Cormen et al., 4ª edição; Knuth, volume 1; Pólya; Rosen; e Lehman, Leighton e Meyer. Os registros foram verificados em páginas oficiais do currículo, MIT Press, Pearson e MIT OpenCourseWare. Não foi necessária nova referência.

Não há código executável, linguagem real, COBOL, JCL, repetição, contador, acumulador, rastreamento detalhado, lógica completa, tabela-verdade, prova formal, plano de testes ou análise assintótica.

## Métricas e carga

Medição anterior ao registro:

- aula: 6.115 palavras, 465 linhas, 16 H2 e 31 H3;
- prática: 2.420 palavras, 277 linhas, 14 H2 e dois H3;
- exercícios: 19, sendo 14 essenciais e cinco opcionais;
- candidatos: sete;
- contratos centrais: três — transação, estoque e agendamento;
- casos explícitos da prática: I1, I2, T1–T5 e um caso fora da classe;
- fontes: seis;
- conceitos matemáticos: domínio, conjunto de saídas, relação, função, par ordenado, sequência e pós-condição;
- leitura: 2h15–2h45;
- exercícios: 1h30–2h;
- prática: 3h15–4h;
- revisão: 30–45 min;
- trilha essencial: 7h50–10h;
- percurso completo opcional: 11h30–15h.

## Verificações e progressão

Foram validados UTF-8, links, whitespace, escopo, matemática e pseudocódigo. Aulas 08–10, 12 e 13 permanecem responsáveis por estado, decisões, repetição, testes e eficiência. A Aula 07 fica pronta para revisão técnica e pedagógica antes da Aula 08.
