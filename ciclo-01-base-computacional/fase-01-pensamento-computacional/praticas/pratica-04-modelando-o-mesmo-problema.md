# Prática 04 — Dois modelos do mesmo problema

## Identificação e objetivo

- **Fase:** Fase 1 — Pensamento Computacional
- **Competência:** C04 — Abstrair e modelar
- **Modalidade essencial:** dois modelos, comparação, auditoria, caso crítico e revisão
- **Aprofundamento:** opcional e não necessário para avançar à Aula 05

O objetivo é produzir e comparar um modelo operacional e um gerencial do mesmo problema de estoque. Cada modelo deve declarar propósito, pergunta, público, decisão apoiada, fronteira, nível, seleções, omissões, pressupostos, limites, riscos e critérios de revisão. A qualidade será avaliada pela adequação e justificativa, não pela quantidade de células preenchidas.

## Caso e regras de uso

Use somente os fatos consolidados:

- dois centros e três produtos críticos;
- 192 linhas não atendidas entre 2.400;
- taxas de 6% e 10,8% por centro e 8% geral;
- 29 históricos incompletos;
- causas não estabelecidas;
- meta inferior a 3% ainda candidata;
- proteções de custo, perdas, divergência e transferência;
- soluções ainda não escolhidas;
- três decomposições e mapa de dependências produzidos no P1.

Você pode criar casos para testar o modelo, desde que os marque como **hipotéticos**. Não transforme hipótese em fato nem escolha solução técnica.

### Modalidades e tempo

Na **trilha essencial**, percorra os nove blocos, mas use a entrega reduzida indicada em cada um: quatro itens na auditoria, dois casos críticos e verificação matemática curta. Consulte a solução somente depois da tentativa e revise uma escolha em cada modelo. Tempo estimado: **2h45 a 3h45**.

No **aprofundamento opcional**, acrescente um modelo de auditoria ou terceiro público, relações matemáticas ampliadas, mudança de fronteira, duas revisões e análise adicional de vieses. Tempo adicional: **2h a 3h**.

## Bloco 1 — Reconstruir o todo

Em 100 a 160 palavras, registre problema, objetivo, escopo, critérios, incertezas e finalidade desta prática. Não refaça toda a formulação da Aula 02. Preserve a diferença entre fato, hipótese e solução.

Use estas perguntas de controle:

- O texto reconhece que as causas não foram estabelecidas?
- A meta inferior a 3% permanece candidata?
- As quatro proteções continuam visíveis?
- A finalidade é modelar, não decidir tecnologia?

## Bloco 2 — Definir os dois modelos

Preencha antes de escolher atributos. Se uma resposta mudar durante a prática, mantenha a versão inicial e registre a revisão no Bloco 9.

| Dimensão | Operacional | Gerencial |
|---|---|---|
| propósito |  |  |
| pergunta |  |  |
| público |  |  |
| decisão apoiada |  |  |
| fronteira |  |  |
| unidade de análise |  |  |
| nível |  |  |
| período |  |  |
| limite principal |  |  |

Verifique se a pergunta operacional exige ocorrência individual e se a gerencial exige população ou agrupamento. Não presuma que o público gerencial deseja sempre menos detalhe; declare sua responsabilidade concreta.

## Bloco 3 — Modelo operacional

Escolha de seis a oito objetos ou elementos. Para cada um, registre atributos essenciais, relações, evidências e motivo. Inclua ocorrências individuais, exceções, condições relevantes, omissões e pressupostos. Diferencie atividade, registro e resultado quando palavras como análise ou decisão aparecerem. Não crie fluxo ou sequência de execução.

| Objeto ou elemento | Atributos ou condições | Relações necessárias | Evidência | Motivo |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

Depois, responda:

1. Que ocorrência deve permanecer identificável?
2. Como “posição registrada” difere de condição física?
3. Como os 29 históricos incompletos aparecem sem serem tratados como ausência de movimento?
4. Que relação ajuda a preservar responsabilidade por uma decisão?
5. Quais três aspectos foram omitidos deliberadamente e por quê?
6. Que pressuposto, se falso, inviabiliza a investigação?

## Bloco 4 — Modelo gerencial

Escolha de quatro a seis indicadores ou dimensões. Para cada um, declare definição, população, período, agrupamento, proteção, limite e possibilidade de desagregação. Não desenhe dashboard.

| Indicador ou dimensão | Definição e população | Período e agrupamento | Proteção | Limite | Desagregação |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

Inclua as taxas conhecidas sem inferir causas. Explique como a meta candidata será apresentada sem virar decisão confirmada. Preserve custo, perdas, divergência e transferência como proteções. Indique que definição precisa ser comum para comparar centros.

## Bloco 5 — Comparação e rastreabilidade

Compare o que aparece e desaparece, as decisões apoiadas e não apoiadas e o caminho entre agregado e ocorrência.

| Critério | Operacional | Gerencial | Conexão necessária |
|---|---|---|---|
| unidade |  |  |  |
| aspectos visíveis |  |  |  |
| aspectos perdidos |  |  |  |
| decisão apoiada |  |  |  |
| decisão não apoiada |  |  |  |
| risco principal |  |  |  |
| evidência |  |  |  |
| condição de revisão |  |  |  |

Explique em 120 a 180 palavras:

- como um indicador retorna às ocorrências que o compõem;
- como uma exceção operacional chega ao nível gerencial;
- por que os modelos podem ser simultaneamente adequados;
- por que nenhum deve substituir o outro.

## Bloco 6 — Auditoria de omissões

Na trilha essencial, classifique quatro itens obrigatórios: conteúdo dos históricos incompletos, ocorrência individual na visão gerencial, definição de disponibilidade e uma proteção entre custo, perdas, divergência ou transferência. No aprofundamento opcional, complete pelo menos oito itens. Use: **incluído**, **omitido deliberadamente**, **desconhecido**, **fora da fronteira**, **adiado**, **agregado** ou **omitido indevidamente**.

| Item | Modelo | Classificação | Justificativa | Risco | Condição de revisão |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

Para completar oito itens no aprofundamento, acrescente produtos fora dos três críticos, taxa geral na visão operacional, condição física e uma categoria escolhida por você.

Se algo for desconhecido, não invente valor. Se estiver fora da fronteira, explique por que ainda pode motivar revisão. Se estiver agregado, declare como desagregar.

## Bloco 7 — Casos de teste conceitual

Os seis casos abaixo são **hipotéticos**. Eles não acrescentam fatos ao projeto. Na trilha essencial, analise “ocorrência grave em grupo pequeno” e escolha um entre “definição divergente entre centros” e “taxa reduzida pela exclusão de casos”. Os demais pertencem ao aprofundamento opcional. Para cada caso realizado, indique qual modelo revela, qual pode esconder, que risco surge e qual revisão é necessária.

| Caso hipotético | Modelo que revela | Modelo que pode esconder | Risco | Revisão |
|---|---|---|---|---|
| ocorrência grave em grupo pequeno |  |  |  |  |
| histórico incompleto |  |  |  |  |
| definição divergente entre centros |  |  |  |  |
| melhora geral com piora em um produto |  |  |  |  |
| taxa reduzida pela exclusão de casos |  |  |  |  |
| meta atingida com perdas maiores |  |  |  |  |

Não basta dizer “o operacional mostra detalhe”. Nomeie o atributo, proteção ou ligação ausente. Explique também quando o modelo que normalmente revela o caso ainda falharia.

## Bloco 8 — Matemática introdutória

Na trilha essencial, verifique uma seleção `S ⊆ U`, identifique uma relação que não estabelece causa e explique por que ocorrências sem centro identificado devem permanecer visíveis. A construção completa abaixo é aprofundamento opcional:

1. Defina um conjunto `U` com oito aspectos possíveis e um conjunto selecionado `S ⊆ U`; justifique duas exclusões.
2. Com `P = {P1, P2, P3}` e `C = {A, B}`, escreva `R ⊆ P × C`. A relação representa associação, não causa, e produto relacionado a vários centros não define função de `P` para `C`.
3. Seja `O` o conjunto de ocorrências e `O_identificadas ⊆ O` o subconjunto com centro conhecido. Proponha `f: O_identificadas → C`, explicando a saída única por entrada.
4. Registre `O \ O_identificadas` como ocorrências não classificadas ou pendentes, com quantidade e motivo. Explique por que resultados do subconjunto não se estendem silenciosamente a `O`.
5. Declare domínio, codomínio, domínio de validade e o efeito de dados incompletos. Como alternativa controlada, avalie `f: O → C ∪ {não identificado}`, esclarecendo que a categoria não é um centro real. Não faça prova formal.

## Bloco 9 — Revisão

Consulte a solução comentada somente depois de concluir os blocos anteriores. Em seguida, revise pelo menos uma escolha em cada modelo.

| Modelo | Escolha inicial | Escolha revista | Evidência ou risco | Efeito sobre utilidade | Efeito sobre limite |
|---|---|---|---|---|---|
| operacional |  |  |  |  |  |
| gerencial |  |  |  |  |  |

Uma revisão válida pode alterar pergunta, fronteira, atributo, definição, nível, ligação de rastreabilidade ou proteção. “Fiz igual ao exemplo” não é justificativa. Explique o que a comparação revelou.

## Entrega esperada

Entregue:

- reconstrução breve do todo;
- dois modelos completos;
- quadro comparativo e explicação de rastreabilidade;
- auditoria dos quatro itens essenciais;
- análise de dois casos hipotéticos essenciais;
- verificação matemática curta;
- uma revisão em cada modelo;
- autoavaliação pela rubrica.

No aprofundamento opcional, complete oito itens de auditoria, os seis casos e a matemática formalizada; acrescente, se desejar, terceiro modelo, mudança de fronteira ou segunda rodada de revisões.

## Solução comentada — consulte somente depois da tentativa

Não existe uma única seleção correta. As possibilidades abaixo demonstram critérios e deixam células abertas para preservar sua autoria.

### Reconstrução possível

Há 192 linhas não atendidas entre 2.400, em dois centros e três produtos, com taxas de 6%, 10,8% e 8%. Os 29 históricos incompletos e as causas permanecem desconhecidos; a meta inferior a 3% é candidata, sob proteções de custo, perdas, divergência e transferência. A prática não escolhe solução: organiza recortes para investigar ocorrências e acompanhar magnitude.

### Seleções possíveis

No operacional, linha, produto, centro, momento, posição, movimento, condição, separação, decisão, evidência e ação posterior são candidatos. Podem ser objetos, atributos, atividades, registros ou resultados conforme perspectiva explícita.

No gerencial, taxas, produto/ciclo, históricos incompletos e proteções podem compor o modelo. “Tendência” exige ciclos comparáveis; sem eles, registre dimensão planejada, não direção inventada.

Uma comparação possível:

| Aspecto | Operacional | Gerencial |
|---|---|---|
| unidade | linha não atendida | população e grupo |
| força | evidência individual | visão de magnitude |
| perda | contexto global | trajetória individual |
| limite | não prova tendência | não prova causa |

### Omissões e caso crítico

Os históricos incompletos são **desconhecidos**, não omitidos. Produtos fora dos três críticos estão **fora da fronteira**, que pode ser revista. Ocorrências ficam **agregadas** no gerencial e exigem caminho de desagregação.

Uma ocorrência de pequeno grupo e grande perda pode aparecer no operacional e sumir na taxa. A revisão gerencial protege impacto ou sinaliza exceção; a operacional define sua comunicação.

Definições divergentes impedem comparação direta apesar de cálculos corretos. Declare-as, verifique equivalência e limite a comparação ou apresente resultados separados.

### Matemática possível

Se `U = {produto, centro, momento, posição, movimento, condição, custo, decisão}` e `S = {produto, centro, momento, custo}`, então `S ⊆ U`. A relação produto–centro pode incluir `(P1, A)`, `(P1, B)` e outros pares observados. Ela não é necessariamente função de produto para centro porque um produto pode relacionar-se a ambos.

Uma função ocorrência–centro pode usar `f: O_identificadas → C`, com `O_identificadas ⊆ O`, se cada ocorrência do domínio recebe exatamente um centro. A escolha restringe o domínio: `O \ O_identificadas` precisa permanecer como conjunto explícito de ocorrências não classificadas ou pendentes, com quantidade e motivo. Conclusões sobre `O_identificadas` não se estendem automaticamente a toda a população `O`. Como alternativa, `f: O → C ∪ {não identificado}` preserva todos os casos, desde que a categoria represente qualidade do dado e não um centro real. A função não afirma causa nem execução computacional.

### Revisões possíveis

Separar “sem movimento” de “histórico incompleto” evita concluir ausência. Exibir incompletude, permitir desagregação, incluir impacto ou rever fronteira são revisões possíveis, justificadas por propósito e risco.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| propósito | genérico ou ausente | finalidade clara | orienta todas as escolhas |
| pergunta | não pode ser respondida | corresponde ao modelo | delimita conclusões |
| público | rótulo estereotipado | responsabilidade declarada | afetados também são considerados |
| fronteira | implícita | recorte declarado | fora do recorte motiva revisão |
| nível | mistura sem motivo | agregado ou detalhado coerente | passagem entre níveis é controlada |
| relevância | inclui por disponibilidade | seleciona pelo propósito | justifica inclusões e exclusões |
| omissões | apagadas | classificadas | têm motivo, risco e revisão |
| coerência | elementos se contradizem | relações fazem sentido | pressupostos são explícitos |
| rastreabilidade | agregado sem origem | permite retorno | exceção alcança decisão |
| domínio de validade | universaliza | declara situação válida | impede uso indevido |
| risco | só técnico ou ausente | identifica perda principal | considera pessoas e proteções |
| caso crítico | tratado como ruído | força avaliação | provoca revisão proporcional |
| comparação | escolhe “melhor” absoluto | reconhece propósitos | compara perdas e usos vedados |
| revisão | copia comentário | muda por evidência | registra efeito e limite |

Considere o essencial concluído quando nenhum critério estiver em “precisa de revisão” e você conseguir explicar, sem ler, por que os dois modelos são úteis, o que cada um perde e qual evidência o faria mudar.

## Carga integrada

Aula e anotações demandam cerca de **2h a 2h30**; recuperação ativa, **20 a 30 min**; exercícios essenciais, **1h30 a 2h**; prática essencial, **2h45 a 3h45**; consulta da solução, revisão e autoavaliação, **30 a 45 min**. A trilha essencial completa fica em aproximadamente **7h05 a 9h30**.

Exercícios adicionais, auditoria de oito itens, seis casos, matemática completa e eventual terceiro modelo elevam a carga completa para cerca de **10h30 a 14h**. O aprofundamento é opcional e não condiciona o avanço à Aula 05.
