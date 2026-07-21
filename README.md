# formacao-cs-mainframe-cobol

Este repositório organiza a construção progressiva de uma formação em Ciência da Computação voltada para sistemas corporativos, Mainframe e COBOL. A proposta não é começar pela sintaxe de uma linguagem, por comandos de ferramenta ou por exemplos rápidos. O ponto de partida é a base conceitual que permite entender por que sistemas existem, como dados são representados, como programas processam informação, como computadores executam instruções e como ambientes corporativos exigem confiabilidade, rastreabilidade e operação disciplinada.

Este projeto não é um curso rápido de COBOL, não é uma apostila de sintaxe e não é uma coleção de exemplos soltos. COBOL aparecerá como consequência de uma sequência de fundamentos: computação, lógica, dados, arquitetura de computadores, sistemas operacionais, estruturas de dados, algoritmos, arquivos, bancos de dados, redes, engenharia de software, processamento batch, sistemas críticos, Mainframe, z/OS, JCL, VSAM, DB2 e CICS.

## Visao geral do projeto

A formação será construída em ciclos e fases. Cada fase terá objetivo próprio, escopo delimitado, critérios de domínio e conexão explícita com as fases anteriores e posteriores. O material deve permitir estudo autônomo, mas não deve ser escrito como resumo. As futuras aulas precisam funcionar como capítulos de estudo: com explicação desenvolvida, exemplos contextualizados, transições claras e fechamento.

O repositório começa com uma fundação organizacional, pedagógica e editorial. Antes de criar aulas, exercícios ou exemplos de código, é necessário registrar a direção do projeto, a ordem de desenvolvimento, os critérios de qualidade e os modelos que serão usados para manter consistência.

## Estado atual do percurso

A **Fase 0 — Alfabetização Técnica**, primeira fase do Ciclo 1 — Base Computacional, possui 12 aulas revisadas e materiais de consolidação e está disponível para estudo. A **Fase 1 — Pensamento Computacional: De problemas informais a soluções estruturadas**, segunda fase do mesmo ciclo, está em planejamento. Seu planejamento fica em `ciclo-01-base-computacional/fase-01-pensamento-computacional/`.

## Por que comecar pelos fundamentos

Mainframe e COBOL não são assuntos isolados. Eles aparecem em ambientes onde dados precisam ser processados com previsibilidade, onde operações de negócio dependem de arquivos, transações, bancos de dados, rotinas batch, integração e manutenção de sistemas de longa duração. Sem compreender esses fundamentos, o aluno pode até copiar comandos ou ler pequenos trechos de código, mas terá dificuldade para entender o comportamento de sistemas reais.

Começar pela base reduz atalhos perigosos. Um programa COBOL que lê um arquivo, atualiza registros ou participa de uma rotina batch pressupõe conhecimento sobre representação de dados, processamento sequencial, persistência, controle de erro, sistemas operacionais, contratos de entrada e saída e regras de negócio. A formação deve tornar esses pressupostos visíveis antes de pedir que o aluno escreva código.

## Publico-alvo

Este projeto é destinado a pessoas que desejam estudar Mainframe e COBOL com base sólida, incluindo iniciantes em tecnologia, estudantes de programação, profissionais em transição para sistemas corporativos e desenvolvedores que já programam em outras linguagens, mas não compreendem ainda o contexto operacional de ambientes mainframe.

O material deve acolher quem está começando sem reduzir os assuntos a definições rasas. Termos técnicos serão introduzidos com cuidado, explicados em camadas e retomados quando forem relevantes para sistemas reais.

## Perfil de saida esperado

Ao final da formação completa, espera-se que o aluno consiga compreender sistemas corporativos de forma sistêmica. Isso inclui entender dados, arquivos, processamento batch, transações, bancos de dados, integração, manutenção, documentação, rastreabilidade, operação e código COBOL em contexto.

O objetivo não é formar alguém que apenas reconheça comandos. O perfil esperado é de uma pessoa capaz de ler sistemas, fazer perguntas corretas, compreender impactos, preservar regras de negócio, analisar fluxos de dados e evoluir aplicações com responsabilidade.

## Como o projeto sera construido

O projeto será desenvolvido em etapas pequenas. Primeiro, esta fundação define diretrizes, roadmap, ciclos, templates, glossário inicial e critérios de qualidade. Depois, cada fase será trabalhada individualmente, começando pela Fase 0, sem avançar para a fase seguinte antes de haver coerência mínima na fase atual.

Cada novo conteúdo deve consultar os documentos existentes antes de criar arquivos adicionais. O roadmap orienta a sequência; as diretrizes editoriais orientam a forma de escrita; os templates orientam a estrutura mínima; os critérios de qualidade ajudam a revisar profundidade, clareza e continuidade.

## O que nao sera feito no inicio

No início, este projeto não criará aulas completas, exemplos COBOL, código, Dockerfile, Makefile, ambiente de desenvolvimento, exercícios práticos ou módulos inteiros. Essas partes dependem de preparação conceitual e de uma organização pedagógica que ainda precisa ser consolidada fase por fase.

Também não serão criados documentos apenas para preencher estrutura. Cada arquivo precisa ter função clara dentro da formação.

## Como usar este repositorio durante a construcao

Use este repositório como uma base de continuidade. Antes de pedir uma nova etapa, consulte o roadmap, as diretrizes do projeto, as diretrizes editoriais e a ordem de desenvolvimento. O trabalho deve sempre preservar a progressão: primeiro entender o que será ensinado, depois definir escopo, depois criar conteúdo, depois revisar qualidade.

Ao criar novos prompts, peça uma etapa pequena e verificável. Evite solicitações como "crie toda a formação" ou "desenvolva todas as aulas". O projeto foi desenhado para crescer por camadas, mantendo coerência entre fundamentos e aplicação futura em Mainframe e COBOL.

## Como os proximos prompts devem respeitar o projeto

Todo prompt futuro deve respeitar as diretrizes registradas neste repositório. Isso significa não antecipar código quando o assunto ainda é conceitual, não transformar aulas em listas curtas, não avançar para COBOL antes da base, não usar linguagem promocional e não ignorar a conexão entre cada fase e a formação completa.

Quando um conteúdo parecer superficial, ele deve ser revisado com base em critérios explícitos: profundidade, clareza, continuidade textual, precisão técnica, conexão com sistemas reais e utilidade para estudo autônomo.
