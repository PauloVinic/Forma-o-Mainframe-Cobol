# Aula 04 — Abstração e modelos

## Metadados

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo:** De problemas informais a soluções estruturadas
- **Posição:** quarta de 14 aulas
- **Competência:** C04 — Abstrair e modelar
- **Níveis trabalhados:** Nível 2 — explicação; Nível 3 — aplicação guiada; início do Nível 4 em caso simples e delimitado
- **Pré-requisitos:** formulação de problemas; todo, partes, critérios de decomposição, dependências, interfaces, lacunas, sobreposições e propriedades globais
- **Prática associada:** `../praticas/pratica-04-modelando-o-mesmo-problema.md`
- **Projeto integrado:** início do Projeto Parcial 2, com dois modelos do problema de estoque

## Introdução: do problema decomposto ao modelo útil

### Objetivo da aula

Ao concluir esta aula, o aluno deverá conseguir definir operacionalmente abstração e modelo; distinguir abstração de vagueza e modelo de realidade, dado e representação; declarar propósito, pergunta, público, perspectiva, fronteira e nível de detalhe; selecionar objetos, atributos, condições e relações relevantes; justificar e classificar omissões; construir dois modelos textuais ou tabulares simples do mesmo caso; comparar perdas, vieses, riscos e domínios de validade; confrontar os modelos com evidências e revisá-los.

Não basta afirmar que um modelo “está simples” ou “tem os dados importantes”. É preciso explicar para quê, para quem e em qual decisão; mostrar o que ficou de fora; e reconhecer quando o recorte deixa de servir.

### O problema que a aula resolve

A Aula 03 produziu partes, dependências, interfaces e três decomposições do estoque. Tentar mostrar simultaneamente toda ocorrência, produto, centro, registro, movimento, regra, pessoa afetada, indicador e incerteza pode gerar excesso de detalhe e perda da pergunta principal.

O oposto também é sério: uma descrição curta pode apagar exceção crítica ou divergências. Reduzir 2.400 linhas a uma taxa ajuda algumas perguntas, mas pode esconder ocorrência de baixo volume e alto impacto.

Precisamos decidir quais aspectos observar em função de uma pergunta. Essa decisão é a abstração. Precisamos organizar os aspectos selecionados, suas relações e pressupostos em uma construção examinável. Essa construção é o modelo.

### Ponte com a Aula 03

Decomposição decide como um todo pode ser dividido segundo um critério, preservando conexões necessárias à recomposição. Abstração decide quais aspectos desse todo ou de suas partes devem ser considerados em determinado nível e propósito. Modelo organiza a seleção. Representação materializa o modelo em texto, tabela ou outra forma.

Essa sequência não é rígida. Construir um modelo pode revelar uma parte ausente e exigir nova decomposição; uma evidência pode mudar a pergunta; uma representação pode expor ambiguidade no modelo. Nesta aula, o foco está no conteúdo selecionado, não na escolha detalhada entre meios de representação, tema da Aula 06.

## Caso de abertura: dois públicos olhando o mesmo estoque

O caso consolidado possui dois centros, três produtos críticos e 2.400 linhas examinadas. Destas, 192 não foram atendidas: taxa geral de 8%. As taxas por centro são 6% e 10,8%. Há 29 históricos incompletos. As causas ainda não foram estabelecidas, a meta inferior a 3% é candidata e qualquer ação precisa proteger custo, perdas, divergência e transferências. Soluções ainda não foram escolhidas.

Uma equipe operacional recebe o pedido de caracterizar as linhas não atendidas e examinar hipóteses sobre o ocorrido. Para cada ocorrência, pode precisar de produto, centro, momento, posição registrada, movimentos, condição física, separação, divergência, decisão e ação posterior. Sua unidade de análise é a linha ou ocorrência. Uma média geral não caracteriza uma ocorrência nem determina sua causa.

A gestão precisa acompanhar taxas, produtos afetados, custo, perdas, meta candidata e proteções. Sua unidade é um conjunto de linhas em período declarado; examinar 2.400 histórias completas dificultaria perceber diferenças globais.

Os pedidos tratam do mesmo problema com detalhes diferentes. O operacional favorece investigação, mas dificulta visão global; o gerencial favorece comparação, mas pode esconder ocorrência crítica. Nenhum é superior ou mais verdadeiro. Ambos selecionam, perdem informação e declaram limites.

## Abstração: seleção intencional e omissão controlada

### Definição operacional

Adotaremos:

> **Abstração é a seleção intencional de aspectos relevantes de um objeto, problema ou sistema para uma pergunta e um propósito declarados, em determinado nível, com omissão controlada dos demais aspectos e explicitação dos limites produzidos.**

Seleção significa que nem tudo entra; intenção, que a escolha pode ser explicada e revista. Relevância surge da relação entre objeto, pergunta, público e uso. Propósito informa a finalidade; nível, a resolução. Omissão controlada exige conhecer exclusão e risco. Limite registra onde a seleção deixa de sustentar conclusão ou decisão.

Abstrair não é conhecer menos por descuido. Um detalhe pode ser dispensável para comparar taxas e indispensável para investigar uma perda. A cor de uma embalagem talvez não importe para a taxa de atendimento; sua identificação visual pode importar quando embalagens semelhantes induzem separação incorreta. A relevância muda com a pergunta.

### Abstração não é vagueza

“O estoque estava errado” é vago se não distingue quantidade física, saldo registrado, disponibilidade, reserva ou projeção. A vagueza deixa interpretações concorrentes sem controle. Um modelo abstrato pode usar “disponibilidade”, desde que declare o significado adotado, os componentes considerados, o momento de referência e as situações em que esse conceito não basta.

Excluir movimentos individuais com motivo e ligação para consulta é omissão justificada. Não perceber que abandonos saíram do total é omissão não controlada. “Ocorrência” pode ser termo genérico controlado se definido como linha válida não atendida no período; “caso resolvido” é ambíguo se puder significar resposta enviada, correção ou satisfação. Decidir não detalhar é legítimo quando motivo e consequência ficam visíveis; falta de evidência não vira abstração por ser descrita brevemente.

### Abstração não é simplesmente resumir

Um resumo reduz extensão e pode preservar ou destruir o que importa. Abstração seleciona conforme propósito e, às vezes, exige ampliar um detalhe. Um resumo gerencial de dez páginas pode ser mal abstraído; uma tabela de trinta ocorrências críticas pode ser a abstração apropriada para uma investigação.

Também não se abstrai removendo “detalhes difíceis” até obter uma história confortável. Exceções, incertezas e pessoas afetadas podem ser justamente os aspectos decisivos. Abstração não é pensamento superficial, imagem bonita, generalização sem evidência, eliminação de exceções nem cópia da realidade em escala menor. É uma escolha responsável e auditável.

## Modelo: uma construção para um propósito

### Definição operacional

Adotaremos:

> **Modelo é uma construção deliberada que organiza aspectos selecionados e relações de um objeto de interesse para descrever, explicar, comparar, monitorar, prever com ressalvas, comunicar ou apoiar uma decisão, dentro de propósito, fronteira, público e condições de validade declarados.**

Um modelo não é realidade, cópia completa, descrição neutra, verdade ou prova de hipótese. Pode combinar dados, relações e pressupostos, ser útil mesmo incompleto, ter cálculos corretos e ser inadequado à decisão ou perder validade quando o contexto muda.

O modelo também não substitui conhecimento do domínio. Se “linha não atendida” tem definições divergentes entre centros, uma taxa calculada com precisão continua semanticamente frágil. O modelo precisa declarar a convenção e confrontá-la com pessoas, registros e ocorrências.

### Realidade, dado, informação, modelo e representação

O **objeto de interesse** é aquilo observado, analisado ou imaginado: aqui, o atendimento de linhas de estoque em dois centros. Um **dado** é uma representação registrada de algum aspecto, como “Centro A”, “produto P2” ou “não atendida”. **Informação** é dado interpretado em contexto, como “a linha do produto P2 não foi atendida no Centro A no ciclo observado”.

O **modelo** organiza seletivamente aspectos e relações para uma finalidade. A **representação do modelo** é a forma material pela qual ele pode ser examinado: texto, tabela, e futuramente diagrama, equação ou outra notação. Modelo e representação não são idênticos. O mesmo modelo pode ser expresso por texto e tabela; uma tabela bem formatada pode conter dados sem declarar propósito, população ou relações e, por isso, não constituir um modelo adequado.

Uma planilha pode conter registros, realizar cálculos e materializar parte de um modelo. Sua existência não demonstra que a pergunta foi formulada, que a população está correta ou que omissões foram auditadas. Aparência e precisão numérica não demonstram adequação, coerência interna nem sustentação empírica.

### Modelo não é especificação, algoritmo ou implementação

Uma especificação pode definir requisitos detalhados e verificáveis; algoritmo define procedimento; implementação materializa decisões em meio executável. Os modelos desta aula são exploratórios, descritivos, analíticos ou orientados à decisão. Não definem sistema, módulos, serviços, contratos técnicos ou processamento passo a passo.

Um modelo pode informar especificação futura, indicar relações e orientar investigação, mas não a substitui, não diz necessariamente como processar nem prova causa.

## Propósito, pergunta, público e perspectiva

### Declarar antes de selecionar

Antes de construir, registre: para quê; que pergunta; para quem; que decisão será apoiada; qual horizonte; e quem responde pelas consequências. Essas declarações não precisam surgir perfeitamente na primeira tentativa, mas precisam existir para que a seleção possa ser avaliada.

Propósitos incluem descrever, investigar hipóteses, comparar, monitorar, comunicar risco e decidir. Prever exige evidências não desenvolvidas aqui. Um modelo pode combinar finalidades, desde que explicite tensões.

Perguntas produzem seleções diferentes: investigar ocorrências exige acesso individual; comparar taxas exige populações equivalentes; localizar divergências exige confrontar posições; examinar autorização exige responsabilidades. Dados corretos que não respondem à pergunta podem ser irrelevantes.

### Público e responsabilidade

Público é quem precisa interpretar ou usar o modelo. Pode incluir operador, analista, gestor, auditor, responsável técnico e pessoa afetada. Não se deve presumir que gestor sempre quer pouco detalhe ou que operador nunca precisa de visão agregada. O conteúdo depende da responsabilidade concreta.

Pessoas afetadas não são apenas “usuárias”. Um modelo pode mudar prioridade e acesso mesmo quando elas não consultam o artefato; sua experiência pode revelar omissões e consequências invisíveis ao público principal.

### Perspectiva

Perspectiva é o conjunto de preocupações privilegiado. O modelo operacional privilegia ocorrências; o gerencial, comparação e proteção global. Isso não invalida o modelo, mas precisa ser explícito: definir fronteiras e categorias determina o que se torna visível.

Dois modelos podem ser simultaneamente adequados porque respondem a perguntas diferentes. Eles deixam de ser adequados quando são usados fora dessas perguntas ou quando perdas relevantes não são compensadas por rastreabilidade, desagregação ou outro controle.

## Fronteira, nível de detalhe e tipos de omissão

### Três fronteiras relacionadas

A fronteira do problema declara o que a formulação pretende enfrentar. A fronteira da decomposição define o todo dividido segundo um critério. A fronteira do modelo recorta os aspectos que serão organizados para uma pergunta. Elas podem coincidir parcialmente, mas não são idênticas.

O problema de estoque inclui atendimento, custos, perdas, divergências e transferências. Um modelo operacional pode focar as 192 linhas não atendidas e suas evidências. Um gerencial pode abranger as 2.400 linhas para calcular taxas, mas excluir detalhes de movimento da visualização principal. O que está fora do modelo não deixa de existir.

### Níveis de detalhe

Uma visão agregada reúne ocorrências em indicadores. Uma intermediária preserva grupos, como centro e produto. Uma detalhada preserva a ocorrência individual e seus atributos. Nível não é sinônimo de importância ou verdade. O agregado revela proporções; o detalhe revela trajetórias e exceções.

Detalhe excessivo pode esconder relações globais; agregação pode esconder subgrupos, definições e impacto raro. Modelos podem permitir passagem entre níveis sem representar tudo simultaneamente. Ligar taxa a ocorrência importa mais que uma tabela sem caminho de investigação.

### Classificar omissões

Omissões precisam ser distinguidas:

| Situação | Significado | Exemplo | Tratamento |
|---|---|---|---|
| Deliberada | aspecto conhecido excluído por não servir ao propósito atual | sequência completa de movimentos na visão gerencial | justificar e preservar acesso quando necessário |
| Desconhecida | aspecto relevante ainda não disponível | conteúdo de 29 históricos incompletos | registrar lacuna; não fingir ausência |
| Adiada | aspecto relevante reservado para análise posterior | custo detalhado por ocorrência | indicar prazo ou condição de retorno |
| Fora da fronteira | aspecto existente, mas fora do recorte declarado | outros produtos fora dos três críticos | declarar fronteira e risco |
| Agregada | detalhes substituídos por medida conjunta | linhas transformadas em taxa por centro | permitir desagregação quando o risco exigir |
| Omitida indevidamente | exclusão capaz de distorcer pergunta ou decisão | retirar casos graves do denominador sem informar | corrigir ou restringir o uso |

“Não temos o dado” não equivale a “decidimos omiti-lo”. “Fora da fronteira” não equivale a irrelevante para sempre. A omissão controlada deixa rastro: motivo, risco e condição de revisão.

### Pressupostos, domínio de validade e limites

Pressuposto é algo aceito provisoriamente para que o modelo possa operar, como considerar comparáveis as definições de “linha válida” nos dois centros. Pressupostos ocultos criam confiança indevida. Devem ser declarados e, quando importantes, confrontados com evidências.

Domínio de validade é o conjunto de situações em que há razões para usar o modelo. O modelo gerencial pode valer para as 2.400 linhas, nos dois centros, três produtos e ciclo definido, conforme a mesma regra de contagem. Não se estende automaticamente a outros produtos, períodos ou definições.

Limite é uma condição em que o modelo não responde, perde precisão relevante ou não deve apoiar decisão. Uma taxa por centro não estabelece causa; o operacional não estima sozinho tendência global. Declarar limite não enfraquece o modelo: impede que utilidade local seja confundida com verdade universal.

## O conteúdo do modelo: objetos, atributos, estados e relações

### Objetos ou entidades de interesse

Objeto de interesse é algo cuja identidade ou condição importa à pergunta. “Entidade” será usada aqui em sentido analítico, não como termo de modelagem de banco de dados. Linha de solicitação, produto e centro podem ser objetos conforme o recorte. Outros substantivos exigem precisão: movimento pode ser evento ou seu registro; análise é atividade, seu registro é informação persistida e sua conclusão é resultado; o ato de decidir é atividade ou evento, enquanto a decisão registrada pode ser resultado ou objeto documental. Evidência é material usado para sustentar ou enfraquecer uma afirmação, não sinônimo automático de objeto.

Nem todo substantivo precisa virar objeto. Atividade, registro e resultado podem receber tratamento diferente conforme a perspectiva, que precisa ser declarada. Se a pergunta gerencial trata taxas por centro, a ocorrência individual pode continuar acessível sem aparecer como unidade principal. Selecionar objetos significa explicar por que a identidade de cada tipo importa.

### Atributos e condições relevantes

Atributo é uma característica selecionada de um objeto: produto da linha, centro, momento, quantidade, completude do histórico. Um atributo deve ter significado suficiente para interpretação. “Status” sem valores e referência pode esconder mais do que revela.

Estado ou condição relevante descreve como o objeto se encontra em determinado referencial, como “histórico incompleto”, “separação não confirmada” ou “divergência identificada”. Nesta aula, reconhecemos condições; não construímos sequência de transições, rastreamento ou invariantes.

### Relações sem causalidade presumida

Relação conecta elementos relevantes: uma linha refere-se a um produto; ocorreu em um centro; possui registros de movimentos; uma decisão foi tomada por pessoa autorizada. A presença de relação não prova causa. Produto P2 aparecer em mais ocorrências não demonstra que o produto causou a falha.

Uma relação pode ser importante mesmo sem atributo numérico. Responsabilidade, pertencimento, referência e impacto também conectam elementos. O modelo deve preservar as relações necessárias à pergunta e declarar as que ficaram de fora.

## Adequação, perdas, vieses e revisão

### Avaliar adequação ao propósito

Um modelo é **adequado** quando serve à pergunta, ao público e à decisão declarados. Possui **coerência interna** quando definições, elementos, relações e cálculos são compatíveis entre si. Possui **sustentação empírica** na medida em que suas afirmações são compatíveis com as evidências disponíveis. Seu **domínio de validade** delimita população, período, definições e condições em que esse uso é sustentado. Nenhuma dessas propriedades significa verdade universal ou completude.

Um modelo adequado usa evidência compatível, expõe pressupostos e omissões e respeita limites. Avalie se unidade corresponde à pergunta; população, período e fronteira estão claros; elementos e relações bastam; informação incluída tem função; desconhecidos estão separados de omissões; o agregado retorna à evidência; e decisões não apoiadas são explícitas.

Modelo visualmente claro pode ser inadequado, internamente incoerente ou pouco sustentado pelas evidências. Modelo complexo pode ser desnecessário. Adequação não é beleza, volume nem precisão decimal.

### Perda de informação e falsa precisão

Toda seleção pode perder informação. Perda aceitável é aquela conhecida, proporcional ao propósito e compensada quando necessário. A taxa de 8% perde a identidade das 192 ocorrências. Isso pode ser aceitável para uma visão geral, mas não para investigar causa ou reparar impacto.

Falsa precisão ocorre quando números parecem mais exatos do que conceitos, dados ou condições permitem. Informar 8,00% não resolve 29 históricos incompletos, definições divergentes ou população mal delimitada. Casas decimais descrevem um cálculo, não a validade de seus insumos.

### Viés de seleção, agregação e exceção crítica

Viés de seleção surge quando a escolha do que entra favorece uma visão inadequada. Excluir linhas abandonadas, registrar apenas ocorrências com histórico completo ou ouvir somente um centro pode alterar a conclusão. Agregação pode esconder que um produto piorou enquanto a taxa geral melhorou.

Uma exceção crítica é um caso pouco frequente cujo impacto não pode ser tratado como ruído. Uma linha associada a perda elevada, obrigação ou pessoa vulnerável pode pouco alterar a taxa e ainda exigir ação. Raridade não é sinônimo de irrelevância.

### Confrontar com evidências e revisar

O modelo deve ser comparado com registros, ocorrências, pessoas e resultados. Procure casos que ele caracteriza mal ou que enfraquecem as hipóteses examinadas, não apenas exemplos favoráveis. Um caso que contradiz uma afirmação ampla funciona como contraexemplo ao uso pretendido, sem que esta aula ensine generalização sistemática.

Revisar não significa admitir que o modelo nunca serviu. Contexto, evidência e perguntas mudam. A revisão pode alterar fronteira, definição, nível, atributo, relação, proteção ou condição de validade. Registre a versão, o motivo e o efeito: isso produz rastreabilidade.

## Matemática introdutória da seleção e das relações

### Seleção como subconjunto

Seja `U` o conjunto de aspectos possíveis dentro do recorte e `S` o conjunto selecionado:

`S ⊆ U`

`U` não é toda a realidade; depende da fronteira. `S` depende do propósito. Estar em `S` não prova relevância, e ficar fora de `S` não significa inexistência. A notação torna a seleção explícita, mas a justificativa continua necessária.

Se `U = {produto, centro, momento, posição registrada, condição física, custo, cor}` e `S = {produto, centro, momento, custo}`, então `S ⊆ U`. Ainda é preciso avaliar se excluir posição e condição oculta risco.

### Relações e produto cartesiano

Sejam `A` e `B` conjuntos. `A × B` representa intuitivamente os pares possíveis formados por um elemento de `A` e um de `B`. Uma relação `R` entre eles pode ser tratada como subconjunto:

`R ⊆ A × B`

Se `A` contém os três produtos e `B` os dois centros, a relação “produto observado no centro” contém somente os pares efetivamente pertinentes. A notação não diz que produto causa resultado nem que todos os pares ocorreram.

### Função, domínio e codomínio

Função é uma relação particular na qual cada entrada admissível do domínio recebe exatamente uma saída no modelo:

`f: X → Y`

Restringir o domínio é uma decisão de modelagem, não uma forma de fazer casos problemáticos desaparecerem. Seja `O` o conjunto de ocorrências do recorte e `O_identificadas ⊆ O` o subconjunto para o qual o centro pode ser associado. Podemos usar:

`centro: O_identificadas → Centros`

Cada entrada desse domínio recebe exatamente um centro, e o codomínio contém os centros considerados. As ocorrências em `O \ O_identificadas` permanecem registradas como não classificadas ou pendentes, com quantidade e motivo visíveis. Resultados calculados apenas sobre `O_identificadas` não podem ser generalizados silenciosamente para todo `O`.

Quando for coerente com o propósito, outra construção introdutória seria `centro: O → Centros ∪ {não identificado}`. “Não identificado” registra qualidade insuficiente do dado; não é um centro real. Em ambas as abordagens, ausência de identificação não significa inexistência da ocorrência.

Nem toda relação é função. Um produto pode aparecer em vários centros; uma solicitação pode possuir vários documentos. Uma função matemática não prova determinismo, processamento real ou causalidade. Ela apenas declara uma correspondência no modelo. Não estudaremos aqui composição, injetividade, sobrejetividade ou prova.

## Caso progressivo: dois modelos e uma revisão

### Modelo operacional

**Propósito:** caracterizar ocorrências não atendidas e orientar investigação. **Pergunta:** que registros, condições, relações e divergências caracterizam cada ocorrência e permitem examinar hipóteses ou encaminhar investigação? **Público:** equipe operacional e analistas responsáveis. **Fronteira:** 192 linhas não atendidas, nos dois centros, três produtos e ciclo observado. **Nível:** ocorrência individual. **Limite:** não estima sozinho tendência nem estabelece causa.

| Elemento | Aspectos selecionados | Motivo | Omissões declaradas |
|---|---|---|---|
| linha | produto, centro, momento, quantidade e condição | identifica a ocorrência | visão agregada fica em outro modelo |
| posição registrada | valor e momento de referência | confronta disponibilidade registrada | não prova condição física |
| movimento | ocorrência, referência e evidência disponível | apoia reconstrução analítica | 29 históricos são incompletos |
| condição física | condição observada e evidência | revela divergência possível | não inferida quando desconhecida |
| separação | condição registrada | localiza ponto de investigação | não cria sequência de execução |
| decisão e ação | ato de decidir, decisão registrada, responsável, fundamento e ação posterior | distingue atividade, resultado registrado, responsabilidade e retorno | não especifica solução técnica |

Relações preservadas incluem linha–produto, linha–centro, linha–posição, linha–registros de movimentos, decisão registrada–responsável e ocorrência–ação. Elas ajudam a reconstruir registros e localizar divergências; não confirmam causa. O modelo omite indicadores agregados da visão principal, custos consolidados e produtos fora do recorte. Seus pressupostos incluem identificação consistente de linha e momento de referência comparável.

### Modelo gerencial

**Propósito:** monitorar magnitude, distribuição e proteções. **Pergunta:** como a taxa varia entre centros, produtos e ciclos, e que sinais exigem investigação? **Público:** responsáveis pela decisão e pessoas encarregadas de custo, perdas e operação. **Fronteira:** 2.400 linhas do ciclo, dois centros e três produtos. **Nível:** agregado com possibilidade de desagregação. **Limite:** não explica ocorrências nem prova causas.

| Indicador ou dimensão | Definição | Uso | Limite |
|---|---|---|---|
| taxa geral | 192 linhas não atendidas em 2.400 | magnitude inicial | esconde distribuição |
| taxa por centro | 6% e 10,8%, conforme população declarada | comparar centros | depende de definição comum |
| taxa por produto e ciclo | proporção na respectiva população | localizar concentração e tendência | grupos pequenos exigem contexto |
| históricos incompletos | 29 ocorrências sinalizadas | proteção de qualidade | não informa conteúdo ausente |
| custo e perdas | medidas conforme definição declarada | impedir melhora aparente com dano | ainda requer fonte e período |
| transferências e divergências | sinais de proteção | acompanhar efeitos colaterais | relação não prova causa |

A meta inferior a 3% permanece candidata, não critério confirmado. O modelo deve permitir retornar de indicador a grupos e ocorrências, além de sinalizar exclusões e dados incompletos.

### Comparação

| Dimensão | Operacional | Gerencial |
|---|---|---|
| finalidade | investigar | monitorar e decidir |
| público principal | operação e análise | responsáveis por decisões e proteções |
| unidade | ocorrência | população e grupo |
| nível | detalhado | agregado/intermediário |
| seleção | posições, movimentos, condições, decisões | taxas, dimensões, custos e proteções |
| perda principal | visão global | trajetória individual |
| evidência exigida | registros e observações por ocorrência | populações, definições e agregações rastreáveis |
| decisão apoiada | investigar e encaminhar | priorizar análise e acompanhar |
| não usar para | inferir tendência sozinho | atribuir causa ou resolver caso individual |

### Caso crítico e conexão

Suponha, apenas para testar o modelo, uma ocorrência de um grupo pequeno que gera perda relevante. Ela pouco altera os 8%, aparece claramente no operacional e pode desaparecer no agregado. O caso é hipotético; não acrescenta fato ao problema. Ele mostra que o gerencial precisa de proteção para impacto e caminho de desagregação, enquanto o operacional precisa comunicar exceções ao nível de decisão.

### Revisão após evidência

Ao descobrir que os 29 históricos estão incompletos e que “disponibilidade” tem definições divergentes entre centros, os modelos precisam mudar. O operacional passa a distinguir “não observado” de “sem movimento” e registra a definição usada em cada centro. O gerencial sinaliza incompletude, suspende comparação direta quando as definições não forem equivalentes e apresenta a taxa com ressalva.

Se um grupo pequeno afetado for apagado pelo agregado, inclui-se proteção de impacto e possibilidade de desagregação. Se houver erro de contagem, corrigem-se numerador, denominador e versões anteriores. A revisão reduz comparabilidade imediata, mas aumenta validade.

## Prática guiada interna: atendimento aparentemente eficiente

Uma área informa: “tempo médio de atendimento: 4 minutos; 92% resolvidos”. A tabela não declara público, período nem significado de resolvido. Chamadas abandonadas foram excluídas e não há limite apresentado.

Antes de seguir, responda:

1. Qual propósito provável e que público poderia usar o modelo?
2. Que elementos foram selecionados?
3. O que foi omitido, desconhecido ou agregado?
4. Que pressuposto sustenta “resolvido”?
5. Que risco nasce da exclusão dos abandonos?
6. Qual revisão mínima permitiria uso mais responsável?

### Análise comentada

O propósito provável é monitorar eficiência, mas precisa ser confirmado. Foram selecionados tempo médio e resolução; distribuição, abandonos, retornos, período, população e definição estão ausentes. Excluir abandonos pode melhorar artificialmente os números, e “resolvido” pode significar encerramento, resposta ou solução efetiva.

Uma revisão mínima declara pergunta, público, período, população, inclusão, definição e limite da média; trata abandonos e permite examinar grupos. Isso torna o modelo auditável, não prova melhora.

## Atividades, síntese e domínio

### Confusões recorrentes

Abstração não é vagueza nem remoção indiscriminada de detalhes. Modelo não é realidade, verdade, algoritmo ou implementação; maior volume não garante adequação, e um modelo não serve automaticamente a todos.

Dado disponível não precisa entrar; dado ausente ainda pode importar; omitido não significa inexistente. Tabela e número não tornam o modelo automaticamente adequado ou neutro. Modelos operacional e gerencial perdem aspectos diferentes.

Exceção rara pode ser crítica. Fronteira e agregação podem introduzir viés. Função não significa causa ou processamento; relação não significa causalidade. Modelo pode ser útil sem prever, e revisão pode responder a nova evidência ou contexto.

### Exercícios essenciais

1. **Objetiva.** Qual alternativa melhor descreve abstração controlada?
   A) Selecionar aspectos ligados ao propósito, sem registrar o que ficou de fora quando a equipe já conhece o caso.
   B) Selecionar os aspectos disponíveis e reduzir detalhes até que o público consiga ler o resultado.
   C) Selecionar para a pergunta de um público e reutilizar a mesma seleção sempre que o objeto de interesse for o mesmo.
   D) Selecionar para pergunta e propósito declarados, registrando omissões, limites e condições de revisão.

2. **Objetiva.** Uma tabela contém valores conferidos, mas não declara população nem período. A melhor avaliação é:
   A) pode apoiar qualquer pergunta sobre os valores, pois a correção numérica compensa a fronteira ausente;
   B) pode ter uso exploratório restrito, mas adequação e domínio de validade não podem ser avaliados até que população e período sejam declarados;
   C) deve ser descartada, pois a ausência dessas declarações torna necessariamente falsos todos os valores;
   D) é adequada para comparar períodos, desde que as colunas usem as mesmas unidades.

3. **Objetiva.** Qual opção distingue corretamente desconhecido de omitido deliberadamente?
   A) Desconhecido é o aspecto relevante cuja informação ainda não está disponível; omitido deliberadamente é conhecido, excluído com justificativa e sujeito a revisão.
   B) Desconhecido é todo elemento fora da fronteira; omitido deliberadamente é o detalhe agregado em um indicador.
   C) Desconhecido é informação reservada para etapa posterior; omitido deliberadamente é aquilo que não pode ser coletado.
   D) Desconhecido é um detalhe agregado sem identificação individual; omitido deliberadamente é todo aspecto que o público não pediu.

4. **Dissertativa.** Defina abstração e modelo com palavras próprias. Explique seleção, propósito, omissão e limite sem usar “resumo” como sinônimo.

5. **Dissertativa.** Diferencie realidade, dado, informação, modelo e representação usando um caso de cobrança.

6. **Análise de caso.** Um relatório de atrasos mostra apenas total mensal. Declare propósito possível, público, fronteira, nível, dois atributos ausentes e uma omissão que seria indevida.

7. **Análise de caso.** Um gestor pede todos os registros individuais para “não perder nada”. Explique duas perdas produzidas pelo excesso de detalhe e proponha modelo intermediário com rastreabilidade.

8. **Comparação guiada.** Para o caso de atendimento, compare duas seleções fornecidas: `{tempo médio, resolvidos}` e `{abandono, retorno, período, população}`. Indique um propósito e um público plausíveis para cada seleção, localize uma omissão relevante e proponha uma revisão. Não construa dois modelos completos.

9. **Objetos e relações.** Em concessão de benefício, identifique quatro objetos, dois atributos por objeto, três relações e uma condição relevante. Não desenhe esquema técnico e não atribua causa.

10. **Revisão.** Um modelo considera “encerrado” igual a “resolvido”. Após reclamações de retorno, revise propósito, definição, atributo e limite; registre evidência e efeito.

### Exercícios de aprofundamento opcional

11. **Conjuntos.** Considere `U = {centro, produto, momento, saldo, condição física, custo, cor}` e `S = {centro, produto, momento, custo}`. Verifique `S ⊆ U`, identifique uma perda aceitável e construa um caso em que excluir condição física seria indevido.

12. **Relação e função.** Dados `P = {P1, P2, P3}` e `C = {A, B}`, escreva uma relação produto–centro. Explique por que ela pode não ser função de `P` para `C`. Depois proponha uma associação ocorrência–centro que seja função, declarando domínio, codomínio e condição de validade.

13. **Análise de caso.** Uma auditoria recebe somente registros com histórico completo. Identifique viés de seleção, domínio de validade aparente e real, decisão que não deve ser apoiada e revisão necessária.

14. **Contraexemplo.** Construa um caso raro que refute o uso de “taxa geral melhorou” como prova de que todos os produtos melhoraram. Não formule regra geral.

15. **Três públicos.** Compare modelo de cobrança para atendente, auditor e pessoa afetada. Evite presumir que um público sempre requer mais ou menos detalhe.

16. **Análise de caso crítico.** Uma meta foi atingida, mas perdas aumentaram. Explique falsa precisão, proteção omitida, evidência necessária e mudança nos dois modelos de estoque.

17. **Transferência.** Escolha agendamento ou conciliação. Construa dois modelos simples, declare domínio de validade e revise um deles após introduzir dado incompleto.

### Recuperação ativa

- O que torna uma abstração controlada?
- Por que abstração não é vagueza?
- Como modelo difere da realidade?
- Qual a diferença entre modelo e representação?
- Por que propósito vem antes do detalhe?
- Como público altera a seleção?
- O que é omissão deliberada?
- Como desconhecido difere de omitido?
- O que é nível de detalhe?
- Quando dois modelos diferentes podem ser adequados?
- O que é domínio de validade?
- Como uma agregação pode esconder problema?
- Quando uma relação não é função?
- Como revisar um modelo?

### Reflexão

Quem escolhe o que aparece no modelo e quem pode contestar? Que pessoas afetadas não participaram da definição? Como um modelo usado para distribuir recursos transforma omissões em consequências? Uma métrica pode mudar o comportamento de quem é avaliado? Como proteger exceções minoritárias? Quais pressupostos precisam ser transparentes? Quem tem poder para definir categorias? Que reparação existe quando uma omissão causa dano?

### Síntese

Abstração seleciona aspectos relevantes para pergunta, propósito, público e nível, omitindo os demais de modo controlado. Modelo organiza a seleção e suas relações dentro de fronteira e domínio de validade. Objetos, atributos, condições e relações dão conteúdo ao modelo; representação torna-o examinável.

Modelos diferentes do mesmo caso podem ser adequados e perder informações diferentes. Avaliá-los exige examinar omissões, pressupostos, falsa precisão, vieses, exceções e rastreabilidade. Evidência e feedback podem exigir revisão. Ao tornar atributos, relações, categorias e condições comparáveis, os modelos preparam a Aula 05, mas ainda não estabelecem padrões ou regras gerais.

### Mini glossário

**Abstração:** seleção intencional para propósito e pergunta, com omissão e limites declarados.
**Seleção:** escolha dos aspectos que entram no modelo.
**Omissão controlada:** exclusão conhecida, justificada e auditável.
**Detalhe:** aspecto observado em determinada resolução.
**Nível de abstração:** grau de agregação ou detalhe adotado.
**Modelo:** construção seletiva para descrever, analisar, comunicar ou decidir.
**Objeto de interesse:** aquilo que se pretende observar ou analisar.
**Entidade:** objeto analítico cuja identidade ou condição importa ao modelo; não é usada aqui como termo de banco de dados.
**Atributo:** característica selecionada de um objeto.
**Relação:** associação entre elementos, sem causalidade presumida.
**Estado:** condição relevante de um objeto em um referencial.
**Propósito:** finalidade do modelo.
**Pergunta:** questão que orienta a seleção.
**Público:** quem interpreta, usa ou é responsável pelo uso.
**Perspectiva:** preocupações privilegiadas pelo recorte.
**Fronteira:** limite do que o modelo inclui.
**Domínio de validade:** situações em que o uso é sustentado.
**Pressuposto:** condição aceita provisoriamente e que deve ser explícita.
**Representação:** forma pela qual o modelo é expresso.
**Agregação:** reunião de ocorrências em medida ou grupo.
**Perda de informação:** aspecto que deixa de estar disponível após seleção ou agregação.
**Falsa precisão:** aparência de exatidão maior que a sustentada.
**Viés de seleção:** distorção ligada ao que entra ou fica fora.
**Adequação:** capacidade de servir à pergunta, ao público e à decisão declarados.
**Validade:** sustentação de um uso dentro de definições, condições, domínio e evidências declarados; não significa verdade universal.
**Rastreabilidade:** possibilidade de relacionar seleção, evidência, decisão e revisão.
**Contraexemplo:** caso que mostra o limite de uma afirmação.
**Função:** relação que atribui exatamente uma saída a cada entrada admissível.
**Domínio:** conjunto de entradas admissíveis de uma função.
**Codomínio:** conjunto declarado de saídas possíveis.

### Critérios de domínio

No **Nível 1**, o aluno reconhece abstração, modelo, propósito e omissão em exemplos. No **Nível 2**, explica abstração sem vagueza e distingue modelo, realidade, dado e representação. No **Nível 3**, constrói de modo guiado modelo simples, declarando pergunta, público, fronteira, nível, seleção, omissões, relações e limites.

O início do **Nível 4** aparece quando produz autonomamente dois modelos de um caso simples, justifica seleções e omissões, compara perdas, encontra viés ou exceção crítica, declara domínio de validade e revisa após evidência. Isso ainda não declara C04 plenamente dominada em contextos complexos.

## Conexão com a Aula 05 — Padrões e generalização

Modelos tornam elementos comparáveis ao selecionar atributos, relações, categorias e condições. A próxima aula perguntará: que semelhanças são relevantes? Que diferenças impedem agrupamento? Que padrão parece existir? Que contraexemplo o limita? Até onde uma regra pode ser generalizada?

Esta aula não respondeu essas perguntas. Comparou casos apenas para avaliar modelos e seus limites. Reconhecer padrões, construir generalizações, formular regras e validar exceções pertencem à Aula 05.

## Referências, métricas e carga

### Referências utilizadas

- WING, Jeannette M. Computational Thinking. *Communications of the ACM*, v. 49, n. 3, p. 33–35, 2006. DOI: [10.1145/1118178.1118215](https://doi.org/10.1145/1118178.1118215). Abstração no pensamento computacional, sem definição universal.
- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. DOI: [10.1145/3664191](https://doi.org/10.1145/3664191). Progressão e níveis de abstração.
- PÓLYA, George. *How to Solve It*. 2. ed. Princeton University Press, 1957. Seleção e revisão, não receita universal.
- SIMON, Herbert A. The Architecture of Complexity. *Proceedings of the American Philosophical Society*, v. 106, n. 6, p. 467–482, 1962. Níveis em sistemas complexos, sem modelo único.
- ROSEN, Kenneth H. *Discrete Mathematics and Its Applications*. 8. ed. McGraw-Hill, 2019. Conjuntos, relações e funções.
- ISO; IEC; IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*. ISO, 2017. [Registro oficial](https://www.iso.org/standard/71952.html). Apoio terminológico sem reprodução normativa.

### Métricas e carga estimada

- **Extensão e estrutura:** 5.971 palavras, 465 linhas, 15 seções H2 e 42 subseções H3; conceitos matemáticos: subconjunto, produto cartesiano, relação, função, domínio e codomínio.
- **Exercícios:** 10 essenciais e 7 de aprofundamento opcional; três objetivas, sete dissertativas/construtivas, ao menos seis análises de caso, uma questão de conjuntos, uma de relação/função, um contraexemplo e atividades de revisão.
- **Casos centrais:** estoque progressivo, atendimento guiado e transferências nos exercícios.
- **Fontes:** seis.
- **Prática associada:** 2.399 palavras, 257 linhas, 15 seções H2, seis subseções H3 e nove blocos de produção e revisão.
- **Trilha essencial:** leitura e anotações (2h–2h30), recuperação ativa (20–30 min), exercícios essenciais (1h30–2h), prática essencial (2h45–3h45) e consulta da solução, revisão e autoavaliação (30–45 min) — aproximadamente 7h05 a 9h30.
- **Carga completa opcional:** trilha essencial mais exercícios adicionais, auditoria e casos completos, matemática ampliada e terceiro modelo — aproximadamente 10h30 a 14h.
