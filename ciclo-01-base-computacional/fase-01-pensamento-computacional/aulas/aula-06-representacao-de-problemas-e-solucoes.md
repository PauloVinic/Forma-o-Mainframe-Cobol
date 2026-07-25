# Aula 06 — Representação de problemas e soluções

## Metadados e objetivo

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo:** De problemas informais a soluções estruturadas
- **Posição:** sexta de 14 aulas
- **Competência:** C06 — Selecionar representações
- **Níveis:** Nível 2 — explicação; Nível 3 — construção e conversão guiadas; início do Nível 4 em caso simples
- **Pré-requisitos:** problema formulado, decomposição, modelo, propósito, público, atributos, classes, regras, exceções e domínio
- **Prática associada:** [Prática 06 — Representar, converter e auditar](../praticas/pratica-06-representando-o-mesmo-procedimento.md)
- **Projeto integrado:** conclusão do P2 com pacote de representações coerentes, rastreáveis e revisáveis

Ao concluir, o aluno deverá escolher uma representação principal e uma complementar; justificar as escolhas; construir texto estruturado e uma segunda forma entre tabela e diagrama simples; analisar a terceira forma básica; interpretar fluxograma, tabela de decisão, modelo de estado e pseudocódigo introdutórios; converter formas; localizar perdas e acréscimos; verificar consistência; construir rastreabilidade; e revisar versões após mudança.

C06 é essencial, mas esta aula inicia o Nível 4 apenas em problemas e procedimentos simples já compreendidos. Representações complexas exigirão prática posterior e conhecimento do domínio.

## Introdução: conteúdo compreendido ainda precisa ser comunicado

As aulas anteriores produziram problema, partes, dependências, modelos, atributos, classes, padrões, regras e limites. Esse conteúdo pode continuar difícil de comparar, verificar, atualizar e comunicar. Uma regra escondida num parágrafo, tabela sem colunas definidas, seta sem legenda, fluxo que inventa ordem, pseudocódigo que omite exceção ou dois artefatos com nomes diferentes criam novas falhas.

Representação não corrige conteúdo defeituoso. Diagrama não salva decomposição arbitrária; tabela não torna modelo adequado; pseudocódigo não elimina regra ambígua; aparência não cria significado. Conteúdo precisa existir antes da conversão, embora representar possa revelar lacuna e levar à revisão do conteúdo.

A Aula 05 produziu classes, regras, condições, contraexemplos e domínio. Agora perguntaremos que forma os torna examináveis para determinado público, que informação precisa ficar visível, que forma complementar cobre perdas e como manter coerência entre artefatos.

## Fundamentos da representação

### Definição operacional

Adotaremos:

> **Representação é uma forma organizada e convencional de expressar aspectos selecionados de um conteúdo ou modelo, para que determinado público possa interpretá-los, verificá-los, comunicá-los, convertê-los ou revisá-los dentro de propósito e limites declarados.**

Representação expressa conteúdo, não é o conteúdo. Usa convenções, seleciona e omite, pode perder ou acrescentar informação, pode ser convertida e deve ser revisada quando conteúdo ou uso mudam.

### Conteúdo, modelo e representação

Conteúdo é aquilo que se pretende comunicar: problema, regra, relação, estado, procedimento, evidência ou classificação. Modelo organiza seletivamente aspectos e relações para finalidade. Representação é a forma examinável pela qual conteúdo ou modelo se manifesta.

O mesmo modelo pode ter texto e tabela. A mesma estrutura tabular pode materializar modelos diferentes conforme população e significado das colunas. Trocar texto por tabela não muda necessariamente o modelo; remover exceção ou alterar relação muda o conteúdo representado. Uma forma nova pode revelar que o modelo era ambíguo, sem se confundir com ele.

### Representação, notação e convenção

Representação é o artefato concreto. Notação é um sistema de símbolos e regras de escrita. Convenção é acordo sobre interpretação. Uma seta pode significar sequência, dependência, envio, influência ou transição. Sem legenda, direção e tipo de relação, o leitor pode inventar significado.

Notações profissionais não são universais para toda pergunta. Nesta aula, convenções mínimas e declaradas valem mais que memorização extensa de símbolos.

### Sintaxe e significado

Sintaxe é a forma permitida; significado — ou semântica, em uso introdutório — é o que a forma expressa. Uma tabela pode estar alinhada e semanticamente errada; um fluxograma pode usar formas consistentes e omitir exceção; pseudocódigo pode parecer organizado e representar regra incorreta.

Não aprofundaremos linguagens formais. A distinção serve para lembrar que correção visual não garante correção do conteúdo.

## Critérios para escolher e combinar

Antes de escolher, declare pergunta, propósito, público, decisão apoiada, conteúdo indispensável, nível, atualização, necessidade de comparação, ordem, estados, combinações, rastreabilidade e risco de uso indevido.

**Adequação** pergunta se a forma ajuda a responder. **Legibilidade** considera o esforço do público. **Precisão** reduz interpretações incompatíveis. **Verificabilidade** permite conferir elementos e relações. **Rastreabilidade** liga origem, artefatos e revisões. **Manutenibilidade** permite incorporar mudanças. **Economia** evita complexidade sem função. **Acessibilidade** evita depender apenas de cor, posição ou imagem. **Complementaridade** busca segunda forma que cubra limitações da primeira.

Não há fórmula numérica universal. Uma tabela pode ser precisa para comparação e fraca para contexto; texto pode explicar exceções e esconder cobertura. A escolha é argumentada por critérios.

Representação principal é a referência mais adequada ao uso prioritário, não o artefato que contém tudo. Complementar destaca conteúdo que a principal esconde. Se ambas repetem exatamente a mesma força e perda, a segunda pode ser ornamentação.

### Uma seleção orientada por perguntas

O primeiro erro de seleção costuma ocorrer antes de qualquer desenho: escolher a forma porque ela está disponível ou parece profissional. Uma planilha aberta convida à tabela; uma ferramenta gráfica convida ao diagrama. A ordem deveria ser inversa. Primeiro se determina o que alguém precisa descobrir, comparar, decidir ou revisar; só então se escolhe a forma. A pergunta “quais condições levam a cada resultado?” favorece uma tabela de decisão pequena. “Que relações ligam as entidades?” favorece um diagrama de relações. “Por que a exceção existe?” provavelmente exige texto. “Em que condição o caso se encontra e o que pode fazê-lo mudar?” sugere um modelo de estado.

Por fim, complementaridade é avaliada pela diferença de capacidades. Texto e tabela podem compartilhar o mesmo conteúdo, mas desempenhar papéis diferentes: o texto preserva motivos e exceções; a tabela expõe padrões e lacunas. Um diagrama complementar pode mostrar dependências que ficam dispersas nas linhas. A combinação se justifica quando o ganho compensa o custo de manter coerência e versões. Criar muitas formas sem responsáveis por atualização aumenta, e não reduz, o risco.

## Linguagem natural e listas estruturadas

### Linguagem natural

Linguagem natural oferece contexto, nuance, justificativa e exceções. Também traz ambiguidade lexical, sujeito oculto, ordem implícita, condição vaga e escopo incerto.

Compare “Quando necessário, o caso deve ser analisado e encaminhado” com:

- a equipe de análise examina ocorrências com evidência insuficiente;
- usa os registros disponíveis e marca desconhecidos;
- encaminha à autoridade indicada quando a decisão excede sua responsabilidade;
- mantém pendente o que não pode concluir.

A segunda forma não é perfeita, mas revela agente, condição, evidência, destino e pendência.

### Texto estruturado

Títulos, identificadores, frases curtas, termos definidos, condições separadas, exceções próximas da regra e referências cruzadas tornam o texto verificável. Cada item deve possuir escopo claro. Lista não implica sequência: bullets podem representar propriedades simultâneas.

Lista hierárquica distingue item principal e subitem, mas recuo visual precisa corresponder a relação semântica. Misturar regra, exemplo e consequência no mesmo nível gera falsa equivalência. Numeração pode identificar elementos sem afirmar ordem, desde que a convenção seja declarada.

## Tabelas e matrizes

Tabelas favorecem comparação, classificação, cobertura, relações entre dimensões, condições e rastreabilidade. Linhas e colunas devem responder à unidade e à pergunta. Misturar casos e totais na mesma coluna, juntar valores incompatíveis ou repetir parágrafos em células reduz utilidade.

Célula vazia é perigosa. Pode significar desconhecido, não aplicável, não coletado, omitido, zero ou ausência confirmada. Use rótulos explícitos. “Não” significa ausência confirmada conforme critério; “desconhecido” significa impossibilidade atual de concluir.

Uma tabela de casos põe unidades nas linhas e atributos nas colunas. Uma tabela comparativa coloca alternativas ou modelos em linhas. Matriz de rastreabilidade cruza origem e artefato. Tabela de regras explicita condição, conclusão e limite. A estrutura deve nascer da pergunta, não do hábito.

Precisão tabular não é validade. Colunas bem alinhadas podem usar definições divergentes. Uma tabela pode ocultar narrativa, responsabilidade ou exceção; texto complementar pode preservá-las.

### Como projetar uma tabela examinável

Antes de preencher células, escreva uma frase: “cada linha representa...” e outra: “cada coluna informa...”. Se não for possível completar essas frases sem usar “depende”, provavelmente há mais de uma unidade misturada. Em uma tabela de ocorrências, cada linha pode ser uma ocorrência. Em uma tabela de regras, cada linha pode ser uma regra. Colocar a ocorrência e a regra como se fossem unidades equivalentes produz comparações sem sentido.

As colunas devem usar domínios coerentes. Se “estado do histórico” aceita completo, incompleto ou desconhecido, uma célula com “urgente” pertence a outra dimensão. Cabeçalhos como “observações” frequentemente se tornam depósito de exceções, decisões e justificativas. Quando esses conteúdos importam, merecem colunas definidas ou referência a texto identificado. Isso torna a omissão visível e facilita revisão.

Agregações também precisam de declaração. Uma linha “total” não é um caso individual. Percentual exige denominador, recorte temporal e tratamento de desconhecidos. Mesmo sem calcular nesta aula, deve-se perguntar se valores ausentes foram excluídos, agrupados ou interpretados como zero. A representação pode induzir conclusão falsa sem conter número aritmeticamente errado.

Considere a pequena fonte: “o registro A tem histórico completo; o registro B ainda não foi consultado; para C, histórico não se aplica”. Uma tabela que deixe B e C vazios perde a diferença. Uma tabela melhor escreve “completo”, “não coletado” e “não aplicável”. Se a fonte afirmar que A não teve ocorrência anterior, “ausência confirmada” é diferente de “zero” quando a coluna não mede quantidade. O rótulo precisa corresponder à pergunta.

Linhas, colunas e ordenação também expressam escolhas. Ordenar por impacto pode sugerir prioridade, mesmo quando a regra não autoriza isso. Destacar uma linha pode sugerir exceção. Mesclar células pode esconder que um valor não foi registrado individualmente. Toda escolha visual importante deve ser compatível com o conteúdo e, quando puder alterar interpretação, declarada.

## Diagramas e fluxogramas

### Diagramas de relações

Diagrama é representação visual ou espacial de elementos e relações. Para ser examinável, declare elementos, tipo de relação, direção, significado de seta, fronteira, legenda e nível.

Uma tabela de relações pode preparar desenho:

| Origem | Relação | Destino | Significado |
|---|---|---|---|
| ocorrência | refere-se a | produto | associação de registro |
| ocorrência | ocorreu em | centro | localização |
| evidência | sustenta ou limita | análise | relação epistêmica, não causa |
| autoridade | registra | decisão | responsabilidade |

Seta não significa causa automaticamente. Relação “evidência → análise” precisa de legenda; sem ela pode parecer sequência, envio ou produção.

### Fluxogramas introdutórios

Fluxograma evidencia ordem, alternativas e retornos de procedimento já compreendido. Nesta aula, use conjunto mínimo: início/fim, atividade, decisão e direção. O significado importa mais que forma decorativa.

Fluxo não é diagrama geral de relações. Se “produto está associado a centro”, não há necessariamente atividade ou ordem. Representar como fluxo inventaria sequência. Uma decisão deve formular pergunta e mostrar saídas rotuladas; seta sem condição transfere ambiguidade.

Não ensinaremos catálogo completo, prova de término ou correção algorítmica. Fluxograma mostra uma leitura do procedimento e pode omitir simultaneidade, responsabilidade ou justificativa.

### Leitura crítica de diagramas

Para ler um diagrama, não comece seguindo setas. Comece pela legenda, fronteira e tipos de elementos. Pergunte o que cada caixa representa: pessoa, informação, evento, atividade, estado ou unidade organizacional. Em seguida, pergunte se todas as setas têm o mesmo significado. Se uma seta significa “possui” e outra “envia”, a diferença precisa aparecer no rótulo ou no estilo acompanhado de legenda acessível.

A posição espacial pode enganar. Elementos próximos parecem relacionados; elementos no alto parecem superiores; a direção da esquerda para a direita parece temporal. Essas leituras são convenções culturais e não fatos do domínio. Se posição não tiver significado, o artefato pode declarar isso. Se tiver, deve explicá-lo. Cor, espessura e forma também nunca devem ser a única maneira de distinguir uma relação importante.

Uma fronteira informa o que está dentro do recorte, não o que inexiste no mundo. Ao desenhar apenas “ocorrência”, “evidência” e “análise”, não se conclui que pessoas ou sistemas não participam. O título e a nota de escopo impedem que uma seleção didática pareça descrição completa. Da mesma forma, uma seta ausente pode significar relação inexistente, relação desconhecida ou apenas relação omitida. A convenção deve diferenciar esses casos quando forem relevantes.

Na revisão, escolha um caminho e traduza-o em frase. Se o desenho mostra “autoridade — registra → decisão”, leia: “a autoridade registra a decisão”. Depois compare com a fonte. Se a frase vira “a autoridade produz a decisão”, o rótulo ou a direção estão inadequados. Faça também o caminho inverso: selecione uma afirmação essencial da fonte e localize caixas e relação correspondentes. Essa dupla leitura aproxima diagrama e rastreabilidade.

Fluxogramas precisam de cuidado adicional. Uma atividade deve dizer o que ocorre, uma decisão deve conter pergunta verificável e cada saída deve indicar a resposta. “Analisar” seguido de losango “resultado” não informa a condição. Um retorno deve ter motivo e destino claros. Um fluxo que termina sem mostrar pendência pode sugerir que todos os casos são concluídos. Ainda assim, incluir todos os detalhes transforma o desenho em labirinto; informações de responsabilidade e justificativa podem permanecer em tabela ou texto complementar, ligadas por IDs.

## Tabela de decisão e modelo de estado

### Tabela de decisão introdutória

Tabela de decisão organiza poucas condições e resultados. O quadro seguinte é um **exemplo didático hipotético**, construído com regras fornecidas apenas para analisar a representação. Ele não registra regra confirmada do projeto de estoque nem autoriza ação automática:

| Histórico | Impacto | Encaminhamento representado |
|---|---|---|
| completo | baixo | registrar análise |
| incompleto | qualquer | obter evidência |
| desconhecido | qualquer | manter pendente |
| completo | elevado | submeter à autoridade |

“Qualquer” significa, somente neste exemplo, que o valor do impacto não altera o encaminhamento representado naquela linha. A combinação “histórico completo e impacto não classificado” continua ausente. As condições não são completas, a tabela não é tabela-verdade, não prova cobertura e não cria regra a partir de taxas ou padrões da Aula 05. Todo encaminhamento permanece sujeito à regra externa e à autoridade decisória competente.

### Modelo de estado introdutório

Estado é condição relevante; evento é ocorrência que pode provocar mudança; transição liga estado de origem e destino sob evento ou condição. “Aguardar evidência” pode ser atividade; “evidência pendente”, estado. Confundi-los prejudica leitura.

Modelo textual simples:

| Estado de origem | Evento ou condição | Estado de destino |
|---|---|---|
| registrado | evidência insuficiente reconhecida | evidência pendente |
| evidência pendente | evidência recebida | pronto para análise |
| pronto para análise | decisão registrada | encerrado no recorte |

Isso não é rastreamento de execução. Não estudaremos variáveis, invariantes ou sequências completas; a Aula 08 aprofundará estados.

## Pseudocódigo como representação

Pseudocódigo é notação textual estruturada para expressar procedimento sem exigir sintaxe de linguagem executável. Pode revelar estrutura e responsabilidade abstrata. Deve ser legível, consistente e independente de linguagem.

Um exemplo introdutório, apresentado como texto e não como programa:

> RECEBER uma ocorrência selecionada<br>
> IDENTIFICAR o estado informado do histórico<br>
> SE o histórico estiver desconhecido<br>
> &nbsp;&nbsp;REGISTRAR pendência<br>
> CASO CONTRÁRIO<br>
> &nbsp;&nbsp;REGISTRAR a classificação sustentada<br>
> ENCERRAR o recorte representado

O trecho representa um procedimento; não prova correção, completude ou término algorítmico. “Selecionada” e “classificação sustentada” dependem de definições. A Aula 07 definirá algoritmo, a Aula 09 aprofundará decisões e a Aula 10 tratará repetição; este exemplo não ensina essas construções integralmente.

Pseudocódigo não é código simplificado, não executa e não deve imitar Java, Python, JavaScript, COBOL ou outra sintaxe. Linguagem natural vaga não vira precisão só por usar maiúsculas e recuo.

> **Nem todo texto em pseudocódigo constitui um algoritmo adequado.**

A Aula 07 definirá algoritmo, entrada, saída, efetividade e término. Aqui avaliamos a representação, não domínio algorítmico.

### Como avaliar pseudocódigo sem executá-lo

O leitor deve conseguir reconhecer o início e o fim do recorte, as unidades tratadas, as condições e os resultados representados. Termos devem permanecer estáveis. Se “ocorrência”, “caso” e “registro” forem usados para a mesma unidade, essa equivalência precisa ser declarada; se forem unidades diferentes, a troca é erro. Recuo e marcadores indicam estrutura, mas não substituem palavras que expliquem condição e finalidade.

Uma condição examinável precisa permitir ao leitor saber que informação seria consultada. “Se estiver adequado” é fraco sem critério. “Se o histórico estiver desconhecido” é mais claro, desde que “desconhecido” já tenha definição. Uma ação como “resolver o caso” pode esconder várias responsabilidades e resultados. Nesta fase, vale decompor apenas o necessário para que o procedimento fornecido seja interpretável, sem tentar construir uma solução executável.

Uma condição externa também exige limite conceitual. “Ocorrência selecionada” deixa aberta a regra de seleção. Isso pode ser aceitável se a seleção estiver fora do recorte e a referência estiver registrada. Se for essencial ao resultado, a omissão precisa virar pendência. Uma representação honesta torna o desconhecido visível; não inventa uma condição só para parecer completa.

Ao comparar pseudocódigo com fluxograma, procure equivalência sem exigir aparência idêntica. Uma decisão no fluxo pode corresponder a uma condição textual. Duas atividades consecutivas podem corresponder a dois enunciados. Uma nota de limite pode não aparecer dentro do fluxo e continuar preservada por vínculo ao texto complementar. Se o pseudocódigo acrescenta uma ordem que a fonte descrevia como simultânea, houve alteração semântica.

Também não se deve avaliar o trecho perguntando apenas se “parece código”. Palavras em maiúsculas, termos condicionais, alinhamento ou fechamento visual não asseguram entrada definida, saída, efetividade nem término. Essas propriedades pertencem à discussão de algoritmos da Aula 07. Aqui, o pseudocódigo é uma lente para enxergar a estrutura alegada de um procedimento e confrontá-la com sua fonte.

## Combinação, conversão, consistência e rastreabilidade

### Combinar formas

Texto explica contexto e exceções; tabela compara; diagrama destaca relações; fluxo evidencia ordem; tabela de decisão cruza condições; modelo de estado mostra condições; pseudocódigo estrutura procedimento. Combinação boa distribui responsabilidades sem fragmentar significado.

Represente o mesmo conceito com termo estável. Se texto usa “pendente”, tabela usa “incompleto” e diagrama usa “aguarda”, determine se são equivalentes ou distintos. Glossário local e identificadores ajudam.

### Conversão não é cópia

Converter exige reconstruir significado em outra forma. Texto para tabela exige escolher unidade e colunas. Tabela para diagrama exige escolher relações. Diagrama para texto exige explicitar convenções espaciais.

Audite:

- **preservado:** conteúdo com significado equivalente;
- **perdido:** conteúdo da origem ausente;
- **acrescentado:** conteúdo sem origem;
- **ambíguo:** permite interpretações incompatíveis;
- **incompatível:** contradiz a origem.

Acrescentar pode ser legítimo quando é convenção ou esclarecimento justificado. Inventar decisão para preencher lacuna não é.

### Consistência

Consistência interna é ausência de contradição dentro do artefato. Consistência entre representações significa compatibilidade semântica, não texto idêntico. Uma tabela pode agregar e o texto detalhar, desde que as diferenças sejam intencionais e rastreáveis.

Compare nomes, fronteiras, condições, exceções, estados, responsabilidades e resultados. Divergência deve ser resolvida na fonte ou registrada como pendência, não escondida por formatação.

### Rastreabilidade e matemática

Seja `O` o conjunto de elementos da origem e `R` o conjunto de elementos representados. A relação de rastreabilidade:

`T ⊆ O × R`

Um par `(o, r) ∈ T` registra que o elemento representado `r` deriva ou corresponde ao elemento `o`. A relação pode ser muitos para muitos: uma origem pode aparecer em várias formas, e um elemento representado pode sintetizar várias origens. Um vínculo não prova equivalência semântica.

Sem vínculo em um artefato específico pode haver omissão deliberada, desde que a complementar preserve o conteúdo e o uso da primeira esteja limitado. Sem vínculo em todo o pacote pode haver perda essencial. Elemento representado sem origem ou justificativa é **órfão**; convenção ou esclarecimento acrescentado e explicitamente justificado não é invenção. A cobertura é avaliada no pacote, não obrigatoriamente em cada forma isolada.

Cobertura não prova qualidade. Um vínculo pode existir e estar semanticamente errado. A matriz registra situação:

| Origem | Texto | Tabela | Diagrama | Situação |
|---|---|---|---|---|
| E1 | T1 | L1 | D1 | preservado |
| E2 | T2 | L2 | — | omitido do diagrama com justificativa |

Versionar significa identificar estado do artefato e mudança. Quando uma regra muda, localize representações dependentes, atualize versões, refaça vínculos e registre impacto.

### Um protocolo de conversão e revisão

Uma conversão segura pode ser organizada em seis movimentos. Primeiro, congele e identifique a origem: título, recorte e versão. Segundo, numere os elementos relevantes sem reescrevê-los silenciosamente. Terceiro, declare a pergunta que a nova forma responderá. Quarto, produza a representação e registre convenções. Quinto, percorra cada elemento da origem e cada elemento do destino nos dois sentidos. Sexto, classifique diferenças e decida corrigir, justificar ou manter como pendência.

A leitura da origem para o destino encontra perdas: para cada `o ∈ O`, procure ao menos um `r ∈ R` relacionado. A leitura do destino para a origem encontra acréscimos: para cada elemento representado, procure origem ou justificativa explícita. Não é necessário que a correspondência seja um para um. Um parágrafo pode alimentar várias linhas; várias afirmações podem ser sintetizadas numa relação, desde que a síntese não altere significado.

Uma matriz cheia de marcas não encerra a auditoria. O vínculo E7–T4, por exemplo, pode existir mesmo que T4 diga o contrário de E7. Por isso a situação registra “preservado”, “parcial”, “incompatível” ou “pendente”, acompanhada por nota quando necessário. O identificador cria caminho de inspeção; a revisão humana confere o sentido.

Considere uma mudança de fonte: antes, “histórico desconhecido orienta obtenção de evidência”; depois, “histórico desconhecido exige registro separado antes de qualquer encaminhamento, salvo decisão explícita”. O impacto alcança texto, linhas tabulares, possíveis estados, condições de decisão, fluxo e pseudocódigo. Um diagrama puramente estrutural talvez não mude, mas deve ser conferido. Registrar “conferido, sem impacto” é diferente de ignorá-lo.

Versão não precisa usar sistema complexo nesta aula. Basta identificador coerente, data ou ordem, descrição da mudança e ligação com a origem. O que não se deve fazer é substituir o artefato e apagar o motivo da alteração. Quando duas formas divergem, a mais bonita ou mais nova não vence automaticamente: retorna-se à fonte vigente, aos critérios e às pendências autorizadas.

Há ainda uma tensão entre manutenção e duplicação. Copiar uma regra completa em cinco artefatos aumenta o número de pontos sujeitos a divergência. Usar apenas referências pode tornar a leitura impossível. Uma solução equilibrada mantém a formulação normativa ou principal em um local identificado, repete apenas o necessário para a tarefa e cria vínculos. O pacote deve dizer qual artefato prevalece para cada finalidade, sem alegar que uma única forma substitui todas as demais.

## Caso progressivo do estoque e conclusão do P2

### Conteúdo de origem

Considere o conteúdo já sustentado: ocorrência não atendida possui identificador, centro e produto; histórico pode ser completo, incompleto ou desconhecido; classes analíticas podem sobrepor-se; estado informacional pendente não é classe causal; impacto elevado exige proteção; decisão depende de autoridade; causas não foram estabelecidas.

### Representação principal: tabela rastreável

| ID | Tipo | Conteúdo | Origem conceitual | Limite |
|---|---|---|---|---|
| E1 | fato do recorte | ocorrência tem identificador, centro e produto | modelo operacional | não explica causa |
| E2 | estado informacional | histórico pode ser desconhecido | Aula 04 | desconhecido não é incompleto |
| E3 | classificação | classes analíticas podem sobrepor-se | Aula 05 | não decide ação |
| E4 | regra revisável | impacto elevado requer proteção | modelos gerencial/operacional | autoridade decide |
| E5 | limite | associação não prova causa | Aulas 04–05 | vale em todo pacote |

A tabela favorece cobertura e atualização, mas comprime justificativa e relações.

### Representação complementar: relações

| Origem | Relação declarada | Destino |
|---|---|---|
| ocorrência | possui | estado informacional |
| ocorrência | pode pertencer a | classe analítica |
| evidência | sustenta ou limita | classificação |
| decisão | é registrada por | autoridade |
| regra revisável | orienta, sem automatizar | encaminhamento |

Essa forma destaca relações, mas não mostra detalhes por ocorrência. A seta, se desenhada, teria significado da coluna “relação”, nunca causa implícita.

### Conversão e auditoria

Ao converter a tabela principal para relações, identificador e limite podem desaparecer. “Autoridade decide” não autoriza inventar qual cargo. Se “desconhecido” for convertido em “incompleto”, houve incompatibilidade. O pacote precisa de matriz de rastreabilidade e texto curto de convenções.

### Conclusão do P2

O P2 contém modelos operacional e gerencial; matriz de atributos e classes; padrões e regras revisadas; representação principal e complementar; matriz de rastreabilidade; auditoria de perdas; e pendências para a Aula 07. O pacote não é solução técnica nem algoritmo.

## Prática guiada interna: concessão de benefício

Fonte ambígua: “Quando faltar documento, analisar o pedido e, se necessário, encaminhar; pedidos prioritários devem ser resolvidos rapidamente.”

Tabela inconsistente:

| Pedido | Documento | Prioridade | Resultado |
|---|---|---|---|
| B1 | vazio | alta | encaminhar |
| B2 | não | vazio | analisar |

Diagrama textual: `Pedido → Análise → Decisão`, sem significado das setas.

Problemas: “faltar” pode ser ausência confirmada ou desconhecido; não há responsável, critério de prioridade, evidência, autoridade ou definição de “rapidamente”; vazio é ambíguo; o diagrama inventa sequência única e pode sugerir que análise causa decisão.

Uma escolha principal possível é texto estruturado para preservar responsabilidade e exceções; tabela complementar pode comparar casos. A conversão deve usar “desconhecido”, “não aplicável” ou “ausência confirmada”, nunca vazio. A legenda precisa declarar se seta significa precedência de atividade. A divergência entre “encaminhar” e “analisar” permanece pendente até esclarecer a regra.

### Desenvolvimento guiado do caso

Comece separando o que a fonte realmente afirma do que o leitor gostaria de saber. Há falta documental, análise, possível encaminhamento, prioridade e rapidez. Não há definição de documento obrigatório, agente, autoridade, prazo, condição de encaminhamento ou significado de prioridade. Esses itens ausentes são perguntas; não podem aparecer como respostas inventadas na representação.

Uma versão estruturada pode atribuir IDs: B1 para a condição de falta documental; B2 para a atividade de análise; B3 para o encaminhamento condicionado; B4 para a prioridade; B5 para o limite “rapidamente” ainda sem medida. O texto preserva a sequência verbal da fonte apenas como sequência do enunciado, não como prova da ordem operacional. Uma nota declara que agente e autoridade estão pendentes.

Na tabela de casos, “vazio” é substituído conforme evidência. Para B1, se nada informa se o documento foi consultado, escreva “desconhecido”, e não “ausente”. Para B2, a fonte diz “não”, mas é preciso saber se isso significa ausência confirmada; até essa confirmação, a célula pode carregar “valor original: não; significado pendente”. A prioridade vazia também é “desconhecida”, a menos que a dimensão não se aplique, o que a fonte não sustenta.

O diagrama `Pedido → Análise → Decisão` só pode ser mantido como fluxo se a fonte ou uma decisão autorizada confirmar precedência. Mesmo então, “Decisão” precisa dizer qual decisão e o caminho de encaminhamento deve mostrar a condição. Como diagrama de relações, as caixas poderiam ser pedido, documento, análise e encaminhamento, com relações rotuladas “possui situação documental”, “é objeto de” e “pode resultar em”. Nenhum desses rótulos estabelece causa.

Ao final, a representação correta pode continuar incompleta. Correção não exige preencher todas as lacunas; exige preservar o que é conhecido, tornar o desconhecido explícito e impedir que a aparência autorize uma ação não sustentada. Essa é uma habilidade central para ambientes organizacionais: um artefato revisável e honesto vale mais que um fluxo aparentemente acabado construído sobre suposições.

## Atividades, síntese e domínio

### Confusões recorrentes

Representação não é conteúdo. Tabela não elimina ambiguidade; diagrama não é sempre mais claro; seta não significa sequência ou causa automaticamente; lista não implica ordem. Fluxograma não serve para qualquer relação.

Todo procedimento não é algoritmo. Pseudocódigo não é código simplificado nem prova correção. Modelo de estado não é fluxograma; estado não é atividade; tabela de decisão não é tabela-verdade.

Duas formas diferentes podem ser consistentes; conversão não é copiar. Célula vazia não é zero. Cor não basta. Principal não contém tudo; complementar não é ornamento. Rastreabilidade não é apenas numerar. Revisar formato não corrige conteúdo automaticamente.

### Exercícios essenciais

1. **Objetiva.** Qual afirmação distingue corretamente conteúdo e representação?<br>
   A) A representação seleciona e organiza conteúdo por convenções; por isso, mudar a forma pode preservar ou alterar significado e deve ser auditado.<br>
   B) A representação muda a forma do conteúdo, mas nunca seu significado, desde que mantenha os mesmos termos principais.<br>
   C) A representação deve conter todo o conteúdo da origem; qualquer seleção caracteriza erro, independentemente do propósito.<br>
   D) A representação torna-se equivalente à origem quando todos os elementos possuem vínculos de rastreabilidade.

2. **Objetiva.** Num diagrama, uma seta liga “evidência” a “decisão”. Qual interpretação é adequada?<br>
   A) O sentido depende do contexto; a direção da seta basta para indicar que a evidência ocorre antes da decisão.<br>
   B) O sentido depende da convenção predominante do domínio, mesmo que o artefato não a declare ao público.<br>
   C) O sentido deve ser estabelecido por legenda ou rótulo explícito que declare a relação e a direção aplicável.<br>
   D) O sentido pode ser inferido pela posição das caixas quando a leitura visual parece inequívoca.

3. **Objetiva.** Uma tabela será usada para decidir se um caso pode seguir sem análise adicional. Na conversão do texto, desapareceu uma exceção que exige essa análise. Como classificar a diferença?<br>
   A) Perda aceitável, pois uma forma complementar preserva a exceção, ainda que a tabela continue sendo usada isoladamente para decidir.<br>
   B) Perda incompatível com o propósito, porque a exceção é essencial à decisão apoiada pela tabela.<br>
   C) Alteração de nível de detalhe justificada, pois tabelas podem omitir condições para manter legibilidade.<br>
   D) Divergência pendente de avaliação, mesmo que o propósito e a relevância da exceção já estejam declarados.

4. **Dissertativa.** Defina representação e diferencie conteúdo, modelo, notação e convenção.

5. **Análise de linguagem.** Em “quando necessário, encaminhar rapidamente”, separe o conteúdo conhecido das informações ausentes. Produza texto estruturado que registre explicitamente “agente: não informado”, “condição: precisa de esclarecimento”, “destino: não informado” e “prazo: ‘rapidamente’ sem medida”; indique a evidência ainda necessária e formule perguntas de esclarecimento. Não invente respostas.

6. **Conversão.** Converta três regras textuais de classificação em tabela com ID, condição, conclusão, exceção e limite.

7. **Tabela.** Analise células vazias em cadastro. Proponha rótulos para desconhecido, não aplicável, não coletado, zero e ausência confirmada.

8. **Diagrama.** A partir de quatro relações fornecidas no caso do estoque, proponha caixas, relações e legenda; não use causalidade.

9. **Fluxo.** Um desenho usa seta para associar produto e centro. Explique por que fluxo é inadequado e proponha diagrama de relações.

10. **Escolha justificada.** Para auditor acompanhar regra, origem e versão, escolha principal e complementar com quatro critérios.

11. **Rastreabilidade.** Construa `T ⊆ O × R` para cinco elementos e localize um elemento essencial sem ligação.

12. **Auditoria.** Compare texto e tabela do benefício, registrando preservado, perdido, acrescentado, ambíguo e incompatível.

13. **Revisão.** Uma regra muda “histórico incompleto” para “histórico desconhecido”. Identifique artefatos afetados, atualize versões e vínculos.

### Exercícios de aprofundamento opcional

14. **Tabela de decisão.** Acrescente duas combinações à tabela introdutória e marque uma combinação ausente, sem buscar cobertura formal.

15. **Modelo de estado.** Identifique estados, eventos e transições em quatro enunciados; corrija atividade nomeada como estado.

16. **Pseudocódigo.** Interprete o trecho da aula: indique condição vaga, exceção ausente e informação necessária. Não construa algoritmo completo.

17. **Conversão em três etapas.** Texto → tabela → diagrama → texto; compare a última forma com a origem.

18. **Acessibilidade e versão.** Revise artefato dependente de cor, acrescente descrição textual e registre mudança de versão.

19. **Transferência.** Para conciliação, escolha duas formas, crie matriz ampliada e defenda o uso proibido de cada uma.

### Recuperação ativa

- Como conteúdo difere de representação e modelo?
- O que são notação, convenção, sintaxe e significado?
- Por que seta precisa de significado?
- Quando linguagem natural, tabela e fluxograma são adequados?
- Qual a diferença entre lista e sequência?
- Como estado difere de atividade?
- O que tabela de decisão ajuda a revelar?
- Por que pseudocódigo não é código?
- Como escolher forma complementar?
- O que se perde numa conversão?
- O que são consistência e rastreabilidade?
- Como revisar após mudança?

### Reflexão

Quem consegue interpretar o artefato? Cor, posição ou jargão excluem participantes? Diagrama aparenta certeza inexistente? Tabela esconde decisão ou exceção? Pessoa afetada desapareceu? Que responsabilidade existe quando versão desatualizada orienta decisão?

### Síntese

Representação expressa conteúdo por convenções para público e propósito. Modelo organiza aspectos; notação fornece formas; sintaxe organiza; significado determina interpretação. Texto, tabela, diagrama, fluxo, tabela de decisão, modelo de estado e pseudocódigo têm forças e perdas.

Escolha principal e complementar, converta sem inventar, audite perdas, verifique consistência, mantenha rastreabilidade e versões, revise após mudança. Aparência nunca substitui semântica.

Para aplicar a síntese diante de um artefato novo, use quatro perguntas encadeadas. “O que está sendo representado?” localiza conteúdo, modelo e recorte. “Para quem e para quê?” testa adequação e legibilidade. “Que convenções permitem interpretar cada elemento?” verifica notação, significado, acessibilidade e precisão. “Como sei que nada essencial foi alterado?” conduz à origem, à conversão, à consistência, às perdas e à rastreabilidade.

Uma boa entrega, portanto, não é a que acumula mais artefatos. É a que permite ao público responder à pergunta declarada, localizar a origem, reconhecer limites, comparar versões e perceber o que continua desconhecido. Quando uma forma omite algo necessário a outro uso, a complementar deve torná-lo visível. Quando uma mudança ocorre, os vínculos permitem encontrar os pontos afetados. Quando surge divergência, a fonte e a autoridade declaradas orientam a revisão.

Esse modo de trabalhar prepara a passagem para algoritmos sem antecipá-la. O estudante aprende a não confundir a estrutura visível de um procedimento com suas propriedades. Na aula seguinte, entradas, saídas, passos efetivos e término poderão ser examinados sobre uma base representacional mais clara, sem tratar qualquer sequência de caixas ou linhas recuadas como solução algorítmica.

### Mini glossário

**Representação:** forma convencional que torna conteúdo examinável.<br>
**Conteúdo:** aquilo que se pretende expressar.<br>
**Notação:** sistema de símbolos e regras de escrita.<br>
**Convenção:** acordo de interpretação.<br>
**Símbolo:** forma que recebe significado por notação ou legenda.<br>
**Sintaxe:** regras de formação adotadas por uma notação.<br>
**Significado:** interpretação atribuída aos elementos e relações da representação.<br>
**Linguagem natural:** linguagem humana usada para contexto e regras.<br>
**Texto estruturado:** texto organizado por IDs, títulos e escopos.<br>
**Lista:** conjunto de itens; não implica ordem.<br>
**Tabela:** linhas e colunas segundo unidade e atributos.<br>
**Matriz:** tabela que relaciona duas dimensões.<br>
**Diagrama:** forma espacial de elementos e relações.<br>
**Seta:** símbolo cujo significado precisa ser declarado.<br>
**Legenda:** explicação das convenções.<br>
**Fluxo:** ordem ou caminho declarado.<br>
**Fluxograma:** diagrama de fluxo de procedimento.<br>
**Condição:** circunstância examinada numa regra.<br>
**Tabela de decisão:** organização de condições e resultados.<br>
**Estado:** condição relevante num referencial.<br>
**Evento:** ocorrência capaz de motivar transição.<br>
**Transição:** relação entre estados sob evento ou condição.<br>
**Modelo de estado:** representação de estados e transições.<br>
**Pseudocódigo:** notação textual não executável para representar procedimento; não é algoritmo nem código.<br>
**Principal:** forma prioritária para o uso declarado, sem ser fonte universal.<br>
**Complementar:** forma que cobre uma limitação concreta da principal.<br>
**Conversão:** reconstrução de significado em outra forma.<br>
**Consistência interna:** compatibilidade dentro do artefato.<br>
**Consistência entre representações:** compatibilidade semântica entre formas.<br>
**Rastreabilidade:** ligação entre origem, artefatos e versões.<br>
**Perda de informação:** conteúdo ausente após seleção ou conversão.<br>
**Ambiguidade:** possibilidade de interpretações incompatíveis.<br>
**Versão:** estado identificado do artefato.

### Critérios de domínio

No Nível 1, o aluno reconhece formas e convenções. No Nível 2, explica forças, limites e distinções. No Nível 3, constrói e converte com orientação. O início do Nível 4 exige escolher autonomamente duas formas para caso simples, justificar, rastrear, auditar perdas e revisar divergência.

Isso não declara C06 dominada em sistemas complexos.

## Conexão com a Aula 07 — O que é um algoritmo

A Aula 06 forneceu meios para representar problemas, regras, procedimentos, condições, estados e relações. A Aula 07 perguntará quando procedimento é algoritmo, que classe resolve, entradas, saídas, efetividade e término.

Pseudocódigo é representação; algoritmo é conteúdo com propriedades específicas; código é implementação em linguagem. Não são sinônimos. Essas propriedades serão desenvolvidas na próxima aula.

## Referências, métricas e carga

### Referências utilizadas

- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. DOI: [10.1145/3664191](https://doi.org/10.1145/3664191). Representações, comunicação e progressão.
- PÓLYA, George. *How to Solve It*. 2. ed. Princeton University Press, 1957. Representação do problema e revisão, sem método obrigatório.
- ROSEN, Kenneth H. *Discrete Mathematics and Its Applications*. 8. ed. McGraw-Hill, 2019. Relações e pares ordenados.
- ISO; IEC; IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*. ISO, 2017. Apoio terminológico sem reprodução normativa.
- IEEE COMPUTER SOCIETY. *SWEBOK Guide*. Version 4.0a, 2025. Consulta para rastreabilidade e consistência, sem processo profissional completo.

### Carga estimada

- Leitura e anotações: 2h10–2h30.
- Recuperação: 20–30 min.
- Exercícios essenciais: 1h30–2h.
- Prática essencial: 3h15–4h30.
- Solução e revisão: 30–45 min.
- Trilha essencial: aproximadamente 7h45–10h15.
- Percurso completo opcional: 12h–16h, com complementares adicionais, segunda conversão, transferência e auditoria ampliada.
