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

Na **trilha essencial**, realize todos os nove blocos, consulte a solução somente depois da tentativa e revise uma escolha em cada modelo. Tempo estimado: **3h15 a 4h20**.

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

Escolha de seis a oito objetos ou elementos. Para cada um, registre atributos essenciais, relações, evidências e motivo. Inclua ocorrências individuais, exceções, condições relevantes, omissões e pressupostos. Não crie fluxo ou sequência de execução.

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

Classifique pelo menos oito itens. Use: **incluído**, **omitido deliberadamente**, **desconhecido**, **fora da fronteira**, **adiado**, **agregado** ou **omitido indevidamente**.

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

Inclua obrigatoriamente: conteúdo dos 29 históricos incompletos; produtos fora dos três críticos; ocorrência individual na visão gerencial; taxa geral na visão operacional; definição de disponibilidade; custo; condição física; e uma categoria escolhida por você.

Se algo for desconhecido, não invente valor. Se estiver fora da fronteira, explique por que ainda pode motivar revisão. Se estiver agregado, declare como desagregar.

## Bloco 7 — Casos de teste conceitual

Os seis casos abaixo são **hipotéticos**. Eles não acrescentam fatos ao projeto. Para cada um, indique qual modelo revela, qual pode esconder, que risco surge e qual revisão é necessária.

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

1. Defina um conjunto `U` com oito aspectos possíveis dentro de sua fronteira e um conjunto `S` com os aspectos selecionados por um modelo. Registre `S ⊆ U` e justifique duas exclusões.
2. Considere produtos `P = {P1, P2, P3}` e centros `C = {A, B}`. Escreva uma relação `R ⊆ P × C` com pares pertinentes ao seu modelo. A relação precisa representar associação, não causa.
3. Proponha uma função `f: O → C`, em que `O` é um conjunto de ocorrências admissíveis. Explique por que cada ocorrência recebe exatamente um centro no modelo.
4. Dê exemplo de relação que não seja função, como produto associado a mais de um centro ou solicitação associada a vários documentos.
5. Declare domínio, codomínio, dados que podem impedir a aplicação e domínio de validade. Não faça prova formal.

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
- auditoria de ao menos oito itens;
- análise dos seis casos hipotéticos;
- atividade matemática;
- uma revisão em cada modelo;
- autoavaliação pela rubrica.

No aprofundamento opcional, acrescente somente o que escolheu: terceiro modelo, matemática ampliada, mudança de fronteira ou segunda rodada de revisões.

## Solução comentada — consulte somente depois da tentativa

Não existe uma única seleção correta. As possibilidades abaixo demonstram critérios e deixam células abertas para preservar sua autoria.

### Reconstrução possível

O problema envolve 192 linhas não atendidas entre 2.400, em dois centros e três produtos críticos. As taxas conhecidas são 6%, 10,8% e 8% no conjunto, mas 29 históricos estão incompletos e as causas não foram estabelecidas. O objetivo anterior é reduzir ocorrências sob critérios ainda em validação; a meta inferior a 3% continua candidata. Custo, perdas, divergência e transferência precisam ser protegidos. Esta prática não escolhe solução: organiza dois recortes do mesmo caso para investigar ocorrências e acompanhar magnitude, tornando seleções, omissões e limites examináveis.

### Seleções possíveis

No operacional, linha, produto, centro, momento, posição registrada, movimento, condição física, separação, decisão, evidência e ação posterior são candidatos. Não é obrigatório tratá-los como dez objetos: alguns podem ser atributos ou condições, desde que o significado e as relações permaneçam claros.

No gerencial, taxa geral, taxa por centro, dimensão produto/ciclo, históricos incompletos e proteções de custo, perdas, divergência e transferência podem compor o modelo. “Tendência” exige mais de um ciclo comparável; se essa evidência não estiver fornecida, registre a dimensão planejada, não invente direção.

Uma comparação possível:

| Aspecto | Operacional | Gerencial |
|---|---|---|
| unidade | linha não atendida | população e grupo |
| força | evidência individual | visão de magnitude |
| perda | contexto global | trajetória individual |
| limite | não prova tendência | não prova causa |

### Omissões e caso crítico

Os 29 históricos incompletos são **desconhecidos**, não omitidos deliberadamente. Produtos fora dos três críticos estão **fora da fronteira** declarada, mas podem exigir ampliação se houver deslocamento do problema. Ocorrências individuais ficam **agregadas** na visão gerencial; o controle adequado é manter caminho de desagregação.

Considere o caso hipotético de uma ocorrência de pequeno grupo e grande perda. O operacional pode revelá-la por identificação e impacto; a taxa geral pode escondê-la. A revisão gerencial inclui proteção de impacto ou sinal de exceção, sem transformar todo detalhe em indicador principal. A revisão operacional define como comunicar a exceção.

Definições divergentes entre centros impedem comparação direta, mesmo que os cálculos estejam corretos. Uma solução plausível é declarar cada definição, verificar equivalência e limitar a comparação até que a base seja compatível. Alternativamente, apresentar resultados separados pode ser mais honesto.

### Matemática possível

Se `U = {produto, centro, momento, posição, movimento, condição, custo, decisão}` e `S = {produto, centro, momento, custo}`, então `S ⊆ U`. A relação produto–centro pode incluir `(P1, A)`, `(P1, B)` e outros pares observados. Ela não é necessariamente função de produto para centro porque um produto pode relacionar-se a ambos.

Uma função ocorrência–centro é aceitável se cada ocorrência admissível pertence a exatamente um centro no recorte. Seu domínio exclui ocorrências sem identificação suficiente, que devem ser registradas como lacuna, não apagadas. A função não afirma causa nem execução computacional.

### Revisões possíveis

No operacional, separar “sem movimento” de “histórico incompleto” evita concluir ausência com base em desconhecimento. No gerencial, exibir incompletude e proteger a desagregação reduz confiança indevida. Outra revisão válida é incluir impacto além da frequência ou alterar a fronteira após detectar produto fora do recorte. Defenda sua alternativa pelo propósito e pelo risco.

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

A aula, os exercícios essenciais, esta prática, a solução comentada e a revisão formam uma trilha de aproximadamente **7h30 a 10h**. Exercícios adicionais, terceiro modelo, matemática ampliada e prática aprofundada elevam a carga completa para cerca de **11h30 a 15h**. O aprofundamento é opcional e não condiciona o avanço à Aula 05.
