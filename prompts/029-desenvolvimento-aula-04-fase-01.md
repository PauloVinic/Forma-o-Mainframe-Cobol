# Prompt 029 — Desenvolvimento da Aula 04 da Fase 1

## Objetivo e escopo

Desenvolver integralmente a **Aula 04 — Abstração e modelos** e a **Prática 04 — Dois modelos do mesmo problema**, atualizando minimamente o estado da fase e o roteiro. O trabalho introduz C04 nos níveis 2 e 3 e inicia o nível 4 em caso simples, sem alterar materiais anteriores ou antecipar padrões, representações formais, algoritmos, programação ou COBOL.

## Documentos lidos

Foram lidos integralmente: `DIRETRIZES_DO_PROJETO.md`, `DIRETRIZES_EDITORIAIS.md`, `MANIFESTO_PEDAGOGICO.md`, `planejamento/criterios-de-qualidade.md`, os dois templates; todos os documentos estruturais listados da Fase 1; Aulas 01, 02 e 03 revisadas; Prática 03 revisada; Prompt 028; e as partes pertinentes da Fase 0 sobre sistema, fronteira, ambiente, dado, informação, contexto, estado, componente, relação, interface, representação, arquivos e formatos.

## Decisões conceituais

Definição operacional de abstração:

> Abstração é a seleção intencional de aspectos relevantes de um objeto, problema ou sistema para uma pergunta e um propósito declarados, em determinado nível, com omissão controlada dos demais aspectos e explicitação dos limites produzidos.

Definição operacional de modelo:

> Modelo é uma construção deliberada que organiza aspectos selecionados e relações de um objeto de interesse para descrever, explicar, comparar, monitorar, prever com ressalvas, comunicar ou apoiar uma decisão, dentro de propósito, fronteira, público e condições de validade declarados.

Foram distinguidos abstração e vagueza; abstração e resumo; modelo, realidade, dado, informação e representação; modelo e especificação; desconhecido e omitido; relação e causalidade; função matemática e processamento real.

Propósito, pergunta, público, perspectiva, horizonte e responsabilidade precedem a seleção. Fronteira do problema, da decomposição e do modelo foram diferenciadas. Os níveis agregado, intermediário e detalhado foram tratados sem hierarquia de importância. Omissões foram classificadas como deliberadas, desconhecidas, adiadas, fora da fronteira, agregadas ou indevidas.

Objetos/entidades, atributos, condições e relações foram introduzidos analiticamente, sem banco de dados, arquitetura ou contratos técnicos. Domínio de validade, pressupostos, perdas de informação, falsa precisão, viés de seleção, agregação, exceção crítica, rastreabilidade e revisão receberam tratamento explícito.

## Caso, matemática e prática

O caso preserva dois centros, três produtos, 192 de 2.400 linhas, taxas de 6%, 10,8% e 8%, 29 históricos incompletos, causas não estabelecidas, meta candidata e quatro proteções. Foram construídos modelos operacional e gerencial, comparados por unidade, seleção, perda, evidência, decisão e uso vedado. Casos adicionais são marcados como hipotéticos.

A matemática inclui `S ⊆ U`, relação como subconjunto de `A × B` e função `f: X → Y`, com domínio, codomínio, uma saída por entrada admissível, dados incompletos e ausência de causalidade ou determinismo presumido. Não inclui propriedades avançadas ou prova.

A prática exige dois modelos, quadro comparativo, auditoria de oito omissões, seis casos conceituais, matemática, revisão e autoavaliação. A solução comentada oferece possibilidades sem preencher todas as células e sem substituir a tentativa.

## Exercícios, fontes e carga

A aula contém 10 exercícios essenciais e 7 de aprofundamento opcional: três objetivas com distratores plausíveis, questões dissertativas, análises de caso, conjuntos, relação/função, contraexemplo e revisão.

Foram usadas seis fontes já verificadas e registradas na fase: Wing (2006), CS2023, Pólya (1957), Simon (1962), Rosen (2019) e ISO/IEC/IEEE 24765:2017. Não foi necessária nova referência.

A trilha essencial integra leitura, recuperação, exercícios, prática, solução e revisão em aproximadamente 7h30 a 10h. A carga completa opcional é de aproximadamente 11h30 a 15h. A prática essencial leva 3h15 a 4h20; o aprofundamento acrescenta 2h a 3h.

## Verificações e fronteiras curriculares

Devem ser verificados contagens, estrutura, UTF-8, links, matemática, `git diff --check`, ausência de temporários e escopo do diff. Não há código, pseudocódigo, fluxograma, algoritmo, programação, COBOL, modelagem de banco de dados ou arquitetura.

A Aula 05 permanece responsável por padrões, classificação, generalização, regras, exceções e validação de generalizações. A Aula 06 permanece responsável pela seleção e combinação detalhada de representações, diagramas, fluxogramas e pseudocódigo. Estado aparece somente como condição relevante, sem rastreamento.

## Métricas

- Aula: 5.971 palavras, 474 linhas, 15 H2 e 42 H3.
- Prática: 2.324 palavras, 253 linhas, 15 H2 e seis H3.
- Exercícios: 10 essenciais e sete de aprofundamento opcional.
- Casos: estoque progressivo, atendimento guiado, seis testes conceituais na prática e casos transferidos nos exercícios.
- Fontes: seis.
- Conceitos matemáticos: subconjunto, produto cartesiano, relação, função, domínio e codomínio.
- Carga essencial: aproximadamente 7h30 a 10h.
- Carga completa opcional: aproximadamente 11h30 a 15h.
- Prática essencial: 3h15 a 4h20; aprofundamento: 2h a 3h adicionais.

Contagens descrevem os artefatos e não substituem avaliação técnica e pedagógica.
