# Prompt 025 — Desenvolvimento da Aula 02 da Fase 1

## Objetivo

Desenvolver integralmente a **Aula 02 — O que é um problema** e sua prática associada, avançando do panorama da Aula 01 para a introdução formal das competências **C01 — Formular o problema** e **C02 — Especificar a transformação**. A entrega deveria ensinar o aluno a transformar situações vagas em formulações iniciais delimitadas, analisáveis e verificáveis, sem escolher antecipadamente ferramenta, automação, modelo ou algoritmo.

## Escopo executado

Foram criados:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-02-o-que-e-um-problema.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-02-formulando-problemas.md`;
- `prompts/025-desenvolvimento-aula-02-fase-01.md`.

Foram atualizados minimamente, apenas para registrar o novo estado:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`.

Não foram alterados arquivos da Fase 0, outras aulas, ementa, plano da fase, matriz de competências, critérios de domínio, glossário, mapa conceitual, planos de práticas ou avaliação, README global ou ROADMAP.

## Documentos lidos

O desenvolvimento tomou como base:

- `DIRETRIZES_DO_PROJETO.md`;
- `DIRETRIZES_EDITORIAIS.md`;
- `MANIFESTO_PEDAGOGICO.md`;
- `planejamento/criterios-de-qualidade.md`;
- `templates/TEMPLATE_AULA.md`;
- `templates/TEMPLATE_EXERCICIO.md`;
- README, ementa, plano da fase, roteiro de aulas, matriz de competências, critérios de domínio, glossário, mapa conceitual, guia de estudo, plano de práticas, plano de avaliação e referências da Fase 1;
- a Aula 01 revisada, sua prática associada e o Prompt 024, para continuidade conceitual e controle de antecipação;
- as sínteses e os critérios de domínio das aulas pertinentes da Fase 0, especialmente sistema, dados, processamento, entrada e saída e investigação de erro;
- os limites das Aulas 03 a 07 no roteiro da Fase 1.

O arquivo solicitado `templates/TEMPLATE_ESTUDO.md` não existe no repositório. Foram usados como equivalentes existentes, sem criar ou renomear templates, `templates/TEMPLATE_ESTUDO_DIRIGIDO.md` e `templates/TEMPLATE_ESTUDO_DE_CASO.md`. O primeiro orientou recuperação, sinais de domínio e registro de lacunas; o segundo orientou casos realistas, análise guiada e fechamento sem antecipar tecnologia.

Depois da redação, a Aula 02 e a Prática 02 foram lidas integralmente, e os diffs do README da fase e do roteiro foram inspecionados. Os dois registros preservam que a Aula 01 foi revisada, registram Aula 02 e prática como desenvolvidas e mantêm as Aulas 03 a 14 como planejadas.

## Definição operacional adotada

A aula adota:

> **Problema é um objeto delimitado de análise que envolve uma diferença, um obstáculo, um risco, uma incerteza relevante, uma decisão necessária, uma necessidade não atendida ou uma oportunidade de melhoria. Sua formulação relaciona a situação a interessados e objetivos e torna explícitos, na medida necessária, estado atual e pretendido, evidências, escopo, condições, restrições, pressupostos, questões em aberto e critérios pelos quais respostas poderão ser avaliadas.**

A definição é declarada como convenção pedagógica ampla, não universal nem neutra. Ela admite problemas que não começam por uma falha observada e exige que lacunas permaneçam explícitas quando causa, estado desejado, autoridade ou critério ainda não forem conhecidos.

## Decisões terminológicas

- **Situação** é o contexto no qual algo ocorre; pode conter vários problemas e perspectivas.
- **Necessidade** expressa algo considerado necessário ou valioso por alguém, mas não delimita sozinha o problema.
- **Problema** é o objeto de análise formulado e revisável; não é sinônimo da primeira reclamação.
- **Solução proposta** é uma alternativa de intervenção e permanece fora da definição até ser avaliada.
- Pergunta, decisão, risco e oportunidade podem motivar a formulação sem serem tratados como uma única categoria indiferenciada.
- **Interessado**, **pessoa afetada** e **responsável pela decisão** foram separados para não confundir exposição, voz e autoridade.
- Objetivo, estado atual, estado desejado e resultado esperado cumprem funções diferentes. Resultado esperado também não foi confundido com uma saída técnica.
- Escopo e fronteira se relacionam, mas o primeiro declara o recorte e suas exclusões, enquanto a segunda distingue objeto e ambiente para o propósito adotado.
- Restrição, recurso, preferência e pressuposto foram distinguidos por origem, firmeza e consequência.
- Entrada, saída, regra e condição introduzem C02 no nível da transformação esperada; sua simples enumeração não constitui algoritmo.
- Critério de sucesso, métrica, meta e linha de base foram separados. Critérios de proteção impedem que uma meta isolada seja tratada como sucesso completo.
- Problema mal definido ou pouco estruturado designa aspectos incompletos, ambíguos, instáveis ou conflitantes; não é juízo sobre a importância do relato nem culpa de quem o apresentou.
- Requisito e especificação foram retomados funcionalmente da Fase 0, sem reduzir engenharia de requisitos a uma ficha.

## Situação, necessidade, problema e solução

A progressão usa a solicitação de estoque para mostrar que “evitar falta” expressa uma necessidade, que “ficar sem” ainda admite definições diferentes e que comprar ferramenta de previsão é solução sugerida. A formulação precisa declarar recorte, evidência, objetivo, critérios e incertezas antes de avaliar aumento de estoque, redistribuição, correção de registros ou ferramenta.

Essa separação também aparece em chatbot, inteligência artificial e validação automática. A ausência de determinada tecnologia não foi tratada como problema por si só; o problema deve continuar inteligível caso a tecnologia sugerida seja descartada.

## Sintomas, causas e estatuto das afirmações

Sintoma foi definido como manifestação percebida ou registrada. Causa exige relação sustentada por evidência adequada; hipótese causal é explicação provisória que orienta investigação e admite observações capazes de fortalecê-la ou enfraquecê-la. A formulação pode avançar sem causa confirmada.

Em eixo complementar, a aula diferencia evidência, fato do caso, inferência, hipótese e decisão. Um sintoma pode ser fato, uma causa alegada pode continuar hipótese e uma decisão de intervenção não confirma a hipótese que a motivou. Essa escolha evita transformar associação temporal, testemunho ou cálculo derivado em prova causal.

## Modelo didático de formulação

Foi criado um modelo de perguntas em sete blocos, explicitamente apresentado como andaime, não formulário universal:

1. contexto e relevância;
2. base conhecida;
3. transformação pretendida;
4. delimitação;
5. viabilidade e responsabilidade;
6. avaliação;
7. incerteza e alternativas.

O modelo integra C01 e C02, mas aceita ordem e profundidade diferentes conforme o caso. A qualidade depende das relações e justificativas, não do preenchimento mecânico de todos os campos.

## Matemática introduzida

A matemática foi integrada aos exemplos e limitada ao necessário para tornar critérios legíveis:

- igualdade e desigualdades `<`, `>`, `≤`, `≥` e `=`;
- cálculo de taxa `r = n/N` e conversão para percentual;
- intervalos inclusivos e exclusivos;
- conjuntos simples e pertencimento;
- relação entre linha de base e meta.

Os exemplos registram população, período, denominador e fronteiras. A aula insiste que notação precisa não corrige métrica inadequada, fonte incompleta, meta arbitrária nem efeito colateral ignorado. Não foram introduzidas lógica proposicional, tabela de decisão ou construção algorítmica.

## Caso progressivo

O caso de estoque avança a Aula 01 com dados hipotéticos: 192 de 2.400 linhas de pedido não atendidas integralmente na primeira separação, taxas de 6% no CD Norte, 10,8% no CD Sul e 8% no total, 29 ocorrências sem histórico completo e grupos potencialmente sobrepostos. Saldo desatualizado e atraso de entrada permanecem hipóteses.

A formulação inicial delimita três produtos, dois centros e 28 dias; apresenta a taxa inferior a 3% por centro durante três ciclos como meta candidata ainda não aprovada; inclui proteções contra deslocamento, perdas, custo e divergência; preserva questões sobre contagem, qualidade dos registros, impacto, causas e autoridade. Ela não decompõe o processo, desenha fluxo ou escolhe intervenção.

## Exercícios

Foram criados 15 exercícios:

- 3 questões objetivas com alternativas plausíveis, cujas respostas internas esperadas são 1-b, 2-a e 3-c;
- 5 questões discursivas sobre as distinções e relações centrais;
- 4 análises de caso envolvendo cadastro, indisponibilidade, atendimento e estoque;
- 1 exercício matemático com desigualdade, intervalo e conjunto;
- 1 contraexemplo sobre critério numérico inadequado;
- 1 reescrita de solicitação orientada a ferramenta.

As questões pedem justificativa e não exibem gabarito destacado. A reescrita limita-se a 150–220 palavras, preserva lacunas e não exige especificação completa, decomposição, modelo ou algoritmo.

## Prática associada

A prática possui quatro blocos com funções diferentes:

1. estoque — formulação completa guiada e declaração inicial;
2. benefício — classificação de sintoma, evidência, testemunho, inferência, hipótese causal e decisão;
3. atendimento — conflitos entre objetivos, interessados, afetados ausentes e critérios de proteção;
4. reembolsos — crítica e reescrita de solução prematura, com contraexemplo.

Todos os números são declarados hipotéticos. A solução comentada é posterior à tentativa: oferece um modelo completo somente para o Bloco 1 e comentários selecionados nos demais. A rubrica avalia precisão, evidência, neutralidade quanto à ferramenta, delimitação, interessados, critérios, pressupostos, questões abertas, conflitos, clareza e rastreabilidade. Respostas alternativas permanecem válidas quando justificadas.

## Fontes utilizadas

1. Pólya, *How to Solve It*, para compreensão e revisão do problema sem transformar heurística em sequência universal.
2. Simon, “The Structure of Ill Structured Problems”, para problemas pouco estruturados e graus de indefinição.
3. Kumar et al., *Computer Science Curricula 2023*, para progressão curricular e resolução de problemas independente de linguagem.
4. ISO/IEC/IEEE 24765:2017, para vocabulário de sistemas e software.
5. ISO/IEC/IEEE 29148:2018, para a fronteira com requisitos e especificação.
6. SWEBOK Guide 4.0a, para situar engenharia de requisitos como campo iterativo mais amplo que esta aula.
7. Rosen, *Discrete Mathematics and Its Applications*, para desigualdades, intervalos, conjuntos e pertencimento.

As fontes sustentam decisões específicas; a aula não tenta resumir integralmente resolução de problemas, requisitos ou matemática discreta.

## Métricas reais

As palavras foram contadas com `Measure-Object -Word`; as linhas, com `Get-Content` em UTF-8.

### Aula 02

- 6.638 palavras;
- 371 linhas;
- 25 seções H2 e 11 subseções internas, sendo 8 H3 e 3 H4;
- 15 exercícios;
- 4 tabelas;
- 7 fontes utilizadas.

### Prática 02

- 2.585 palavras;
- 205 linhas;
- 14 seções H2 e 3 subseções H3;
- 5 tabelas;
- 4 blocos de atividade, seguidos por comentários correspondentes;
- 1.603 palavras antes da solução e 982 palavras na solução e autocorreção;
- duração declarada e confirmada pela soma dos blocos: 3 a 4 horas.

## Verificações finais

- os cinco arquivos do escopo passaram por decodificação UTF-8 estrita e não possuem espaços finais;
- o caminho da prática informado nos metadados da aula existe;
- a aula contém 15 exercícios numerados, 30 entradas no mini glossário e quatro tabelas com colunas consistentes;
- a prática contém quatro blocos de tentativa e quatro comentários correspondentes;
- não há bloco de código, pseudocódigo, COBOL ou JCL na aula ou na prática; algoritmo aparece somente para declarar fronteira curricular;
- `templates/TEMPLATE_ESTUDO.md` foi confirmado como ausente e os dois equivalentes registrados existem;
- as duas URLs da aula foram conferidas: o DOI de Simon respondeu diretamente, e o DOI do CS2023, embora bloqueie requisição automatizada, foi confirmado no relatório oficial e no registro da ACM;
- o escopo contém exatamente os cinco caminhos autorizados, sem diff na Fase 0, na Aula 01 ou em documentos estruturais proibidos;
- os diffs de README e roteiro são mínimos e restritos ao estado da Aula 02;
- as métricas foram recalculadas após a revisão conceitual;
- `git diff --cached --check` não encontrou erro e não há arquivo temporário;
- `main` e `origin/main` permaneciam no commit-base `37648ddefe1688ded1bc8576296db38e1a58a977` antes do commit desta entrega.

## Pendências e decisão de prontidão

Não ficou pendência conceitual, pedagógica ou editorial bloqueante. A entrega está pronta para commit e para revisão técnica e pedagógica posterior. Essa revisão deve preceder o desenvolvimento da Aula 03.

## Limites reservados à Aula 03

A Aula 02 estabelece o problema como um todo. Permanecem reservados à Aula 03:

- decomposição funcional, por dados ou por etapas;
- definição de partes, responsabilidades e níveis;
- identificação de dependências e ordem entre partes;
- critérios de granularidade e de parada da decomposição;
- interfaces iniciais;
- análise de duplicidades, lacunas, incompatibilidades e otimização local;
- recomposição e validação do todo.

Não foram construídas árvore de problemas, decomposição do estoque, mapa de dependências, fluxo, modelo detalhado ou algoritmo. Assim, a Aula 03 continua necessária e recebe um todo delimitado para dividir sem perder relações.
