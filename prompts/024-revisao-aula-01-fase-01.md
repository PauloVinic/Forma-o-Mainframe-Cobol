# Prompt 024 — Revisão da Aula 01 da Fase 1

## Objetivo

Realizar uma revisão técnica e pedagógica localizada da **Aula 01 — O que é pensamento computacional** e de sua prática associada. A revisão preservou a base conceitual da entrega anterior e corrigiu amplitude da definição operacional, fragmentação, repetição, antecipações curriculares, previsibilidade de exercícios, carga mecânica da prática e estimativas de tempo.

## Escopo executado

Foram revisados diretamente:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-01-o-que-e-pensamento-computacional.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-01-reconhecendo-pensamento-computacional.md`.

Foram atualizados minimamente para registrar a revisão:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`.

Foi atualizado por correção bibliográfica comprovada:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/referencias-da-fase.md`.

Foi criado este histórico:

- `prompts/024-revisao-aula-01-fase-01.md`.

## Documentos lidos

Foram lidos integralmente:

- a Aula 01, sua prática associada e o Prompt 023;
- README, ementa, plano da fase, roteiro de aulas, matriz de competências, critérios de domínio, glossário, mapa conceitual, guia de estudo, plano de práticas, plano de avaliação e referências da Fase 1;
- `DIRETRIZES_EDITORIAIS.md` e `MANIFESTO_PEDAGOGICO.md`;
- `planejamento/criterios-de-qualidade.md`;
- `templates/TEMPLATE_AULA.md` e `templates/TEMPLATE_EXERCICIO.md`.

No roteiro, os limites das Aulas 02 a 07 foram lidos integralmente e usados para separar panorama introdutório de desenvolvimento futuro.

## Diagnóstico inicial

A aula estava conceitualmente sólida e dentro da faixa editorial, mas combinava problemas localizados:

- a definição operacional era ampla o bastante para incluir procedimentos humanos organizados sem vínculo suficientemente claro com a computação;
- 31 seções de segundo nível produziam leitura fragmentada e algumas distinções reapareciam em blocos independentes;
- problema, decomposição, abstração, representação e algoritmo recebiam detalhes que reduziam o espaço de descoberta das Aulas 02 a 07;
- a abertura e o caso progressivo repetiam parte do mesmo diagnóstico de estoque;
- as três questões objetivas tinham distratores desiguais, resolvidos em parte por palavras-chave ou alternativas caricatas;
- questões abertas e perguntas de recuperação retomavam funções semelhantes;
- a prática exigia até 120 células discursivas e sua solução respondia quase toda a atividade;
- a estimativa anterior não separava os blocos de trabalho e atribuía tempo excessivo à leitura.

Foram identificados ainda dois erros bibliográficos comprovados em `referencias-da-fase.md`: a entrada de Wing misturava o documento institucional de 2010 com o veículo posterior *The Link*, e a entrada do CS2023 não seguia autoria, título, ano e DOI prescritos pelo relatório.

## Acertos preservados

Permaneceram explícitos:

- a inexistência de definição acadêmica universal;
- a distinção entre pensamento computacional, programação, uso de computador e qualquer raciocínio organizado;
- os quatro pilares como mapa didático recorrente, não taxonomia fechada;
- a perspectiva sociotécnica e a possibilidade de execução por pessoas, máquinas ou combinações;
- verificação, revisão e limites éticos, organizacionais e epistêmicos;
- o caso progressivo de estoque em três versões;
- a separação entre evidência, inferência e lacuna;
- domínio nos níveis 1, 2 e início guiado do 3;
- ausência de trechos de código, notação de pseudocódigo e COBOL.

História, debate conceitual, limites, prática guiada, síntese e critérios observáveis de domínio continuaram como unidades próprias porque anunciam mudanças reais de problema.

## Definição anterior e definição revisada

A definição anterior era:

> Pensamento computacional é uma família de práticas e perspectivas usada para formular problemas e representar soluções de modo que elementos relevantes — como dados, estados, relações, regras, partes, resultados e limites — se tornem explícitos e analisáveis, e que procedimentos ou estratégias possam ser executados, verificados e aprimorados por pessoas, máquinas ou sistemas sociotécnicos, com automatização quando ela for pertinente.

A definição revisada é:

> Pensamento computacional é uma família de práticas e perspectivas orientadas pela computação para formular problemas e representar soluções de modo compatível com o processamento de informação. Nessas representações, elementos relevantes — como dados, estados, decomposições, relações, regras, procedimentos e limites — podem tornar-se explícitos para análise; estratégias podem ser executadas ou simuladas, resultados verificados e soluções revistas por pessoas, máquinas ou sistemas sociotécnicos. Isso não exige programação nem torna a automação obrigatória.

“Orientadas pela computação” e “compatível com o processamento de informação” delimitam a relação distintiva sem exigir programação ou automação. A aula esclarece que a formulação é uma convenção operacional do curso e não um consenso final. Desenvolvimento, síntese e mini glossário foram harmonizados com essa redação.

## Organização estrutural

Foram fundidas:

- relação com Ciência da Computação, distinção de programação, distinção de uso de computador e fronteira com pensamento organizado, sob **Fronteiras do conceito**;
- pessoas, máquinas e sistemas sociotécnicos com escala, repetição e automação, sob **Pessoas, máquinas, escala e automação**;
- exemplos, contraexemplos e confusões recorrentes, com redução de casos equivalentes;
- recuperação ativa e reflexão, preservadas como subseções internas;
- orientações de autocorreção, agora subordinadas aos exercícios.

Decomposição, abstração, padrões, procedimentos, representação e verificação permaneceram como subtítulos sob **Dimensões relacionadas, não etapas isoladas**. Essa estrutura é útil para navegação e cada dimensão cumpre uma função panorâmica diferente. O número de seções de segundo nível caiu de 31 para 24.

## Antecipações reduzidas e progressão preservada

- A situação inicial de estoque passou a introduzir a confusão sem repetir a análise posterior.
- A versão C distingue em tabela o conhecido, a hipótese ou inferência e o ainda desconhecido; ela é chamada apenas de formulação inicial estruturada, não de problema completo, especificação ou algoritmo.
- Procedimentos, algoritmos e representações ficaram no nível de função e distinção, com desenvolvimento remetido às aulas próprias.
- Decomposição e abstração são reconhecidas no caso, mas não produzidas autonomamente.
- Teste, depuração, correção, custos e eficiência continuam apenas sinalizados e remetidos às Aulas 12 e 13.
- Exercícios que pediam melhoria ou formulação de problema foram convertidos em identificação de reduções, evidências, inferências, lacunas e perguntas.

A sequência resultante progride da confusão e do caso corporativo para definição, debate, história, fronteiras, dimensões, agentes e automação, limites, reaplicação, prática guiada, exercícios, síntese e domínio. A Aula 02 continua necessária para formular problemas de maneira disciplinada.

## Exercícios revisados

Foram mantidos 15 exercícios, com funções mais distintas. As três objetivas agora comparam situações plausíveis. As respostas internas esperadas são **1-b, 2-b e 3-b**; elas não aparecem como gabarito na aula. A questão 4 agrupa sinais como evidência fraca ou relevante, ainda inconclusiva, admite empates e pede informação capaz de alterar a classificação.

Nas abertas:

- história passou a distinguir uso anterior, difusão e ausência de definição final;
- a definição é examinada por consequência de remover um elemento;
- decomposição futura e abstração inicial são distinguidas sem pedir decomposição ou modelo completos;
- execução e responsabilidade sociotécnica foram separadas;
- automação de reembolsos é criticada sem formular o problema ou propor solução;
- dados com atualizações diferentes mostram limites de uma mesma regra;
- um caso limítrofe e uma solução com quatro pilares, mas ainda inadequada, substituem duplicações anteriores.

As perguntas de recuperação caíram para seis e as de reflexão para três. Critérios de domínio continuam observáveis e alinhados a reconhecimento, explicação, comparação justificada e aplicação guiada.

## Prática reorganizada

Os quatro domínios e todas as versões A, B e C foram preservados. As quatro matrizes repetidas foram substituídas por:

1. um mapa rápido das 12 descrições, com classificação e evidência decisiva;
2. análise aprofundada de 1B, 2C, 3B e 4C, separando evidência, inferência, escolha e informação capaz de mudar a escolha;
3. uma lente específica por domínio: comparação no estoque, rastreabilidade e limites no benefício, classificações alternativas no atendimento e fronteira sem computador na atividade cotidiana;
4. contraexemplo autoral, inventário de fatos/lacunas/perguntas e duas revisões após a consulta.

A solução posterior à tentativa contém um mapa compacto, um único modelo completo, três comentários de casos limítrofes, critérios para as quatro lentes e rubrica. Ela não fornece redações prontas para o contraexemplo ou para o inventário e aceita classificações alternativas justificadas. A parte anterior à solução possui 1.359 palavras; a solução parcial, 983.

## Verificação histórica e bibliográfica

Foram conferidos diretamente em fontes primárias, institucionais ou registros oficiais:

- *Mindstorms*, primeira edição da Basic Books de 1980, com a ocorrência da expressão na p. 182; Papert permanece como uso anterior verificado, não como inventor absoluto ou autor de uma definição contemporânea;
- Wing 2006, incluindo formulação, alcance e distinção de programação;
- o documento institucional de Wing de 17 nov. 2010, incluindo a formulação usada por Wing, Jan Cuny e Larry Snyder e a inspiração atribuída a Al Aho;
- título, ano e DOI do relatório do National Research Council;
- autoria, título, volume, páginas, ano e DOI de Shute, Sun e Asbell-Clarke;
- título, volume, número, páginas, ano e DOI de Denning;
- a citação oficial do CS2023, com Kumar et al., três editoras, ano 2023 e DOI `10.1145/3664191`.

Em `referencias-da-fase.md`, Wing 2010 passou a ser descrito como documento institucional, a entrada do CS2023 foi corrigida e Papert foi incluído na correspondência da Aula 01. Nenhuma fonte foi adicionada apenas por ornamentação.

## Métricas antes e depois

As palavras foram contadas com `Measure-Object -Word`; as linhas, com `Get-Content` em UTF-8.

| Artefato | Antes | Depois |
|---|---:|---:|
| Aula — palavras | 6.495 | 6.320 |
| Aula — linhas | 468 | 446 |
| Aula — seções de segundo nível | 31 | 24 |
| Aula — exercícios | 15 | 15 |
| Prática — palavras | 2.456 | 2.342 |
| Prática — linhas | 198 | 215 |
| Prática — situações/descrições | 4/12 | 4/12 |

O aumento de linhas da prática vem de tabelas menores e instruções separadas, enquanto o volume verbal, o preenchimento mecânico e a extensão da solução diminuíram.

## Carga recalibrada

- leitura atenta: 1 h 15 min a 1 h 40 min;
- pausas de elaboração e anotações: 40 min a 55 min;
- exercícios da aula: 1 h 45 min a 2 h 15 min;
- tentativa da prática antes da solução: 1 h 45 min a 2 h 15 min;
- consulta da solução e revisão da prática: 45 min a 1 h;
- recuperação ativa e síntese final: 30 min a 40 min.

A carga total sugerida passou de **7 h 45 min–9 h 45 min** para **6 h 40 min–8 h 45 min**. A nova estimativa é a soma explícita dos blocos, sem forçar a faixa planejada. A prática corresponde a 2 h 30 min–3 h 15 min desse total.

## Verificações finais

- o escopo contém exatamente os seis caminhos autorizados;
- os seis arquivos passam por decodificação UTF-8 estrita;
- os caminhos internos da aula, do README e do roteiro existem;
- as métricas foram recalculadas após a última revisão;
- a aula contém exatamente 15 exercícios e a prática preserva quatro situações e 12 descrições;
- aula e prática não contêm bloco de código, notação de pseudocódigo ou COBOL;
- não houve alteração na Fase 0 nem criação de outra aula da Fase 1;
- as 15 URLs presentes nos arquivos alterados foram verificadas: 11 responderam diretamente com sucesso, três DOI resolveram para os destinos registrados e a página da MIT Press foi confirmada no navegador apesar de bloquear a requisição automatizada;
- `git diff --check` não encontrou erro;
- o diff integral foi inspecionado e não há arquivo temporário;
- `main` e `origin/main` permaneciam no commit-base `afde0d85f1ec0d5763cf5401f3be431a4757a88b` antes do commit desta revisão.

## Pendências e decisão de prontidão

Não ficou pendência conceitual ou pedagógica bloqueante. A Aula 01 está pronta para anteceder o desenvolvimento da Aula 02: estabelece as fronteiras, oferece vocabulário panorâmico e termina em lacunas investigáveis, sem executar a formulação completa que pertence à próxima aula.

Nenhuma aula adicional foi criada e nenhum conteúdo da Fase 0 foi alterado.
