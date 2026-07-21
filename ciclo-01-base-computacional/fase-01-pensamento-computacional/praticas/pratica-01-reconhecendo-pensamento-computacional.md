# Prática 01 — Reconhecendo pensamento computacional em problemas reais

## Identificação

- **Fase:** Fase 1 — Pensamento Computacional
- **Aula relacionada:** Aula 01 — O que é pensamento computacional
- **Nível esperado:** Nível 1 — Reconhecimento; Nível 2 — Explicação; início guiado do Nível 3 — Aplicação guiada
- **Tempo estimado:** 2 h 30 min a 3 h, incluindo tentativa, consulta da solução e revisão

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

## Tabela de análise

Preencha uma tabela para cada situação, mantendo as três descrições separadas.

| Campo de análise | Descrição A | Descrição B | Descrição C |
|---|---|---|---|
| Classificação predominante e classificações secundárias |  |  |  |
| Objetivo aparente |  |  |  |
| Elementos explícitos |  |  |  |
| Suposições necessárias |  |  |  |
| Dados ou estados identificáveis |  |  |  |
| Procedimento presente |  |  |  |
| Possibilidade de verificação |  |  |  |
| Elementos de pensamento computacional |  |  |  |
| Elementos ausentes |  |  |  |
| Risco de automatização prematura |  |  |  |

## Entrega esperada

Entregue:

- quatro tabelas preenchidas;
- uma justificativa de 150 a 250 palavras para uma classificação discutível, preferencialmente 3B, 4B ou 4C;
- um contraexemplo a uma destas afirmações: “usar computador demonstra pensamento computacional”, “qualquer lista de passos é algoritmo” ou “automatizar torna um processo correto”;
- uma versão melhorada de uma descrição vaga, com 100 a 180 palavras, registrando o conhecido, o que precisa ser esclarecido e como o resultado poderia ser examinado, ainda sem solução completa;
- depois da consulta à solução comentada, um registro breve de duas revisões realizadas.

# Solução comentada — consulte apenas depois de tentar

As respostas abaixo são referências de análise, não redações obrigatórias. “Explícito” corresponde à evidência textual; “suposição” corresponde a inferência; “classificação” é escolha justificada. Uma alternativa deve ser aceita quando usa evidência, declara critérios e reconhece lacunas.

## Situação 1 — Comentário

### 1A

**Evidência:** o texto nomeia centros, produtos e um estado indesejado, mas não informa escopo, período, procedimento nem o significado de “ficar sem”. **Inferência:** presumir que toda falta tem a mesma causa ou que já existe uma regra de reposição seria inventar informação. **Classificação escolhida:** descrição vaga de uma necessidade; o objetivo aparente é evitar indisponibilidade e ainda não há base para verificar o resultado. **Risco de automatização prematura:** produzir excesso de estoque ou priorização inadequada a partir de critérios não declarados.

### 1B

**Evidência:** há uma planilha, um momento, um responsável, uma observação, uma ação e uma comunicação; “baixo” e “quantidade suficiente” não são definidos. **Inferência:** não se pode concluir que a planilha contenha histórico confiável nem que pessoas diferentes julguem da mesma forma. **Classificação escolhida:** procedimento informal com uso de ferramenta e sinais parciais de pensamento computacional. A verificação é parcial, pois pode haver registro, mas nenhum resultado esperado foi definido. **Risco de automatização prematura:** repetir em escala decisões baseadas em termos vagos.

### 1C

**Evidência:** objeto de análise, informações disponíveis, resultado esperado e lacunas estão declarados; a origem de uma indicação poderia ser examinada. **Inferência:** não se pode presumir que os registros sejam atuais, que “saldo disponível” já tenha significado comum ou que exista uma regra aprovada. **Classificação escolhida:** formulação estruturada inicial; “modelo inicial” também é justificável, desde que não seja confundido com especificação completa. Ainda não existe procedimento de execução nem garantia de correção. **Risco de automatização prematura:** dar aparência de precisão a indicações produzidas com conceitos, limites ou responsabilidades indefinidos.

## Situação 2 — Comentário

### 2A

**Evidência:** o texto menciona velocidade e prevenção de pagamento indevido, sem dados, regras, procedimento ou medida. **Inferência:** não é possível saber se os dois objetivos são compatíveis; aprovar menos poderia reduzir pagamentos e atrasar casos devidos, enquanto aprovar mais rapidamente poderia elevar risco. **Classificação escolhida:** descrição vaga de uma necessidade com objetivos potencialmente conflitantes. **Risco de automatização prematura:** transferir ao solicitante o custo de critérios e conflitos ainda não esclarecidos.

### 2B

**Evidência:** há uso de sistema, conferência, aprovação, devolução e uma proposta de reordenar casos; “tudo certo” e “casos mais fáceis” não têm critério. **Inferência:** estados como em análise, aprovado e devolvido podem ser reconhecidos, mas o texto não permite presumir elegibilidade, justiça da fila ou tratamento de exceções. **Classificação escolhida:** procedimento informal com uso de ferramenta e proposta de automação. O sistema utilizado não torna a formulação suficiente. **Risco de automatização prematura:** priorizar ou devolver solicitações por uma noção não definida de facilidade ou correção.

### 2C

**Evidência:** documentos, verificações, versão da regra, motivo, exceções e análise humana são explícitos; regras, acesso, correção, contestação e critérios de consistência permanecem abertos. **Inferência:** rastreabilidade não permite presumir que a regra seja adequada, que os dados estejam corretos ou que casos semelhantes já recebam tratamento consistente. **Classificação escolhida:** formulação estruturada inicial e deliberadamente sociotécnica, com possibilidade parcial de verificação. **Risco de automatização prematura:** aplicar de modo rastreável uma regra inadequada ou dados incorretos e ampliar efeitos sobre pessoas.

## Situação 3 — Comentário

### 3A

**Evidência:** há dois objetivos gerais, reduzir fila e atender melhor, sem medida, público, período ou procedimento. **Inferência:** os objetivos podem convergir ou competir; o texto não autoriza escolher uma interpretação de “melhor”. **Classificação escolhida:** descrição vaga de uma necessidade, sem base suficiente para verificação. **Risco de automatização prematura:** otimizar apenas velocidade e prejudicar qualidade, acessibilidade ou casos complexos.

### 3B

**Evidência:** a senha representa uma solicitação; existe ordem de chegada, prioridade para urgência e uma ação diante da ausência. **Inferência:** estados como aguardando, chamada e ausente podem ser reconhecidos, mas urgência, empate, retorno e acessibilidade não foram definidos. **Classificação escolhida:** procedimento informal com elementos de representação, estado e priorização; “formulação inicial insuficiente” é defensável se as lacunas forem reconhecidas. **Risco de automatização prematura:** repetir em escala uma classificação de urgência ou uma ordem inadequada.

### 3C

**Evidência:** campos, estados, explicação posterior e perguntas abertas estão explícitos; não há regra completa de ordenação nem definição de “atender melhor”. **Inferência:** a presença dos campos não permite concluir que os critérios sejam legítimos ou que qualidade se reduza ao tempo de espera. **Classificação escolhida:** formulação estruturada inicial, com possibilidade de verificar parte da ordem, mas não a qualidade total do atendimento. **Risco de automatização prematura:** aplicar critérios ainda não legitimados e prejudicar pessoas ou grupos.

## Situação 4 — Comentário

### 4A

**Evidência:** há um objetivo cotidiano, mas “item importante” não tem significado declarado e não existe procedimento ou forma de verificação. **Inferência:** não se pode presumir quem decide a importância, quais compras pertencem à semana ou por que algo foi esquecido. **Classificação escolhida:** descrição vaga de uma necessidade cotidiana. **Risco de automatização prematura:** escolher um aplicativo que apenas digitalize a ambiguidade.

### 4B

**Evidência:** há inspeção da cozinha, registro em papel e marcação dos itens encontrados; a lista representa necessidades, mas o ato de riscar não distingue compra, substituição ou desistência. **Inferência:** observar a cozinha pode não revelar todas as necessidades, e pessoas diferentes podem usar critérios distintos. **Classificação escolhida:** procedimento informal manual com representação externa e sinais parciais de pensamento computacional; “raciocínio cotidiano organizado com sobreposição” também é aceitável. **Risco de automatização prematura:** ampliar uma lista incompleta ou retirar julgamento contextual sem esclarecer necessidade, resultado e exceções.

### 4C

**Evidência:** a folha representa itens, motivos e estados; há revisão, categorias de resultado e limites humanos explícitos; nenhum computador é utilizado. **Inferência:** não se pode presumir que orçamento, restrições ou preferências estejam completos nem que toda substituição admita regra fixa. **Classificação escolhida:** formulação estruturada inicial executada manualmente; “resolução geral organizada com forte sobreposição” também é justificável quando apoiada em representação, estado, repetibilidade e verificação. A ausência de computador não elimina esses sinais. **Risco de automatização prematura:** recomendar compras ou substituições inadequadas a partir de informações familiares incompletas e reduzir o espaço do julgamento contextual.

## Modelos de entregas complementares

### Justificativa possível para 4C

A descrição 4C apresenta elementos de pensamento computacional sem programação porque explicita uma representação, distingue estados e prevê revisão. A evidência está nos campos da folha e nas categorias de resultado. A classificação não precisa ser absoluta: o processo continua cotidiano e inclui julgamentos humanos não reduzidos a regras. Por isso, “formulação estruturada inicial com elementos de pensamento computacional” é mais preciso que afirmar apenas “é pensamento computacional”. Também seria defensável falar em sobreposição com raciocínio organizado, desde que a ausência de computador não seja usada para negar os elementos observáveis.

### Contraexemplo possível

Uma pessoa copia para uma planilha um número recebido por mensagem e encaminha o arquivo porque essa foi a instrução. Ela usa computador e uma representação tabular, mas a descrição não mostra que tenha formulado o problema, compreendido o dado, escolhido o procedimento ou verificado o resultado. O processo mais amplo pode ter sido estruturado por outra pessoa; o simples uso da planilha não demonstra isso.

### Melhoria possível para 1A

> A necessidade declarada é reduzir episódios em que produtos necessários não estão disponíveis nos centros de distribuição. Antes de escolher uma solução, a equipe precisa esclarecer quais produtos, centros e períodos pertencem ao escopo; o que será considerado falta; quais informações sobre estoque existem e quando são atualizadas; quais movimentos ainda não foram concluídos; quem decide sobre reposição; e que evidência permitiria observar melhora. Esses pontos são perguntas abertas. A descrição não define uma regra de reposição nem determina que o processo deva ser automatizado.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| Clareza | resposta vaga ou circular | comunica a análise | usa termos com precisão e concisão |
| Distinções | equipara ferramenta, automação e pensamento computacional | distingue conceitos principais | reconhece sobreposições sem apagar diferenças |
| Justificativa | rotula sem evidência | cita elementos do texto | separa evidência, inferência e escolha |
| Lacunas | preenche o não informado | identifica ausências relevantes | explica por que impedem verificar ou decidir |
| Integridade | inventa regra, dado ou ferramenta | marca o que falta | transforma lacunas em perguntas |
| Limites | trata automação como correta ou neutra | identifica risco pertinente | relaciona risco a objetivo, dado, pessoa ou responsabilidade |

Uma resposta alternativa é válida quando sustenta a classificação no texto, explicita critérios, reconhece limites, não transforma inferência em fato e não exige computador para reconhecer estrutura. Depois de comparar, revise duas células da sua tabela e registre por que mudaram. Copiar a solução sem justificar a revisão não produz nova evidência de domínio.
