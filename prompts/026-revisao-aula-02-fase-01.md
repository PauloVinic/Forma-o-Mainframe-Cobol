# Prompt 026 — Revisão da Aula 02 da Fase 1

## Objetivo e veredito

Realizar uma revisão técnica, pedagógica e editorial localizada da **Aula 02 — O que é um problema** e da **Prática 02 — De situações vagas a problemas verificáveis**, sem reescrever a aula, ampliar seu programa ou antecipar a Aula 03.

**Veredito após a revisão:** material aprovado para continuidade. A definição operacional, a progressão C01/C02, os casos, a matemática contextual e a fronteira curricular já eram consistentes. Os problemas encontrados eram localizados: o binário “causa confirmada”, o tratamento de testemunho como categoria paralela à evidência, alternativas objetivas pouco equilibradas, uso excessivamente mecânico do quadro didático e subestimação da duração da prática. Esses pontos foram corrigidos sem alterar a arquitetura da aula.

## Escopo executado

Foram atualizados:

- `ciclo-01-base-computacional/fase-01-pensamento-computacional/aulas/aula-02-o-que-e-um-problema.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/praticas/pratica-02-formulando-problemas.md`;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/README.md`, somente no estado da Aula 02;
- `ciclo-01-base-computacional/fase-01-pensamento-computacional/roteiro-de-aulas.md`, somente no estado da Aula 02.

Este arquivo foi criado como registro da revisão. Não foram alterados Fase 0, Aula 01, outras aulas, matriz de competências, critérios de domínio, ementa, plano da fase, glossário da fase, mapa conceitual, planos de práticas ou avaliação, README global ou ROADMAP. `referencias-da-fase.md` foi conferido e permaneceu intacto porque não foi demonstrado erro bibliográfico.

O Prompt 025 permanece como registro histórico. Suas expressões “sem causa confirmada”, “testemunho” como categoria paralela e o gabarito anterior da Questão 1 foram superados por esta revisão, mas não foram alterados retroativamente.

## Pontos fortes preservados

A revisão manteve:

- a definição operacional ampla de problema, declarada como convenção pedagógica não universal;
- problema como objeto delimitado e revisável, sem exigir falha já observada;
- diferença entre situação, necessidade, problema e solução;
- pergunta, decisão, risco e oportunidade como enquadramentos distintos e combináveis;
- separação entre sintoma, contribuição causal e hipótese causal em contextos sociotécnicos de causalidade múltipla;
- distinção entre evidência, fato do caso, inferência, hipótese e decisão;
- interessados, pessoas afetadas e responsabilidade decisória;
- objetivo, estados atual e desejado, saída e resultado esperado;
- escopo, exclusões e fronteira;
- restrição, recurso, preferência e pressuposto;
- métricas, metas, linhas de base, critérios de sucesso e critérios de proteção;
- questões em aberto, revisabilidade e proporcionalidade da formulação;
- matemática incorporada ao contexto, sem transformar símbolos em sinal automático de qualidade;
- 15 exercícios com funções distintas e os quatro blocos da prática;
- reserva de decomposição, dependências, interfaces e recomposição para a Aula 03;
- ausência de código, pseudocódigo, COBOL ou JCL.

## Revisão da linguagem causal

“Causa confirmada” foi substituída seletivamente por expressões que declaram apoio, recorte e finalidade:

- **contribuição causal sustentada no recorte**;
- **alegação causal sustentada pelas evidências disponíveis**;
- fator causal suficientemente sustentado para determinada decisão;
- **relação causal não estabelecida**;
- hipótese fortalecida ou enfraquecida por novas observações.

A aula agora explicita que apoio causal é situado e revisável; não implica causa única, suficiente ou necessária; correlação não estabelece causação; condições técnicas e organizacionais podem contribuir em conjunto; e uma decisão provisória ou protetiva pode ser necessária antes que todas as relações causais estejam estabelecidas. A decisão deve registrar evidência, limites, incerteza e condições de revisão, em vez de simular certeza.

O caso progressivo passou a informar que nenhuma relação causal foi estabelecida no recorte. A prática guiada trata a promessa de que inteligência artificial resolverá o caso como alegação não sustentada. A recuperação ativa e o mini glossário também foram alinhados ao contínuo entre hipótese, relação não estabelecida e contribuição sustentada.

## Evidência, fato do caso, relato e testemunho

Relato ou testemunho agora aparece como **possível fonte de evidência** ou registro de experiência e percepção. Não é categoria epistemológica paralela à evidência, não transforma automaticamente seu conteúdo em fato e não prova causalidade.

O exemplo central foi tornado explícito: se uma solicitante declara ter enviado o documento duas vezes, há apoio para afirmar que o relato ocorreu. Isso não demonstra que o sistema recebeu ou armazenou ambos os envios; protocolos, logs ou registros de transação seriam necessários para essa conclusão.

Na Prática 02:

- a orientação manda identificar o material que funciona como evidência e classificar afirmações por seu estatuto;
- o registro técnico “marca”, em vez de “confirma”, a indisponibilidade;
- a tabela do Bloco 2 separa estatuto, base e alcance e informação faltante;
- o comentário distingue a alegação do analista, o relato da solicitante, o fato do caso sobre o registro e o impacto causal ainda não demonstrado;
- a rubrica usa “fato do caso e hipótese”.

## Modelo didático e critério de suficiência

O quadro de sete blocos continua como conjunto de perguntas, não como formulário universal. A revisão acrescenta que:

- campos podem permanecer em aberto;
- a importância relativa dos campos varia conforme o caso;
- a profundidade depende da próxima decisão;
- uma formulação mínima suficiente pode ser melhor que uma versão artificialmente completa;
- a tabela organiza perguntas, mas não substitui investigação;
- preencher células não demonstra domínio.

O critério editorial e pedagógico adotado ficou explícito na aula: **“A formulação deve conter informação suficiente para orientar a próxima decisão sem ocultar incertezas relevantes.”**

## Exercícios da aula

Foram mantidos os 15 exercícios, sem adicionar tarefas. As questões 4 a 8 permanecem no Nível 2; as questões 9 a 13, no Nível 3 guiado; e as questões 14 e 15 chegam à aplicação autônoma inicial em caso simples. A Questão 8 não pede algoritmo; a Questão 12 não pede decomposição; a Questão 13 avalia fronteiras e contexto; a Questão 15 não exige requisito, interface, procedimento ou especificação completa.

A Questão 12 passou a usar os sete blocos como perguntas de apoio, admitir lacunas e itens não aplicáveis justificados e vedar preenchimento artificial.

As três objetivas foram reequilibradas. Todas as alternativas contêm elementos plausíveis; a resposta correta exige a combinação completa, não uma pista lexical.

### Gabarito interno das objetivas

1. **d** — delimita canal, população e período, declara o objetivo de reduzir a discrepância, prevê validação de critérios e proteções e mantém causas e intervenções em aberto. A alternativa a mede espera, mas não delimita população nem meta aceitável; b trata perguntas repetidas como explicação causal; c formula a discrepância, porém impõe chatbot como restrição.
2. **a** — a afirmação numérica é fato do caso sustentado pelo relatório e limitado ao período; reprocessamento é hipótese causal; suspensão é decisão provisória. O relatório é fonte de evidência, não substitui o estatuto da afirmação que sustenta, e a decisão não comprova causa.
3. **c** — alinha objetivo, população, linha de base, método comparável, meta e proteção. Todas as alternativas possuem período, número e métrica aparente; a mede automação, b compara populações diferentes e d usa contagem em população selecionada com volume variável.

As respostas esperadas foram registradas somente neste Prompt 026; a aula preserva a exigência de justificativa sem destacar gabarito.

## Revisão da prática

Os quatro blocos preservam funções distintas:

1. estoque — formulação guiada proporcional;
2. benefício — análise do estatuto das afirmações e de alegações causais;
3. atendimento — conflitos, afetados ausentes, critérios e autoridade;
4. reembolsos — crítica de solução prematura, reformulação e contraexemplo.

No Bloco 1, a antiga ficha de 18 linhas e duas colunas de resposta produzia 36 células, além da declaração. Os mesmos conceitos foram agrupados em nove respostas essenciais: evidências; hipóteses; interessados, afetados e autoridade; estados e objetivo; escopo e exclusões; restrições e pressupostos; critérios e proteções; questões em aberto; soluções separadas. Inferências, recursos, entradas e resultados permanecem como aprofundamento: o percurso essencial escolhe dois dos quatro e o percurso com aprofundamento realiza todos. “Não informado” e “não aplicável” são aceitos com justificativa. A declaração foi reduzida de 140–200 para 100–150 palavras.

No Bloco 2, relato deixou de ser categoria paralela, a tabela foi reduzida de quatro dimensões de resposta para três e hipóteses concorrentes devem indicar evidências capazes de fortalecê-las ou enfraquecê-las.

No Bloco 3, o aluno pode indicar papel decisório plausível ou declarar que a autoridade não foi informada. Deve apontar norma, delegação, atribuição, organograma ou instância de governança a consultar; não precisa inventar autoridade real. A solução explicita que a proposta da gestão não demonstra autoridade formal.

No Bloco 4, não se repete a ficha do Bloco 1. O percurso essencial pede três questões prioritárias, reescrita de 90–130 palavras centrada em discrepância, recorte ou prioridade e incerteza relevante, além de critério principal, duas proteções e contraexemplo. O aprofundamento permite mais duas questões.

## Carga horária antes e depois

A estimativa anterior de 3–4 horas fechava aritmeticamente, mas era otimista: incluía 36 células no Bloco 1, até 28 análises no Bloco 2 e entregas compostas nos Blocos 3 e 4.

| Medida | Antes | Depois |
|---|---:|---:|
| Prática 02 | 3–4h | 3h30–4h30, percurso essencial |
| Prática 02 com aprofundamento | não distinguida | 4h30–5h30 |
| Carga total da Aula 02 | 6h40–8h40 | 7h10–9h10, percurso essencial |
| Carga total com aprofundamento | não distinguida | 8h10–10h10 |

Os componentes externos à prática somam 3h40–4h40. O percurso essencial da prática soma 210–270 minutos; o aprofundamento, 270–330 minutos. As faixas publicadas resultam diretamente dessas somas e não foram forçadas para caber em três horas.

## Verificação matemática

Não houve expansão matemática. Foram conferidos:

- `N > 0` antes de `r = n/N`;
- `84/1.400 = 6%`, `108/1.000 = 10,8%` e `192/2.400 = 8%`;
- `380/1.000 = 38%` e `95/500 = 19%` nos casos correspondentes;
- diferença entre `<` e `≤` e entre intervalos inclusivos e exclusivos;
- `r = 2%` satisfaz `r ≤ 2%`;
- `t = 5` pertence a `[0, 5]`, mas não satisfaz `t < 5`;
- pertencimento `d ∈ D` sem inferir que todos os documentos são sempre exigidos;
- linha de base e meta comparáveis somente com população, evento, período, unidade e método compatíveis;
- presença de população, período, unidade e forma de observação nos critérios relevantes.

Os símbolos continuam apresentados como meios de tornar fronteiras legíveis, não como prova de boa formulação.

## Métricas antes e depois

As palavras foram contadas com `Measure-Object -Word`; linhas são linhas físicas do arquivo.

| Artefato | Antes | Depois |
|---|---:|---:|
| Aula 02 — palavras | 6.638 | 6.625 |
| Aula 02 — linhas | 371 | 372 |
| Aula 02 — estrutura | 25 H2; 8 H3; 3 H4 | 25 H2; 8 H3; 3 H4 |
| Aula 02 — exercícios | 15 | 15 |
| Aula 02 — tabelas | 4 | 4 |
| Aula 02 — fontes | 7 | 7 |
| Prática 02 — palavras | 2.585 | 2.581 |
| Prática 02 — linhas | 205 | 210 |
| Prática 02 — estrutura | 14 H2; 3 H3 | 14 H2; 3 H3 |
| Prática 02 — tabelas | 5 | 7 |
| Prática antes da solução | 1.603 palavras | 1.539 palavras |
| Solução e autocorreção | 982 palavras | 1.042 palavras |

As duas novas tabelas líquidas resultam da separação entre respostas essenciais e aprofundamento e da explicitação auditável dos tempos; a quantidade de células obrigatórias caiu.

## Fontes verificadas

As sete fontes existentes foram mantidas porque sustentam decisões específicas:

1. Pólya, *How to Solve It*, 2. ed., 1957 — perguntas sobre incógnita, dados, condições e revisão, sem transformar a heurística em sequência universal.
2. Kumar et al., *Computer Science Curricula 2023* — progressão por competências, formulação e ambiguidade; título, autoria institucional, ano de citação e DOI `10.1145/3664191` conferidos no relatório oficial.
3. ISO/IEC/IEEE 24765:2017 — título e edição do vocabulário de engenharia de sistemas e software conferidos no catálogo ISO.
4. ISO/IEC/IEEE 29148:2018 — título, segunda edição e situação da norma conferidos no catálogo ISO; usada apenas na fronteira com requisitos e especificação.
5. SWEBOK Guide 4.0a — versão de setembro de 2025 conferida na IEEE Computer Society; usada para situar engenharia de requisitos como campo iterativo.
6. Simon, “The Structure of Ill Structured Problems”, *Artificial Intelligence*, v. 4, p. 181–201, 1973, DOI `10.1016/0004-3702(73)90011-8` — usado somente para problemas pouco estruturados e graus de indefinição.
7. Rosen, *Discrete Mathematics and Its Applications*, 8. ed., 2019 — desigualdades, intervalos, conjuntos e pertencimento.

Não foi atribuída a Simon fundamentação para causalidade, formulação geral ou engenharia de requisitos. Nenhuma fonte decorativa foi adicionada.

## Prontidão para a Aula 03

A Aula 02 revisada entrega um problema como todo delimitado, rastreável, proporcional e revisável. Não antecipa decomposição funcional, por dados ou etapas; níveis, responsabilidades, dependências, ordem, interfaces, granularidade, parada, duplicidades, lacunas, incompatibilidades ou recomposição. Está pronta para preceder o **desenvolvimento integral da Aula 03 — Decomposição de problemas**.

## Verificações finais

- UTF-8 estrito, ausência de espaços finais e `git diff --check` aprovados;
- limites de 6.000–6.700 palavras na aula e 2.200–2.600 na prática confirmados;
- 15 exercícios, quatro blocos, ausência de código e integridade das tabelas confirmados;
- diff integral revisado, com exatamente os cinco caminhos autorizados;
- entrega preparada para o commit exato `Revisa Aula 02 da Fase 1` e envio de `main` para `origin/main`.
