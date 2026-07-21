# Prompt 027 — Desenvolvimento da Aula 03 da Fase 1

## Objetivo e estado resultante

Desenvolver integralmente a **Aula 03 — Decomposição de problemas** e a **Prática 03 — Três decomposições do mesmo problema**, implementando a competência C03 em continuidade direta com a Aula 02. O trabalho deveria levar o aluno do reconhecimento guiado à produção e revisão de decomposições em caso simples, sem transformar a análise em implementação de software.

**Estado resultante:** aula e prática desenvolvidas e prontas para revisão técnica e pedagógica. Não se registra aprovação antecipada. A aula possui capítulo completo, exercícios sem gabarito exposto, recuperação ativa, síntese, glossário, critérios de domínio, fontes e carga. A prática possui oito blocos, solução comentada proporcional, revisão posterior, rubrica e estimativa por etapa.

## Escopo executado

Foram criados:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-03-decomposicao-de-problemas.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-03-decompondo-problemas.md`;
- `prompts/027-desenvolvimento-aula-03-fase-01.md`.

Foram atualizados minimamente:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`, apenas no estado da fase;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`, apenas com o estado da Aula 03;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/referencias-da-fase.md`, somente para registrar Simon, Parnas e ISO/IEC/IEEE 15288, efetivamente usados na aula.

Não foram alteradas a Fase 0, as Aulas 01 e 02, práticas anteriores, outras aulas da Fase 1, ementa, plano da fase, matriz, critérios de domínio, mapa conceitual, glossário da fase, planos de práticas ou avaliação, avaliações, consolidação, README global ou ROADMAP.

## Documentos lidos

A implementação foi precedida pela leitura integral do pedido anexado e dos seguintes documentos:

- `DIRETRIZES_DO_PROJETO.md`;
- `DIRETRIZES_EDITORIAIS.md`;
- `MANIFESTO_PEDAGOGICO.md`;
- `planejamento/criterios-de-qualidade.md`;
- `templates/TEMPLATE_AULA.md`;
- `templates/TEMPLATE_EXERCICIO.md`;
- todos os documentos de planejamento da Fase 1: `README.md`, `ementa.md`, `plano-da-fase.md`, `matriz-de-competencias.md`, `criterios-de-dominio.md`, `roteiro-de-aulas.md`, `mapa-conceitual.md`, `como-estudar.md`, `glossario-da-fase.md`, `plano-de-praticas.md`, `plano-de-avaliacao.md` e `referencias-da-fase.md`;
- Aula 01 e Prática 01 integrais;
- Aula 02 e Prática 02 revisadas, integrais;
- `prompts/026-revisao-aula-02-fase-01.md`;
- na Fase 0, as passagens pertinentes da Aula 02 sobre sistema, componentes, relações, fronteira, ambiente e interface; da Aula 05 sobre processamento; da Aula 06 sobre entrada, processamento, saída, estado e contexto; da Aula 07 sobre programa e processo em execução; e as definições correspondentes do glossário.

No roteiro, as Aulas 04, 06 e 11 foram examinadas especificamente para preservar suas fronteiras.

## Definição operacional e critérios de decomposição

A definição adotada foi:

> Decomposição de problemas é a divisão intencional de um todo formulado em partes administráveis, segundo um critério declarado, preservando as relações, dependências, restrições, responsabilidades, pontos de interação e propriedades necessárias para que o todo possa ser recomposto e avaliado.

A aula declara que a definição é operacional e não universal; que a decomposição depende de propósito; que não há resultado único ou neutro; que a atividade é iterativa; e que parte analítica não implica implementação.

Foram desenvolvidos com profundidade equivalente três critérios:

- **funcional:** contribuições ou transformações necessárias ao resultado;
- **dados e objetos de atenção:** informações, registros, documentos e itens do domínio relevantes ao problema, sem desenho técnico de dados;
- **etapas e eventos:** períodos e ocorrências relevantes, sem algoritmo, fluxo formal ou presunção linear.

Enumeração, classificação, sequenciamento, divisão de trabalho, desenho de solução e arquitetura técnica foram contrastados. Parte, subproblema, função, tarefa, etapa, evento, componente e responsabilidade receberam usos distintos.

## Hierarquia, granularidade e parada

A hierarquia foi apresentada como organização analítica em níveis, não como ordem, autoridade, importância ou árvore natural única. Partes irmãs precisam manter critério coerente; mudanças de critério podem ocorrer em nível inferior quando declaradas.

A granularidade é relativa ao propósito, à evidência e à próxima decisão. Os critérios de parada verificam se a contribuição e a fronteira são compreensíveis, se a parte pode ser investigada, se suas relações são identificáveis, se a responsabilidade analítica pode ser atribuída e se nova divisão acrescentaria valor. A aula rejeita parada automática por pessoa, duração, extensão textual ou quantidade fixa de partes e também rejeita decomposição indefinida.

## Dependências e interfaces

Relação foi definida como conexão relevante; dependência, como relação em que resultado, avaliação ou funcionamento de uma parte requer algo de outra sob alguma condição. Informação, ordem, recurso, decisão, regra e estado foram oferecidos como vocabulário inicial, não taxonomia rígida.

Ordem foi distinguida de dependência por testes contrafactuais simples. A aula também separa dependência de causalidade: setas exigem rótulos como “fornece informação”, “requer autorização”, “restringe” ou “atualiza estado”.

Interface foi retomada da Fase 0 como interação entre fronteiras. O registro inclui partes envolvidas, conteúdo que atravessa, significado ou condição preservados e consequência de falha. Ela não foi reduzida a tela nem ampliada para especificações técnicas. O mapa é tabela ou lista textual, não fluxograma, algoritmo ou teoria de grafos.

## Cobertura, sobreposição, lacunas e matemática

Cobertura é relativa ao todo, ao escopo, ao propósito e a um critério. A formalização introdutória define `W` como conjunto de aspectos relevantes e `Pᵢ ⊆ W` como escopo de cada parte. Cobertura é registrada por:

`P₁ ∪ P₂ ∪ ... ∪ Pₙ = W`

Sobreposição é registrada por:

`Pᵢ ∩ Pⱼ ≠ ∅`

Os símbolos `⊆`, `∪`, `∩`, `≠` e `∅` foram explicados. Partição estrita foi qualificada como cobertura por partes não vazias e disjuntas duas a duas. A aula afirma que decomposições sociotécnicas não precisam formar partições estritas e que partes de critérios diferentes não devem ser colocadas na mesma igualdade.

Sobreposição legítima, duplicidade problemática, lacuna e elemento transversal foram diferenciados. Privacidade e regras comuns mostram transversalidade; versões incompatíveis ou responsabilidade incerta mostram duplicidade; contribuição ou relação necessária sem cobertura mostra lacuna.

## Recomposição, propriedades do todo e revisão

Recomposição foi tratada como argumento, não reunião de listas. Ela verifica cobertura, compatibilidade de resultados, condições das dependências, restrições e proteções, propriedades do todo e questões abertas. Falha na recomposição pode exigir revisão de parte, critério, granularidade ou até da formulação do problema.

A otimização local foi mostrada por métricas de uma parte que pioram tempo total, correção ou acesso. Tempo de ponta a ponta, tratamento consistente, rastreabilidade, confidencialidade e capacidade de contestação aparecem como propriedades do conjunto. A decomposição permanece iterativa e revisável.

## Caso progressivo de estoque e Projeto Parcial 1

Foi preservada a formulação canônica da Aula 02: três produtos, dois centros, 192 de 2.400 linhas em 28 dias, Norte `84/1.400 = 6%`, Sul `108/1.000 = 10,8%`, 29 históricos incompletos, nenhuma relação causal estabelecida, meta inferior a 3% por centro durante três ciclos como candidata e proteções sobre perdas, custo, divergências e transferência para outros produtos ou centros. Estoque adicional, redistribuição, correção de registros e previsão permaneceram alternativas não avaliadas.

O mesmo todo foi decomposto por funções, objetos de atenção e etapas/eventos. O mapa rotula dependências e não usa setas causais. Saldo registrado, quantidade física e disponibilidade não foram equiparados. A recomposição conclui o marco P1 com formulação, interessados, restrições, três decomposições, mapa e questões abertas. A modelagem permanece para a Aula 04.

## Prática do benefício

A prática continua o caso de 1.000 solicitações da Prática 02 e acrescenta somente os elementos necessários à decomposição. Os oito blocos são:

1. reconstrução breve do todo;
2. decomposição funcional;
3. decomposição por dados ou objetos, sem modelo técnico;
4. decomposição por etapas ou eventos, sem algoritmo;
5. comparação das três visões;
6. mapa com pelo menos seis partes e sete dependências, incluindo condição, transversalidade e retorno;
7. recomposição com cobertura, lacuna, duplicidade, sobreposição, interface e risco local;
8. revisão posterior à solução, com duas mudanças justificadas e questão aberta.

A solução oferece uma possibilidade seletiva e admite alternativas justificadas. Não preenche mecanicamente todas as células. A rubrica possui 12 critérios e três níveis: precisa de revisão, adequado e consistente.

## Exercícios e gabarito interno

A aula contém 16 exercícios: três objetivos, cinco dissertativos e oito atividades de análise ou integração, das quais pelo menos seis usam casos. Há exercício de união e interseção, contraexemplo e revisão. O gabarito completo não aparece para o aluno.

Respostas esperadas para controle editorial:

1. **B.** Reúne todo formulado, propósito e critério, dependências e recomposição.
2. **A.** Há ordem de agenda e dependência comum da regra, não dependência necessária entre verificações.
3. **C.** Privacidade é transversal e a sobreposição pode ser legítima.
4. Deve explicar que critério dá coerência, preservação mantém relações e recomposição testa o todo; exemplo precisa mostrar o dano da ausência.
5. Deve usar um caso único e distinguir recorte, questão local, contribuição, ação e momento.
6. Pode dividir contestação em receber, verificar admissibilidade e reanalisar, com segundo nível em uma parte; a parada precisa referir a decisão atual.
7. Ordem sem dependência pode usar agendas independentes; dependência sem ordem fixa pode usar análises paralelas que consultam a mesma regra.
8. Deve ligar medida local a efeito global e a uma proteção, não apenas afirmar que há conflito.
9. Deve substituir a mistura por funções coerentes, reposicionando papel, objeto, prazo e meio.
10. Deve produzir duas listas diferentes sobre o mesmo todo e comparar seus pontos cegos.
11. Deve detalhar uma função do estoque sem alegar causa nem escolher alternativa.
12. A união é `{receber, verificar, decidir, comunicar}`; `P₁ ∩ P₂ = {verificar}`; falta `contestar`; não há partição por lacuna e interseção. Adicionar `contestar` explicitamente corrige cobertura; para partição estrita também seria necessário atribuir `verificar` a apenas uma parte.
13. Deve mostrar tarefas atribuídas, mas dependência, interface ou propriedade global perdida.
14. Deve conter seis partes, sete relações rotuladas, condição, restrição transversal e consequência da ambiguidade.
15. Deve registrar duas mudanças reais, razões e efeitos sobre cobertura ou recomposição.
16. Deve auditar lacuna, sobreposição, duplicidade e questão aberta e justificar prontidão apenas para iniciar a Aula 04.

## Fontes pesquisadas e usadas

Foram conferidos metadados e limites de atribuição em páginas oficiais, DOI e registro acadêmico. O conjunto usado foi:

- Pólya, 2ª edição de 1957, para decompor, recombinar e revisar como heurísticas;
- CS2023, DOI `10.1145/3664191`, para enquadramento curricular e progressão;
- Simon, 1962, registro JSTOR `985254`, para hierarquia, níveis e interações;
- Parnas, 1972, DOI `10.1145/361598.361623`, somente para importância do critério e insuficiência da sequência de processamento como única divisão;
- ISO/IEC/IEEE 24765:2017, para consistência terminológica;
- ISO/IEC/IEEE 15288:2023, 2ª edição, para aplicação iterativa, concorrente e recursiva.

O *INCOSE Systems Engineering Handbook*, 5ª edição, e *The Sciences of the Artificial* foram examinados, mas não incluídos: o primeiro seria redundante para as alegações efetivamente feitas; o segundo repetiria, em edição posterior, a tese de Simon e poderia antecipar design e abstração. Simon, Parnas e ISO 15288 foram adicionados às referências da fase porque passaram a sustentar material publicado.

## Métricas e carga

Métricas registradas na versão final anterior ao commit:

| Artefato | Palavras | Linhas | H2 | Subseções H3 | Exercícios/blocos | Casos | Fontes |
|---|---:|---:|---:|---:|---:|---:|---:|
| Aula 03 | 6.783 | 478 | 27 | 0 | 16 exercícios | 3 casos desenvolvidos — estoque, benefício e cobrança —, além de casos curtos | 6 |
| Prática 03 | 2.485 | 202 | 15 | 0 | 8 blocos | 1 caso progressivo | fontes herdadas da aula |

A matemática explícita inclui subconjunto, união, interseção, vazio, cobertura, sobreposição, partição estrita, percentuais e desigualdade. As métricas descrevem o artefato; não provam qualidade.

Carga da aula: leitura 1h45–2h15; recuperação 25–35 min; exercícios 1–8, 1h20–1h50; exercícios 9–16, 2h00–2h40; revisão, 30–45 min; total: **6h00–8h05**.

Carga da prática essencial: **4h05–5h20**. Com aprofundamento: **5h20–7h00**. A tabela da prática separa leitura, cada decomposição, comparação, mapa, recomposição, consulta e revisão.

Carga total aproximada: aula completa mais prática essencial, **10h05–13h25**; aula completa mais prática aprofundada, **11h20–15h05**. Recomenda-se distribuição em vários dias.

## Conteúdos reservados

- **Aula 04:** abstração, omissão controlada, teoria e construção de modelos, propósito e público de modelos, entidade, atributo e relação.
- **Aula 06:** escolha e conversão de representações, convenções, diagramas formais, fluxogramas, modelos de estado e pseudocódigo.
- **Aula 11:** unidades de software, contratos, parâmetros, pré e pós-condições, coesão, acoplamento, reutilização e composição executável.

Árvores textuais e tabelas aparecem apenas como suportes já dados. Funções são do domínio; objetos de atenção não constituem esquema de dados; interfaces são interações iniciais; mapas não são algoritmos.

## Verificações realizadas

Checklist conceitual: definição operacional, propósito, critério, vocabulário, três formas, hierarquia, granularidade, parada, dependências, ordem, interfaces, cobertura, sobreposição, lacunas, recomposição, otimização local e propriedades do todo foram cobertos.

Checklist de progressão: Aula 02 foi retomada brevemente; P1 foi concluído; Aulas 04, 06 e 11 foram preservadas; não há código, pseudocódigo, programação ou COBOL.

Checklist matemático: uniões e interseções foram recalculadas; símbolos foram explicados; partição foi qualificada; sobreposição não foi proibida; o formalismo permaneceu introdutório.

Checklist pedagógico: alternativas objetivas são plausíveis; exercícios exercem funções diferentes; a prática exige três critérios, mapa e recomposição; a solução vem depois da tentativa; carga foi somada por etapa.

Checklist de escopo e repositório concluído antes do commit: diff integral examinado; somente os seis arquivos autorizados presentes; UTF-8 válido; links e símbolos matemáticos conferidos; `git diff --check` limpo; nenhum temporário, código, pseudocódigo ou arquivo de área proibida.
