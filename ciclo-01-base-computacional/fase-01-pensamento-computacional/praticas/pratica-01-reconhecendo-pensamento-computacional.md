# Prática 01 — Reconhecendo pensamento computacional em problemas reais

## Identificação

- **Fase:** Fase 1 — Pensamento Computacional
- **Aula relacionada:** Aula 01 — O que é pensamento computacional
- **Nível esperado:** Nível 1 — Reconhecimento; Nível 2 — Explicação; início guiado do Nível 3 — Aplicação guiada
- **Tempo estimado:** 2 h 30 min a 3 h 15 min, incluindo tentativa, consulta da solução e revisão

## Objetivo

Esta prática ajuda a distinguir descrição vaga, procedimento informal, formulação estruturada inicial, uso de ferramenta, pensamento computacional, automação e verificação. O aluno analisará quatro situações sem escrever código, construir algoritmo ou escolher tecnologia.

As classificações não são caixas mutuamente exclusivas. Uma descrição pode usar uma ferramenta, conter procedimento informal e apresentar alguns elementos de pensamento computacional sem estar suficientemente formulada. O que torna a resposta avaliável é a justificativa baseada no texto.

## Orientações

Analise cada descrição isoladamente. Não use informações de uma versão posterior para preencher lacunas da anterior. Em cada resposta:

1. trate como **evidência** somente o que está escrito;
2. marque como **inferência** uma interpretação plausível que não foi declarada;
3. use “não informado” quando faltar informação;
4. não invente regra, causa, dado, ferramenta ou solução;
5. classifique a verificação como ausente, parcial ou sustentada pela descrição;
6. justifique se há sinais de pensamento computacional;
7. indique o risco de automatizar antes de esclarecer as lacunas.

## Situação 1 — Controle de estoque e reposição

### Descrição 1A

> Precisamos evitar que os centros de distribuição fiquem sem produtos.

### Descrição 1B

> No fim de cada manhã, o responsável abre a planilha. Quando percebe que o estoque está baixo, pede uma quantidade suficiente ao fornecedor e avisa o setor de compras.

### Descrição 1C

> A equipe precisa identificar, por produto e centro, os casos que devem passar por análise de reposição. Estão disponíveis o saldo registrado, as entradas pendentes, as saídas pendentes e o momento da última atualização. O resultado deve registrar quais informações sustentaram cada indicação. Ainda precisam ser definidos o significado de saldo disponível, o limite de reposição, a quantidade a solicitar, o tratamento de registros ausentes ou divergentes e a responsabilidade pela aprovação.

## Situação 2 — Análise de solicitação de benefício

### Descrição 2A

> Precisamos aprovar mais rapidamente as solicitações de benefício e impedir pagamentos indevidos.

### Descrição 2B

> O analista confere os documentos no sistema. Se estiver tudo certo, aprova; se faltar alguma coisa, devolve a solicitação. O sistema também poderia colocar os casos mais fáceis no início da fila.

### Descrição 2C

> Antes de uma decisão, a organização quer registrar, para cada solicitação, os documentos recebidos, as verificações realizadas, a versão da regra oficial considerada e o motivo do resultado. Solicitações com informação ausente, divergente ou excepcional devem permanecer identificáveis para análise humana. Ainda é necessário esclarecer as regras aplicáveis, o acesso aos dados sensíveis, a correção de informações, o tratamento de contestações e as evidências de que casos semelhantes recebem análise consistente.

## Situação 3 — Organização de atendimento

### Descrição 3A

> Precisamos diminuir a fila e atender melhor.

### Descrição 3B

> Cada pessoa retira uma senha. O painel chama por ordem de chegada, mas os casos urgentes passam na frente. Se alguém não responder, o atendente chama a próxima senha.

### Descrição 3C

> A unidade quer representar cada solicitação pelo momento de chegada, pelo tipo de atendimento, pela prioridade declarada e pelo estado atual: aguardando, chamada, em atendimento, concluída ou ausente. A ordem usada e as mudanças de estado devem poder ser explicadas posteriormente. Permanecem em aberto os critérios de urgência, os conflitos entre prioridades, o retorno de uma pessoa ausente, a capacidade de atendimento e o significado mensurável de “atender melhor”.

## Situação 4 — Atividade cotidiana não tecnológica

Neste título, “não tecnológica” significa **sem computador ou tecnologia digital**. A folha de papel e o método continuam sendo artefatos e práticas humanas; a expressão não reduz tecnologia a software nem contradiz a concepção ampla estudada na Fase 0.

### Descrição 4A

> Quero me organizar para não esquecer itens importantes nas compras da semana.

### Descrição 4B

> Antes de sair, olho a cozinha, anoto em papel o que está faltando e risco cada item quando o encontro no mercado.

### Descrição 4C

> A família usa uma folha de papel com o nome do item, o motivo da necessidade, a indicação de que ele já existe ou não em casa e o resultado da compra: obtido, substituído, não encontrado ou deixado para depois. Antes e depois da compra, uma pessoa revisa as necessidades consideradas essenciais. Substituições dependem do orçamento, de restrições, de preferências e do julgamento das pessoas envolvidas. Nenhum computador é utilizado.

## Etapa 1 — Mapa rápido das 12 descrições

Compare todas as versões, mas responda de forma breve. Na primeira coluna, use uma classificação predominante, como **necessidade vaga**, **procedimento informal** ou **formulação estruturada inicial**. Uso de ferramenta, sinais parciais de pensamento computacional e proposta de automação podem aparecer como qualificações secundárias.

| Descrição | Classificação predominante e qualificação | Evidência textual decisiva |
|---|---|---|
| 1A |  |  |
| 1B |  |  |
| 1C |  |  |
| 2A |  |  |
| 2B |  |  |
| 2C |  |  |
| 3A |  |  |
| 3B |  |  |
| 3C |  |  |
| 4A |  |  |
| 4B |  |  |
| 4C |  |  |

Uma classificação sem trecho de apoio não é suficiente. Também não transforme uma palavra isolada, como “sistema”, “estado” ou “revisão”, em prova automática.

## Etapa 2 — Análise aprofundada de quatro casos

Analise apenas **1B, 2C, 3B e 4C**, um caso de cada domínio. Limite cada célula a uma ou duas frases.

| Caso | Evidência explícita | Inferência tentadora | Escolha justificada | Informação que poderia mudar a escolha |
|---|---|---|---|---|
| 1B |  |  |  |  |
| 2C |  |  |  |  |
| 3B |  |  |  |  |
| 4C |  |  |  |  |

O objetivo não é descobrir um rótulo secreto. É mostrar por que a escolha atual decorre do texto e em que condição precisaria ser revista.

## Etapa 3 — Uma lente diferente por domínio

1. **Estoque — do procedimento à estrutura.** Compare 1B e 1C. Indique três elementos que se tornaram explícitos e duas lacunas que ainda impedem verificar uma indicação de reposição. Não complete as regras ausentes.
2. **Benefício — rastreabilidade e limite.** Explique por que os registros previstos em 2C permitem examinar uma decisão, mas não garantem regra adequada, dado correto ou tratamento justo. Identifique uma pessoa ou grupo que suportaria o risco de erro.
3. **Atendimento — classificação discutível.** Apresente duas classificações plausíveis para 3B, escolha uma delas e indique que nova evidência faria você rever essa escolha.
4. **Compra cotidiana — transferência sem computador.** Explique por que a ausência de computador não decide a classificação de 4C e indique onde julgamento humano continua indispensável.

Cada resposta deve ter entre 60 e 100 palavras. Use as perguntas como apoio; não produza especificação completa, regra de decisão ou solução tecnológica.

## Etapa 4 — Síntese e revisão

- produza um contraexemplo de 80 a 120 palavras para uma destas afirmações: “usar computador demonstra pensamento computacional”, “qualquer procedimento repetível é uma solução adequada” ou “automatizar torna um processo correto”;
- escolha uma descrição A e registre **três fatos explícitos, três lacunas e duas perguntas de esclarecimento**, sem reescrever o problema nem propor solução;
- consulte a solução comentada somente depois da tentativa e registre duas revisões: o que mudou e que evidência motivou a mudança.

## Organização do tempo

- leitura das situações e mapa rápido: 30 a 40 min;
- análises aprofundadas e quatro lentes: 60 a 75 min;
- contraexemplo e quadro de fatos, lacunas e perguntas: 25 a 35 min;
- consulta à solução, revisão e autocorreção: 35 a 45 min.

## Entrega esperada

Entregue o mapa dos 12 casos, a tabela aprofundada, as quatro respostas por domínio, o contraexemplo, o quadro de fatos/lacunas/perguntas e o registro das duas revisões. Respostas concisas são preferíveis a preenchimento repetitivo.

# Solução comentada — consulte apenas depois de tentar

Use esta parte para comparar critérios, não para copiar redações. O mapa oferece uma classificação aceitável e uma âncora textual; outras escolhas continuam válidas quando distinguem evidência, inferência e decisão e reconhecem as lacunas.

## Mapa de referência

| Descrição | Classificação aceitável | Âncora textual |
|---|---|---|
| 1A | necessidade vaga | declara indisponibilidade, mas não define escopo ou verificação |
| 1B | procedimento informal com ferramenta | informa momento, responsável e ação; “baixo” e “suficiente” permanecem vagos |
| 1C | formulação estruturada inicial | explicita informações, resultado rastreável e pontos ainda indefinidos |
| 2A | necessidade vaga com objetivos em tensão | pede rapidez e prevenção de pagamento indevido sem critérios |
| 2B | procedimento informal com ferramenta e proposta prematura de automação | usa sistema, mas “tudo certo” e “casos mais fáceis” não são definidos |
| 2C | formulação estruturada inicial e sociotécnica | registra documentos, regra, motivo, exceções e análise humana |
| 3A | necessidade vaga | “diminuir” e “atender melhor” não possuem medida |
| 3B | procedimento informal com sinais parciais | representa solicitações e ordem, mas não define urgência ou retorno |
| 3C | formulação estruturada inicial | explicita campos, estados, explicação posterior e perguntas abertas |
| 4A | necessidade cotidiana vaga | “item importante” não possui critério declarado |
| 4B | procedimento informal manual com sinais parciais | usa lista e marcação, mas não distingue todos os resultados |
| 4C | formulação estruturada inicial manual e limítrofe | representa itens e estados, prevê revisão e preserva julgamento humano |

As letras A, B e C ajudam a comparação, mas não funcionam como gabarito automático. Em especial, 3B, 4B e 4C admitem mais de uma classificação predominante.

## Modelo de análise aprofundada — 2C

**Evidência:** a descrição torna explícitos documentos, verificações, versão da regra, motivo da decisão, exceções e análise humana. Também declara o que permanece aberto: regras aplicáveis, acesso, correção, contestação e critérios para comparar casos.

**Inferência tentadora:** a existência de rastreabilidade não prova que a regra seja adequada, que os dados estejam corretos ou que casos semelhantes recebam tratamento consistente. Esses pontos precisam ser investigados.

**Escolha justificada:** uma classificação defensável é “formulação estruturada inicial e sociotécnica, com possibilidade parcial de verificação”. Ela é inicial porque ainda não há especificação completa; é sociotécnica porque decisões, revisão e responsabilidade continuam distribuídas entre pessoas, regras e sistemas.

**Informação que poderia mudar a escolha:** se documentos, versões e motivos não fossem realmente registrados, a classificação perderia força. Se regras, critérios, responsabilidades e formas de contestação fossem definidos e validados, o caso estaria mais maduro, embora isso ainda não garantisse uma decisão correta ou justa.

Use a mesma estrutura em 1B, 3B e 4C. Não procure imitar o tamanho do modelo: procure tornar visível a passagem da evidência para a decisão.

## Casos limítrofes

### 3B — procedimento ou formulação inicial?

“Procedimento informal com sinais parciais” enfatiza que urgência, empate, retorno e acessibilidade não estão definidos. “Formulação inicial insuficiente” também pode ser aceita se a justificativa reconhecer as representações e os estados já presentes sem fingir que o problema está resolvido. A melhor resposta depende do critério declarado, não do rótulo isolado.

### 4B — pensamento computacional ou organização cotidiana?

A lista externa e a marcação mostram representação e acompanhamento de estado. Ao mesmo tempo, o texto não distingue compra, substituição e desistência, nem declara critérios compartilhados. Classificá-lo como procedimento informal com sobreposição parcial é mais prudente do que transformar toda lista em pensamento computacional.

### 4C — estrutura sem computador

A folha representa itens, motivos e estados, prevê revisão e preserva julgamento humano. Isso sustenta uma formulação estruturada inicial executada manualmente. Também é defensável falar em resolução cotidiana com forte sobreposição, desde que a ausência de computador não seja usada como argumento decisivo.

## Critérios para revisar as quatro lentes

- **Estoque:** a comparação entre 1B e 1C deve mostrar o que muda na representação do problema, e não apenas dizer que uma descrição é “mais detalhada”.
- **Benefício:** procure quem poderá reconstruir uma decisão, quais limites continuam abertos e por que rastreabilidade não equivale a correção.
- **Atendimento:** se você propôs duas classificações para 3B, verifique se ambas usam evidências do texto e se cada uma assume um critério diferente.
- **Atividade cotidiana:** sua análise deve explicar por que computador não é requisito e, ao mesmo tempo, por que qualquer sequência organizada não basta.

No contraexemplo autoral, verifique a fronteira correspondente à afirmação escolhida: tecnologia sem evidência de formulação, repetibilidade sem adequação ou automação sem garantia de correção. No inventário de uma descrição A, não converta suposições em fatos: lacunas devem terminar como perguntas investigáveis.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| Clareza | resposta vaga ou circular | comunica a análise | usa termos com precisão e concisão |
| Distinções | equipara ferramenta, automação e pensamento computacional | distingue conceitos principais | reconhece sobreposições sem apagar diferenças |
| Justificativa | rotula sem evidência | cita elementos do texto | separa evidência, inferência e escolha |
| Lacunas | preenche o não informado | identifica ausências relevantes | explica por que impedem verificar ou decidir |
| Integridade | inventa regra, dado ou ferramenta | marca o que falta | transforma lacunas em perguntas |
| Limites | trata automação como correta ou neutra | identifica risco pertinente | relaciona risco a objetivo, dado, pessoa ou responsabilidade |

Uma resposta alternativa é válida quando sustenta a classificação no texto, explicita critérios, reconhece limites, não transforma inferência em fato e não exige computador para reconhecer estrutura. Depois de comparar, revise duas respostas do mapa ou da tabela aprofundada e registre por que mudaram. Copiar a solução sem justificar a revisão não produz nova evidência de domínio.
