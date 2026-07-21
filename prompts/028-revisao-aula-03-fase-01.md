# Prompt 028 — Revisão da Aula 03 da Fase 1

## Objetivo e estado resultante

Realizar revisão técnica, pedagógica e editorial localizada da **Aula 03 — Decomposição de problemas** e da **Prática 03 — Três decomposições do mesmo problema**, cujo núcleo conceitual já estava aprovado. A revisão deveria reduzir fragmentação estrutural, corrigir ambiguidades terminológicas, tornar as questões objetivas mais discriminativas e separar de fato o núcleo essencial do aprofundamento, sem reescrever integralmente a aula nem acrescentar conteúdo de preenchimento.

**Estado resultante:** aula e prática revisadas técnica e pedagogicamente. O núcleo conceitual foi preservado; a navegação foi reorganizada; terminologia, interface e matemática foram refinadas; exercícios e prática receberam rotas essencial e opcional; a carga essencial foi reduzida; e o material está pronto para a Aula 04 sem exigir o aprofundamento.

## Escopo executado

Foram atualizados:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-03-decomposicao-de-problemas.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-03-decompondo-problemas.md`.

Foi criado:

- `prompts/028-revisao-aula-03-fase-01.md`.

Foram atualizados minimamente, apenas para refletir o novo estado e a terminologia revisada:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`.

`referencias-da-fase.md` foi auditado e não foi alterado, pois não se comprovou erro bibliográfico. Permaneceram intocados Fase 0, Aulas e Práticas 01 e 02, demais aulas da Fase 1, ementa, plano da fase, matriz de competências, critérios de domínio, mapa conceitual, glossário da fase, planos de práticas e avaliação, README global e ROADMAP.

## Leitura obrigatória realizada

Foram lidos integralmente o pedido anexado, Aula 03, Prática 03, Prompt 027, Aula 02 revisada, Prática 02 revisada, roteiro pertinente às Aulas 03 e 04, matriz de competências, critérios de domínio, plano de práticas, referências da fase, `DIRETRIZES_EDITORIAIS.md` e `planejamento/criterios-de-qualidade.md`.

A continuidade foi conferida especialmente contra C03 e C04: C03 exige decompor e recompor com dependências preservadas; C04 inicia seleção e omissão controlada de detalhes, modelos e justificativa de fronteira. A revisão mantém essa fronteira.

## Diagnóstico e acertos preservados

O veredito foi **revisão localizada, não reconstrução**. A versão anterior já apresentava profundidade conceitual, exemplos progressivos e limites adequados. Foram preservados:

- definição operacional orientada por todo, propósito, critério, partes administráveis, preservação e recomposição;
- distinção entre decomposição, enumeração, classificação, sequenciamento, divisão de trabalho, solução e arquitetura;
- três formas principais: funcional, por informações e objetos do domínio e por etapas ou eventos;
- hierarquia, níveis, granularidade e critérios de parada;
- relação, dependência, ordem, compartilhamento, influência, restrição transversal e diferença para causalidade;
- interfaces analíticas, cobertura, sobreposição, duplicidade, lacunas e elementos transversais;
- recomposição, otimização local, propriedades do todo e revisão iterativa;
- caso progressivo de estoque, mapa de dependências e encerramento do P1;
- ausência de código, pseudocódigo, programação, COBOL, desenho técnico de dados e modelagem da Aula 04;
- mini glossário com 27 termos;
- seis fontes com função declarada, sem referência decorativa.

Os problemas principais eram estruturais e calibrativos: 27 H2 sem H3 fragmentavam uma sequência conceitualmente contínua; “dados e objetos de atenção” misturava objeto, informação, registro, atividade e resultado; a definição de interface sugeria interação entre fronteiras; duas questões objetivas tinham distratores frágeis; e a prática essencial repetia quase todo o volume do aprofundamento.

## Estrutura antes e depois

Antes da revisão, a aula possuía **27 H2 e 0 H3**. Depois, possui **10 H2 e 34 H3**. A ordem argumentativa e a maior parte da prosa foram mantidas; a alteração principal foi hierárquica.

| Novo bloco H2 | Seções anteriores consolidadas como H3 | Justificativa |
|---|---|---|
| Metadados | Metadados | bloco documental independente |
| Introdução e definição | objetivo; problema; ponte; caso de abertura; definição; todo e termos próximos | todos estabelecem o todo, a necessidade e o vocabulário inicial |
| Critérios e formas de decomposição | contrastes; propósito e critério; funcional; informações e objetos; etapas e eventos; comparação | reúne as escolhas que recortam o mesmo todo |
| Estrutura das partes | hierarquia e níveis; granularidade e parada | ambos tratam profundidade e escala das partes |
| Dependências e interfaces | relações, dependências e ordem; interfaces e mapa | reúne conexões que atravessam fronteiras |
| Cobertura, sobreposição e lacunas | cobertura e matemática; sobreposição, lacunas e transversais | reúne auditoria do alcance dos escopos |
| Recomposição e validação | recomposição; otimização local, propriedades e iteração | reúne verificação do conjunto e revisão diagnóstica |
| Aplicação aos casos | estoque/P1; cobrança e atendimento | concentra aplicações sem interromper a progressão conceitual |
| Atividades, síntese e domínio | confusões; exercícios essencial e profundo; recuperação; síntese; glossário; domínio; continuidade | organiza estudo, evidência e passagem à próxima aula |
| Referências, métricas e carga | fontes; métricas; tempos | separa documentação editorial do percurso didático |

H2 passou a indicar mudança real de problema pedagógico; H3 passou a permitir consulta por aspecto relacionado. O resultado reduz a fragmentação global sem esconder títulos úteis.

## Definição e terminologia revisadas

A definição operacional preservada, com “interfaces” no lugar do rótulo menos preciso “pontos de interação”, é:

> Decomposição de problemas é a divisão intencional de um todo formulado em partes administráveis, segundo um critério declarado, preservando as relações, dependências, restrições, responsabilidades, interfaces e propriedades necessárias para que o todo possa ser recomposto e avaliado.

“Decomposição por dados e objetos de atenção” foi refinada para **decomposição por informações e objetos do domínio**. A expressão corresponde ao eixo abreviado como “dados” em C03 e não cria uma quarta forma. A aula e a prática distinguem:

- **objeto do domínio:** algo cuja identidade ou condição importa ao problema;
- **dado:** valor ou símbolo cuja interpretação depende de contexto;
- **informação:** representação com significado sobre objeto ou ocorrência;
- **registro:** evidência ou armazenamento de informação;
- **atividade:** transformação realizada no domínio;
- **resultado:** efeito ou produto da atividade.

Documento foi qualificado como artefato delimitado que contém informação registrada e que pode ser objeto do domínio quando sua identidade ou condição importa. “Análise” e “decisão” deixaram de aparecer como objetos indistintos nos exemplos centrais. Conforme o caso, aparecem como atividade de análise, conclusão ou registro da análise, ato de decidir, resultado ou registro da decisão. O mesmo cuidado foi aplicado a avaliação, autorização e comunicação. A precisão é conceitual, sem campos, chaves, tabelas, entidades, atributos ou esquema técnico.

## Interface revisada

A definição passou a ser:

> Interface é a relação ou o ponto de interação pelo qual informação, material, decisão, regra ou mudança de estado atravessa a fronteira entre partes.

O registro continua exigindo parte de origem, parte de destino, conteúdo e significado, condição e consequência da ausência ou ambiguidade. A interface permanece analítica: não é reduzida a tela e não é ampliada para API, protocolo ou contrato técnico.

## Matemática preservada e refinada

A formalização introdutória foi conferida e preserva:

- `Pᵢ ⊆ W`;
- cobertura por `P₁ ∪ P₂ ∪ ... ∪ Pₙ = W`;
- sobreposição, para `i ≠ j`, por `Pᵢ ∩ Pⱼ ≠ ∅`;
- partição estrita com cobertura, partes não vazias e disjunção duas a duas;
- diferença entre cobertura e qualidade e entre decomposição e partição.

Ficou explícito que `W` depende de escopo, propósito e um único critério declarado; alterar um deles exige rever `W`; a igualdade de cobertura não prova que `W` foi bem definido; partes funcionais, por informações e objetos e por etapas não entram na mesma igualdade; transversalidade e sobreposição podem ser legítimas; e a notação não representa sozinha dependências, interfaces ou propriedades do todo. Não foi acrescentada teoria de conjuntos além da necessária.

## Questões objetivas e gabarito interno

As questões 1 e 3 foram reescritas com alternativas que contêm elementos conceitualmente válidos, mas falham por validação apenas local, todo centrado em solução, independência presumida, responsabilidade transversal omitida ou interpretação duplicada. A questão 2 foi preservada com pequeno refinamento do distrator D.

**Gabarito interno:**

1. **B** — reúne todo formulado, propósito, critério, relações, dependências, restrições e recomposição;
2. **A** — há ordem de agenda e dependência comum da regra, não dependência necessária entre as verificações;
3. **C** — privacidade é restrição transversal com efeito, responsabilidade e coordenação explícitos em cada parte afetada.

O gabarito permanece fora da aula destinada ao aluno.

## Exercícios essenciais e aprofundamento

Os 16 exercícios foram mantidos em quantidade e separados por função:

- **Núcleo essencial, exercícios 1 a 9:** definição, dependência e ordem, transversalidade, explicação do conceito, recomposição, decomposição funcional, comparação de dois critérios com cobertura e revisão justificada;
- **Aprofundamento, exercícios 10 a 16:** distinções finas, hierarquia e parada, granularidade do estoque, formalização matemática, contraexemplo de transferência, auditoria de mapa com oito relações e retorno e auditoria opcional do P1.

O exercício de dois critérios passou a fornecer uma visão funcional inicial e pedir uma visão resumida por informações e objetos, evitando duas construções extensas. O mapa aprofundado passou de construção integral repetida para auditoria de um mapa imperfeito com sete ou mais relações. A auditoria adicional do P1 permanece opcional e não cria o modelo da Aula 04.

## Prática recalibrada

Os oito blocos conceituais foram preservados. No essencial, o aluno escolhe uma decomposição principal, a desenvolve integralmente e registra as outras duas de modo resumido; depois compara as três, constrói mapa, recompõe e revisa. No aprofundamento, desenvolve as três integralmente.

| Bloco | Percurso essencial | Aprofundamento opcional |
|---|---|---|
| 1 — todo | 120–160 palavras, duas questões abertas e critério principal provisório | até 180 palavras, quatro questões e condições de mudança do critério |
| 2 — funcional | completa se principal; quatro funções e ponto cego se alternativa | 6–8 funções, subpartes e fronteiras alternativas |
| 3 — informações e objetos | completa se principal; quatro elementos tipados se alternativa | 7–8 elementos, divergências semânticas e granularidades |
| 4 — etapas e eventos | completa se principal; 4–5 momentos e não linearidade se alternativa | quadro integral, retorno, exceção, paralelismo e duas granularidades |
| 5 — comparação | três linhas, escolha confirmada ou revista e complemento | custo analítico e risco adicional |
| 6 — mapa | ao menos 5 partes e 5 dependências, uma condicional e uma transversal | 7 ou mais partes, 8 ou mais dependências, retorno e circularidade |
| 7 — recomposição | cobertura compacta, achados centrais e 120–160 palavras | auditoria ampliada e 170–220 palavras |
| 8 — revisão | uma mudança, efeito, questão aberta e seis critérios decisivos | duas mudanças, alternativa defendida e os 12 critérios |

A solução comentada foi mantida seletiva e proporcional: não oferece quadro nem decomposição principal completa, apresenta quatro dependências representativas e admite escolhas alternativas justificadas. O percurso essencial continua avaliando os três critérios — um em profundidade e dois comparativamente —, além de dependências e recomposição.

## Carga antiga e nova

Antes da revisão:

- aula sem prática: **6h00–8h05**;
- prática essencial: **4h05–5h20**;
- prática aprofundada: **5h20–7h00**;
- total com prática essencial: **10h05–13h25**;
- total completo: **11h20–15h05**.

Depois da revisão:

- leitura: **1h45–2h15**;
- recuperação: **25–35 min**;
- exercícios essenciais: **1h40–2h10**;
- prática essencial: **3h15–4h20**;
- revisão final: **15–25 min**;
- total essencial: **7h20–9h45**;
- total completo opcional, com todos os exercícios, prática aprofundada e revisão ampliada: **11h20–15h05**.

A rota essencial cai aproximadamente 2h45–3h40 porque deixa de exigir três decomposições completas, mapa ampliado, duas revisões e rubrica integral. O percurso completo conserva a profundidade anterior e está claramente marcado como opcional.

## Fontes verificadas

Permanecem as mesmas seis fontes, cada uma com alcance delimitado:

- Pólya, 2ª edição de 1957: decompor, recombinar e revisar como heurísticas, não receita universal;
- CS2023: enquadramento curricular e progressão;
- Simon, 1962: hierarquia, níveis e interações, não árvore natural única;
- Parnas, 1972: importância do critério e insuficiência da sequência como única base, sem antecipar modularização;
- ISO/IEC/IEEE 24765:2017: apoio terminológico;
- ISO/IEC/IEEE 15288:2023, 2ª edição: aplicação iterativa e concorrente dos processos ao sistema e recursiva aos elementos, sem prescrição do método da aula.

Não foi identificado erro bibliográfico comprovado, fonte decorativa nem necessidade de alterar `referencias-da-fase.md`.

## Métricas antes e depois

| Artefato | Versão | Palavras | Linhas | H2 | H3 | Exercícios ou blocos |
|---|---|---:|---:|---:|---:|---:|
| Aula 03 | antes | 6.783 | 478 | 27 | 0 | 16 exercícios sem classificação |
| Aula 03 | depois | 7.606 | 519 | 10 | 34 | 9 essenciais e 7 de aprofundamento |
| Prática 03 | antes | 2.485 | 202 | 15 | 0 | 8 blocos pouco diferenciados por rota |
| Prática 03 | depois | 3.238 | 220 | 15 | 0 | 8 blocos com entregas distintas por rota |

O aumento textual decorre das distinções terminológicas, dos distratores plausíveis e das instruções separadas por modalidade; não adiciona novo eixo conceitual. A redução de H2 na aula é a métrica estrutural decisiva. Contagens descrevem o artefato, não provam qualidade.

## Fronteira e prontidão para a Aula 04

A revisão não introduziu entidade, atributo, relação de modelagem, seleção ou omissão controlada de detalhes, modelos por público, escolha de representação, fluxograma, pseudocódigo, código, programação ou COBOL. Função permanece função do problema; informações e objetos permanecem análise do domínio; tabelas e mapas são suportes fornecidos; interfaces permanecem relações analíticas.

O material está pronto para prosseguir: o núcleo essencial demonstra critério, duas visões, dependências, cobertura, recomposição e revisão; a prática essencial examina os três critérios e desenvolve um deles em profundidade. A auditoria adicional do P1 e os aprofundamentos podem enriquecer a aprendizagem, mas não são condição para iniciar a Aula 04.

## Verificações finais previstas

Antes do commit, devem ser confirmados: diff integral; somente os cinco arquivos autorizados; UTF-8 válido; links locais e externos; `git diff --check`; símbolos matemáticos e cálculos; 27 termos do mini glossário; 16 exercícios; oito blocos da prática; soma dos tempos; marcação inequívoca do aprofundamento como opcional; ausência de temporários, código e alterações fora do escopo. O commit deve usar exatamente `Revisa Aula 03 da Fase 1` e ser enviado a `origin/main`.
