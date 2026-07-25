# Prática 06 — Representar, converter e auditar

## Objetivo e modalidades

Representar o mesmo procedimento organizacional em formas diferentes, escolher principal e complementar, converter e auditar perdas, ambiguidades e divergências.

Na trilha essencial, produza texto estruturado, tabela, diagrama simples e uma complementar entre mini tabela de decisão, mini modelo de estado ou pseudocódigo. Faça conversão, rastreabilidade, mudança e revisão. Tempo: 3h–4h.

No aprofundamento opcional, produza todas as complementares, segunda conversão, acessibilidade ampliada, três versões e transferência. Não é requisito para avançar.

## Bloco 1 — Necessidade de representação

Registre pergunta, propósito, público, decisão apoiada, conteúdo indispensável, conteúdo complementar, riscos e frequência de atualização.

| Dimensão | Declaração |
|---|---|
| pergunta |  |
| propósito |  |
| público |  |
| decisão apoiada |  |
| indispensável |  |
| complementar |  |
| riscos |  |
| atualização |  |

## Bloco 2 — Fonte numerada

O conteúdo abaixo é hipotético e constitui a fonte inicial:

- **E1 — fato:** cada ocorrência não atendida possui identificador, centro e produto.
- **E2 — estado informacional:** histórico pode ser completo, incompleto ou desconhecido.
- **E3 — regra:** desconhecido não pode ser convertido em incompleto.
- **E4 — classificação:** ocorrência pode pertencer a várias classes analíticas.
- **E5 — estado informacional:** classificação pode permanecer pendente.
- **E6 — evidência:** classificação registra a evidência usada e a ausente.
- **E7 — regra revisável:** impacto elevado exige proteção, sem provar causa.
- **E8 — autoridade:** decisão de encaminhamento depende de responsável autorizado.
- **E9 — exceção:** se houver risco imediato previamente definido, a autoridade pode priorizar antes de completar histórico, registrando justificativa.
- **E10 — encaminhamento:** evidência insuficiente orienta obtenção de informação, não conclusão negativa.
- **E11 — revisão:** nova evidência pode alterar classe e encaminhamento.
- **E12 — proteção:** custo, perda, divergência e transferência permanecem visíveis.
- **E13 — limite:** o procedimento não escolhe tecnologia nem intervenção.

Marque fato, regra, hipótese, desconhecido, decisão, exceção e limite. Não invente o que a fonte não informa.

Antes de representar, faça duas leituras. Na primeira, apenas sublinhe termos repetidos e relações explícitas. Na segunda, escreva ao lado de cada elemento: “o que afirma”, “o que não afirma” e “que outro elemento limita sua interpretação”. Por exemplo, E7 afirma uma exigência de proteção sob impacto elevado, mas não afirma causa nem autoriza encaminhamento automático; E8 limita qualquer leitura automática. E9 é exceção condicionada e ainda preserva autoridade e justificativa.

Crie uma pequena lista de termos controlados. Pelo menos “ocorrência”, “histórico”, “classe analítica”, “estado informacional”, “evidência”, “proteção”, “autoridade” e “encaminhamento” devem manter o mesmo sentido nas formas produzidas. Se usar sinônimo, registre a equivalência. Se perceber que dois termos pareciam sinônimos e não são, corrija antes da conversão.

Registre também perguntas que a fonte não responde: quem ocupa a autoridade, como impacto elevado é medido, quais proteções existem, qual evidência basta e quando o procedimento termina. Essas perguntas permanecem pendências. Elas não impedem representar o conteúdo disponível, mas impedem apresentar o pacote como procedimento operacional completo.

## Bloco 3 — Texto estruturado

Produza título, escopo, termos, regras, responsabilidades, desconhecidos, exceção, resultado e limite. Use IDs para ligar trechos à fonte. Não use parágrafo único e não transforme itens simultâneos em sequência.

Checklist:

- “desconhecido” permanece distinto de “incompleto”?
- classe analítica difere de estado informacional?
- autoridade e justificativa aparecem?
- proteção e limite foram preservados?

Use uma estrutura mínima como referência, sem copiá-la mecanicamente:

1. finalidade e recorte;
2. definições locais;
3. fatos e estados informacionais;
4. regras e classificações;
5. responsabilidade e exceção;
6. revisão, proteção e limite;
7. pendências.

Cada afirmação importante deve trazer um ou mais IDs E1–E13. Um mesmo ID pode aparecer em trechos distintos quando o texto apresenta a regra e depois seu limite. Depois de escrever, leia apenas os títulos e a primeira frase de cada item: eles devem permitir localizar a informação sem depender de leitura integral.

Faça ainda um teste de negação. Pergunte se o texto permitiria concluir “desconhecido é incompleto”, “uma classe determina causa” ou “o encaminhamento é automático”. Se permitir, mesmo sem dizer isso literalmente, acrescente limite ou reorganize a frase. A representação também é responsável pelas inferências previsíveis que sua forma favorece.

## Bloco 4 — Tabela

Escolha uma finalidade: elementos/responsabilidades, condições/encaminhamentos, rastreabilidade ou estados informacionais.

| ID da linha | Unidade | Condição ou atributo | Estado informacional | Encaminhamento | Origem |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

Use explicitamente desconhecido, não aplicável, ausência confirmada e pendente. Não use vazio.

Antes de preencher, complete: “cada linha representa ______”. Não misture ocorrência individual com regra geral. Se a tabela escolhida for de condições e encaminhamentos, use uma linha por condição identificada e indique quando o resultado depende de autoridade. Se for de elementos e responsabilidades, não force E1–E13 a caber em colunas de caso.

Inclua legenda dos valores especiais. “Desconhecido” significa informação atualmente indisponível; “não aplicável” significa dimensão fora do caso conforme critério; “ausência confirmada” indica verificação negativa; “pendente” indica trabalho ou decisão ainda aberto. Esses rótulos não são intercambiáveis. Caso a fonte não ofereça exemplo legítimo de algum valor, registre-o na legenda sem atribuí-lo a uma ocorrência inventada.

Revise a ordenação. Se ordenar por impacto, declare que a ordem é apenas para leitura, ou justifique a prioridade por E7 e E9 sem ultrapassar E8. Verifique se destaque, cor ou posição sugerem conclusão não autorizada. Acrescente descrição textual para qualquer distinção visual relevante.

## Bloco 5 — Diagrama simples

Escolha elementos, significado das caixas, relações, direção e legenda. Pode usar tabela:

| Origem | Relação | Destino | ID da fonte |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

Inclua descrição textual equivalente. Se desenhar setas, cada tipo precisa de significado. Não use seta como causa.

O desenho pode ser feito à mão ou com recurso digital, mas a entrega textual equivalente é obrigatória. Antes de desenhar, produza pelo menos seis relações na tabela preparatória. Use verbos específicos como “possui”, “pode receber”, “é sustentada por”, “é registrada por” ou “orienta”. Evite “relaciona-se com” quando a fonte permite precisão maior.

Defina a fronteira: o diagrama descreve informação, responsabilidade ou procedimento? Não misture atividade, estado e pessoa com a mesma aparência sem legenda. Se um elemento externo for necessário, marque-o como externo ao recorte. Depois, leia cada seta como uma frase completa e confronte-a com o ID da fonte.

Faça o teste de acessibilidade sem cor e sem posição. Imagine que as relações sejam lidas numa lista linear. Os rótulos ainda permitem reconstruir o significado? Se não, a forma depende de pista visual não declarada. Corrija a legenda ou a descrição.

## Bloco 6 — Principal e complementar

| Critério | Principal | Complementar |
|---|---|---|
| finalidade |  |  |
| público |  |  |
| força |  |  |
| perda |  |  |
| atualização |  |  |
| risco |  |  |
| uso proibido |  |  |

Explique por que uma forma sozinha não basta e como a segunda cobre perda real.

Escreva uma justificativa de 150 a 250 palavras. Ela deve mencionar a pergunta do Bloco 1, uma força e uma perda concretas da principal, uma força complementar, o público, a frequência de atualização e um uso proibido de cada forma. “A tabela é mais organizada” não basta; diga qual comparação ela torna possível e qual contexto comprime.

Defina também a autoridade de referência: quando houver divergência, qual artefato deve ser consultado para a regra, qual para a origem e qual para relações? Isso não transforma um artefato em verdade absoluta; apenas evita que uma inconsistência seja resolvida por preferência visual.

## Bloco 7 — Conversão

Escolha texto → tabela, tabela → diagrama ou diagrama → texto. Quando viável, faça a primeira tentativa sem consultar a origem. Depois compare:

| Item | Registro |
|---|---|
| preservado |  |
| perdido |  |
| acrescentado |  |
| ambíguo |  |
| incompatível |  |

Elemento acrescentado sem origem exige justificativa ou remoção.

Faça a conversão em uma cópia identificada, preservando a primeira versão. Numere os elementos do destino como T1, L1 ou D1, conforme texto, linha ou relação. Para cada diferença, cite IDs de origem e destino. Não registre apenas “perdeu detalhe”; escreva qual detalhe, por que desapareceu e que risco resulta.

Depois da comparação, classifique cada diferença:

- **corrigir agora**, quando contradiz ou omite conteúdo essencial;
- **justificar**, quando a seleção atende ao propósito e outra forma preserva o conteúdo;
- **manter pendente**, quando a fonte é insuficiente;
- **remover**, quando houve invenção.

Se a primeira conversão tiver preservado tudo, procure especialmente responsabilidade, exceção, limites e estatutos do conhecimento. Uma conversão perfeita é possível em recorte pequeno, mas uma auditoria sem nenhuma observação pode indicar leitura superficial.

## Bloco 8 — Rastreabilidade

| Origem | Texto | Tabela | Diagrama | Situação |
|---|---|---|---|---|
| E1 |  |  |  |  |
| E2 |  |  |  |  |
| E3 |  |  |  |  |
| E4 |  |  |  |  |
| E5 |  |  |  |  |
| E6 |  |  |  |  |
| E7 |  |  |  |  |
| E8 |  |  |  |  |
| E9 |  |  |  |  |
| E10 |  |  |  |  |
| E11 |  |  |  |  |
| E12 |  |  |  |  |
| E13 |  |  |  |  |

Todo elemento essencial aparece em ao menos uma forma. Cobertura não prova qualidade semântica.

Preencha a matriz com identificadores específicos, não apenas “sim”. Use, por exemplo, T3, L2 e D4. Na coluna situação, marque preservado, parcial, omitido com justificativa, incompatível ou pendente. Um elemento pode ser deliberadamente omitido do diagrama e preservado no texto; isso é aceitável se a escolha estiver explícita e não comprometer o uso do diagrama.

Faça duas varreduras. Na primeira, percorra E1–E13 e encontre destinos. Na segunda, percorra todos os itens criados e encontre origem. A segunda detecta informação inventada que uma matriz orientada apenas pela fonte não mostra. Registre elementos do destino sem origem numa lista de “órfãos” e resolva-os.

Selecione três vínculos e confira o significado palavra por palavra. A mera presença de E3 ao lado de uma linha que iguala desconhecido e incompleto não representa cobertura correta; representa incompatibilidade rastreada. Corrija o conteúdo e só então altere a situação.

## Bloco 9 — Uma representação complementar

Escolha apenas uma no essencial.

### Mini tabela de decisão

Use até três condições, resultados e combinação ausente. Não faça tabela-verdade.

### Mini modelo de estado

Use até quatro estados, eventos e transições. Não faça rastreamento. Estado não é atividade.

### Pseudocódigo introdutório

Represente procedimento fornecido em notação não executável e independente de linguagem. Não tente provar algoritmo.

Justifique por que a escolhida cobre limite da principal.

Se escolher tabela de decisão, declare as condições, resultados e pelo menos uma combinação que a fonte não resolve. Não complete essa combinação por intuição. Se escolher modelo de estado, use substantivos ou expressões de condição para estados e verbos/eventos para transições; explique por que “classificar ocorrência” é atividade e “classificação pendente” pode ser estado. Se escolher pseudocódigo, mantenha termos do glossário, declare o início do recorte e marque qualquer condição externa como referência ou pendência.

Compare a complementar com texto, tabela e diagrama já produzidos. Localize pelo menos um ganho e uma nova perda. A complementar não está dispensada de rastreabilidade: acrescente uma coluna à matriz ou crie tabela separada com E1–E13 e seus elementos.

## Bloco 10 — Mudança controlada

Nova informação: **histórico desconhecido exige registro separado e não pode compartilhar o mesmo encaminhamento de histórico incompleto sem decisão explícita da autoridade**.

Identifique artefatos afetados, crie nova versão, atualize rastreabilidade e registre impacto:

| Artefato | Versão anterior | Mudança | Nova versão | Vínculos afetados |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |

## Bloco 11 — Auditoria final

Verifique: elemento perdido; informação inventada; seta sem significado; vazio ambíguo; regra divergente; estado nomeado como ação; ordem inventada; versão desatualizada; dependência exclusiva de cor; incompatibilidade entre principal e complementar.

Registre ao menos uma correção realizada após a auditoria.

Realize a auditoria em três passagens. Na primeira, confira conteúdo e limites. Na segunda, confira convenções, acessibilidade e legibilidade. Na terceira, confira versões e vínculos. Para cada problema, registre evidência, risco, correção e artefato afetado.

Troque temporariamente os artefatos com outra pessoa, se houver parceria disponível, sem explicar as convenções oralmente. Peça que ela responda à pergunta do Bloco 1 e indique uma inferência que considerou possível. Se estiver trabalhando sozinho, aguarde alguns minutos, leia na ordem complementar → diagrama → tabela → texto e anote onde precisou adivinhar. A necessidade de explicação externa mostra que algo deve entrar na própria entrega.

Finalize com uma declaração curta de limites: o que o pacote permite interpretar, o que não permite decidir e quais pendências impedem uso operacional. Essa declaração é parte da qualidade, não uma admissão de fracasso.

## Entrega esperada

Entregue propósito/público, análise da fonte, texto, tabela, diagrama, escolhas, uma complementar, conversão, matriz, auditoria, versões revistas e autoavaliação.

Organize os arquivos ou seções nesta ordem e dê a cada um título e versão. Não apague a versão anterior após o Bloco 10: mantenha-a como evidência da mudança. A entrega essencial deve conter:

- folha de propósito, público e convenções;
- fonte E1–E13 anotada e lista de pendências;
- texto estruturado identificado;
- tabela com legenda de valores;
- diagrama e descrição textual;
- justificativa de principal e complementar;
- registro de conversão e diferenças;
- matriz de rastreabilidade nos dois sentidos;
- complementar escolhida;
- registro de mudança, auditoria e autocorreção.

Antes de consultar a solução, escreva em cinco linhas o que a sua principal mostra melhor, o que ela perde, como a complementar ajuda, qual divergência foi corrigida e qual limitação permanece.

## Solução comentada — consulte somente depois da tentativa

Não existe pacote único. Para público operacional, tabela de condições pode ser principal e texto estruturado complementar; para auditoria, matriz de rastreabilidade pode ser principal. A justificativa deve partir da pergunta.

Conversão parcial possível:

| Origem | Linha tabular possível | Perda possível |
|---|---|---|
| E2 | histórico: completo/incompleto/desconhecido | justificativa de cada estado |
| E7 | impacto elevado: proteção exigida | ausência de causalidade pode sumir |
| E9 | risco imediato: priorização autorizada | autoridade e justificativa podem sumir |

Acrescentar “encaminhar automaticamente” seria indevido: E8 mantém autoridade. Converter desconhecido em incompleto contradiz E3. O diagrama de relações pode perder E12 se proteções não virarem elemento ou anotação.

Após a mudança do Bloco 10, texto, tabela, complementar escolhida e matriz podem ser afetados. Atualize apenas os artefatos que contêm ou dependem da regra, mas registre os demais como conferidos. Uma versão nova sem vínculo atualizado continua inconsistente.

Deixe suas células originais. Compare significado, não aparência, e defenda alternativa coerente.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| propósito/público | ausentes | declarados | orientam escolhas |
| adequação | escolhe por hábito | responde à pergunta | limita usos |
| conteúdo | inventa ou perde | preserva núcleo | distingue estatutos |
| convenção | implícita | possui legenda | significado estável |
| legibilidade | exige adivinhação | leitura possível | adequada ao público |
| precisão | termos vagos | termos definidos | desconhecidos explícitos |
| ambiguidade | ignorada | localizada | corrigida ou limitada |
| complemento | repete | cobre perda | relação justificada |
| conversão | copia forma | reconstrói significado | audita mudanças |
| cobertura | deixa essenciais | cobre origem | não confunde com qualidade |
| rastreabilidade | só numera | cria vínculos | detecta órfãos |
| consistência | formas contradizem | compatíveis | divergências resolvidas |
| perdas | invisíveis | registradas | risco avaliado |
| acessibilidade | depende de cor | possui alternativa | público considerado |
| atualização | altera um artefato | identifica afetados | atualiza vínculos |
| revisão | copia solução | muda por evidência | registra impacto |
| limites | universaliza | declara uso proibido | mantém fronteira |

O essencial termina quando nenhum critério está em “precisa de revisão” e você explica o que cada forma mostra, perde e como E1–E13 permanecem rastreáveis.

## Carga

- Prática essencial: 3h–4h.
- Solução, revisão e autoavaliação: 30–45 min.
- Aprofundamento opcional: 3h–5h adicionais.
- Trilha integrada: 7h30–9h45.
- Percurso completo opcional: 12h–16h.
