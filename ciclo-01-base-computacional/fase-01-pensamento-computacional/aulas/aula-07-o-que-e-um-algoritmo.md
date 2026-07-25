# Aula 07 — O que é um algoritmo

## Metadados e objetivo

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo:** De problemas informais a soluções estruturadas
- **Posição:** sétima de 14 aulas
- **Competência:** C07 — Formular e explicar algoritmos
- **Níveis:** Nível 2 — explicação; Nível 3 — formulação guiada; início do Nível 4 em classe pequena
- **Pré-requisitos:** problema, transformação, decomposição, modelo, regra, domínio, representação, conversão e rastreabilidade
- **Prática associada:** [Prática 07 — Avaliar, formular e explicar um algoritmo](../praticas/pratica-07-avaliando-e-formulando-algoritmos.md)
- **Projeto integrado:** início do P3, com contrato e algoritmo inicial do estoque

Ao concluir, o aluno deverá distinguir classe e instância; declarar entrada, domínio, saída, pré e pós-condição; formular contrato e procedimento simples; avaliar efetividade, precisão, ordem e término; argumentar correção intuitivamente; diferenciar algoritmo de representações e entidades próximas; examinar mais de uma instância; e revisar após contraexemplo.

C07 exige Nível 4 ao final da fase. Esta aula inicia esse nível somente em problemas delimitados e algoritmos terminantes com uma instância por execução. Algoritmos complexos ainda exigirão sequência, estado, decisões, repetição, modularização e verificação nas aulas seguintes.

## Introdução: uma sequência bem escrita ainda pode não ser algoritmo

Considere quatro candidatas.

**Candidata A:** “Analise o caso cuidadosamente e faça o que for mais adequado.” Não declara entrada, saída ou critério. “Cuidadosamente” modifica a intenção, não define operação; “mais adequado” exige julgamento oculto.

**Candidata B:** receber uma solicitação, aguardar aprovação, negociar se necessário, pedir opinião e revisar periodicamente. Pode ser processo organizacional legítimo, mas depende de pessoas e eventos, contém espera sem limite e não garante término.

**Candidata C:** pseudocódigo visualmente organizado que recebe “dados”, manda “resolver” e termina sem declarar domínio ou saída. A notação parece algorítmica, mas a aparência não fornece contrato, efetividade ou correção.

**Candidata D:** recebe um registro individual cujo formato foi declarado; verifica um número fixo de propriedades; produz uma categoria estrutural e um motivo; cobre todas as entradas admitidas no recorte; e chega a uma saída após verificações limitadas. Esta candidata possui os elementos necessários para exame, embora ainda precise ser comparada com sua especificação.

A pergunta central é:

> **O que precisa ser verdadeiro para que uma descrição represente um algoritmo adequado?**

A Aula 06 ensinou que pseudocódigo, texto e fluxograma são representações. Agora examinaremos o conteúdo representado. Uma boa representação pode expressar procedimento inadequado; uma forma simples pode expressar algoritmo correto. Código executável também não resolve a distinção: um programa pode executar e ainda tratar a classe errada, omitir uma saída ou não terminar para entrada admissível.

## Problema, classe, instância e domínio

### Problema como transformação

Neste recorte, problema computacional ou procedimental é uma transformação pretendida, ou relação pretendida, entre entradas admissíveis e saídas esperadas. Isso não reduz qualquer problema humano a computação. Questões que exigem autoridade, negociação, valores ou conhecimento não formalizado podem permanecer externas, ser tratadas por pessoas ou aparecer como limites.

“Validar estruturalmente um registro de transação” descreve transformação. “Há muitas transações problemáticas” é situação. “Bloquear fraude” mistura objetivo amplo, inferência causal e intervenção que não foi especificada.

### Classe de problemas

Classe é o conjunto de instâncias que compartilham estrutura, domínio, objetivo e contrato. A classe “classificar estruturalmente um registro individual conforme presença de campos, moeda e estado de autorização” admite muitos registros concretos. Ela não é “resolver T17”.

Definir a classe pela solução cria circularidade. “Casos resolvidos pelos passos abaixo” não informa o problema independente do procedimento. A classe deve poder ser declarada antes do algoritmo candidato, permitindo comparar alternativas.

### Instância

Instância é um caso concreto da classe: o registro T17 com identificador presente, valor declarado em reais, contas informadas e autorização desconhecida. O resultado “pendente de informação” para T17 é solução daquela instância, não algoritmo.

Memorizar respostas de três registros não demonstra generalidade. Um algoritmo precisa abranger toda instância admissível da classe declarada. Casos ajudam a interpretar e revelar falhas, mas sucesso em exemplos não prova essa abrangência.

### Universo e domínio admissível

Universo reúne casos imagináveis; domínio contém as entradas admitidas pelo contrato. Uma fotografia, uma transação com estrutura ilegível ou um conjunto de milhares de registros podem estar fora do domínio de um algoritmo definido para um registro estruturado por execução.

Entrada inválida pode estar fora do domínio ou ser tratada explicitamente. A escolha precisa ser visível. Reduzir domínio é legítimo quando corresponde ao problema assumido; excluir silenciosamente casos difíceis apenas para salvar o procedimento é inadequado.

## Entrada, saída e contrato

### Entrada e conhecimento oculto

Entrada é informação recebida pelo algoritmo: valores, registros, parâmetros ou condições declaradas. O conhecimento pessoal do executor não é entrada legítima se o resultado depende dele sem registro. “Consulte a experiência da equipe” é dependência externa, não dado magicamente disponível.

Uma entrada precisa de unidade e interpretação. “Valor 100” é insuficiente quando moeda e formato importam. “Autorização ausente” difere de “autorização desconhecida”: no primeiro caso há ausência confirmada segundo critério; no segundo não se pode concluir.

### Saída observável

Saída é resultado produzido e observável. Pode ser categoria, valor, indicação de pendência ou justificativa. Efeito colateral, mensagem e decisão externa devem ser distinguidos.

Na validação estrutural, saídas possíveis são “apta para análise posterior”, “pendente de informação” e “estruturalmente inválida no recorte”, sempre acompanhadas de motivo. Nenhuma significa fraude, segurança, aprovação financeira ou bloqueio.

### Pré-condição

Pré-condição é propriedade que deve valer antes da aplicação para que a entrada pertença ao domínio admitido. Não é primeiro passo. “Receber o registro” é ação; “a entrada representa um único registro legível com estados expressos no vocabulário declarado” é pré-condição.

Pré-condição não pode ficar escondida. Pode declarar formato, presença mínima ou intervalo, mas precisa explicar o tratamento de entradas fora dela. Se toda situação difícil for excluída, o contrato pode ficar correto e inútil para o objetivo original.

### Pós-condição

Pós-condição é propriedade que deve valer na saída quando o algoritmo termina para entrada admissível. Não é a última instrução. “Registrar resultado” é ação; “a saída contém exatamente uma categoria estrutural permitida e motivo compatível com os dados de entrada” é pós-condição.

Uma pós-condição precisa ser verificável e relacionar resultado ao contrato. “O algoritmo funciona” não informa o que observar. Pós-condições diferentes podem servir a propósitos diferentes, mesmo para a mesma entrada.

### Contrato introdutório

| Elemento | Declaração |
|---|---|
| classe | validação estrutural de um registro por execução |
| entrada | identificador, valor, moeda, contas, estado dos campos e autorização |
| domínio | uma ocorrência individual cuja estrutura possa ser localizada e inspecionada, ainda que contenha campo ausente ou valor não interpretável |
| pré-condição | há uma única ocorrência e seus componentes podem ser inspecionados |
| saída | inadequação estrutural, pendência de evidência ou aptidão para análise posterior, sempre com motivo |
| pós-condição | campo obrigatório ausente ou não interpretável gera inadequação; autorização desconhecida gera pendência; somente estrutura adequada com autorização confirmada gera aptidão |
| limites | não decide fraude, bloqueio, risco ou autorização definitiva |

Isso é um contrato didático hipotético, não política bancária nem contrato técnico de software. Nele, autorização confirmada com os demais dados adequados produz aptidão para análise posterior; autorização desconhecida produz pendência de informação; ausência confirmada de autorização e campo obrigatório ausente ou não interpretável produzem inadequação estrutural. Nenhuma categoria significa fraude, bloqueio ou irregularidade financeira. A instituição não permite inferir outra regra, e uma correção posterior fora do algoritmo pode ocorrer.

### Especificação não é procedimento

Especificação descreve a relação exigida entre entradas e saídas, além das condições e limites. Procedimento descreve uma maneira de produzir a saída. Confundi-los impede avaliar alternativas: se “verificar campos nesta ordem” aparece como parte do problema, outro algoritmo que verifica em ordem diferente parecerá incorreto mesmo quando entrega a mesma garantia.

O contrato também não precisa revelar como cada operação será implementada. Ele precisa permitir que alguém reconheça uma entrada admissível e avalie o resultado. Duas equipes podem propor procedimentos diferentes para o mesmo contrato. Se uma delas altera silenciosamente a saída de “pendente” para “rejeitada”, não criou apenas outra implementação; mudou a especificação.

Há uma relação de responsabilidade entre as partes. A especificação não pode ser tão vaga que qualquer saída pareça correta. O procedimento não pode acrescentar política sem origem. A representação não pode esconder divergência entre ambos. Quando o contrato é revisado, os passos e seus vínculos precisam ser conferidos.

Considere “produzir categoria e motivo”. Se o procedimento produz apenas categoria, ele está incompleto em relação à pós-condição, ainda que a categoria isolada pareça razoável. Se produz motivo baseado em campo que não pertence à entrada, usa conhecimento oculto. Se o motivo descreve fraude, ultrapassa o limite estrutural. Essas falhas podem ser encontradas antes de qualquer execução.

### Entradas fora do domínio

Há três tratamentos básicos nesta etapa. Primeiro, declarar o caso fora do domínio e encaminhá-lo a outro contrato, sem fingir que foi resolvido. Segundo, ampliar o domínio e acrescentar saída explícita para a situação. Terceiro, reconhecer que a própria classe foi mal formulada e voltar ao problema.

Não confunda três situações. Um lote com várias transações ou uma estrutura impossível de inspecionar está fora deste domínio. Uma ocorrência individual inspecionável com moeda ausente ou valor textual não interpretável é admissível, mas estruturalmente inadequada. Uma ocorrência admissível com todos os campos interpretáveis é estruturalmente adequada; sua evidência ainda pode estar confirmada ou desconhecida.

Nenhum tratamento deve ser automático. Uma imagem de documento pode estar legitimamente fora de um algoritmo que recebe campos estruturados; isso não significa que a necessidade da pessoa desapareceu. O sistema mais amplo precisa saber quem ou o que transforma a imagem em entrada admissível, com que garantias e que ocorre quando essa transformação falha.

Pré-condição documenta uma fronteira, não concede licença para apagar casos. Quanto maior a consequência de ficar fora, maior a importância de tornar essa fronteira compreensível, contestável e ligada a alternativa. Essa preocupação não altera a definição matemática do domínio, mas melhora a adequação do algoritmo no contexto.

## Procedimento, efetividade e precisão

Procedimento é conjunto organizado de ações ou regras para realizar uma transformação. Nem todo procedimento é algoritmo. Para esta definição, os passos precisam ser efetivos: o executor previsto consegue realizá-los, a operação tem interpretação estável, os recursos estão declarados e a ação pode ser concluída no nível adotado.

Efetivo não significa rápido, fácil, automatizado ou implementado. “Somar dois inteiros” pode ser passo efetivo num nível que já admite aritmética. “Descobrir a intenção real de qualquer pessoa” não é operação efetiva sem método e entrada adicionais.

Ações como “verificar adequadamente”, “resolver”, “escolher o melhor”, “tratar exceções” e “analisar profundamente” escondem critérios. Elas devem ser decompostas em operações examináveis ou registradas como dependências externas. “Verificar se moeda pertence ao conjunto admitido” é mais preciso, desde que o conjunto esteja definido.

Granularidade depende do executor e do propósito. Um passo pode usar operação básica já compreendida sem explicar sua implementação interna. Se dois leitores competentes executam instruções e chegam a interpretações incompatíveis, há imprecisão relevante.

Precisão não é quantidade de palavras. Um procedimento longo pode repetir intenção vaga; um procedimento curto pode ser preciso quando o contrato fornece termos. Também não é determinismo automático: regras não determinísticas podem ser precisas ao declarar alternativas permitidas.

### Executor abstrato e operações básicas

Independência de uma linguagem de programação específica não significa independência de qualquer executor. A descrição assume alguém ou algum mecanismo capaz de interpretar operações básicas. O nível precisa ser declarado. “Comparar o estado recebido com três rótulos permitidos” pode ser básico nesta aula; “interpretar qualquer texto jurídico” não pode ser tratado da mesma maneira.

Um passo efetivo possui conclusão reconhecível. “Consultar o estado já contido no registro” termina quando o valor é lido. “Obter confirmação da autoridade” depende de ação externa e talvez não termine. O procedimento pode produzir pendência em vez de permanecer aguardando; a organização pode cuidar da obtenção em processo separado.

Recursos também importam, mesmo sem análise de eficiência. Se a operação requer tabela de moedas admitidas, essa tabela é entrada, parâmetro ou dependência. Se a definição muda por data, a versão precisa integrar o contrato. Chamar o recurso de “conhecimento do sistema” não o torna disponível.

Uma maneira de testar efetividade conceitual é pedir ao autor que responda: quem executa, que informação consulta, que resultado observa e quando sabe que o passo acabou? Respostas vagas localizam trabalho ainda não especificado. Isso não exige transformar cada passo em instrução microscópica; exige evitar saltos cujo conteúdo decide o problema.

### Precisão local e precisão do conjunto

Cada frase pode ser clara e o procedimento continuar impreciso como conjunto. Dois passos podem usar “válido” com sentidos diferentes. Uma condição pode deixar caso restante sem saída. Uma ação pode contradizer a pós-condição. Precisão local precisa ser acompanhada de coerência entre contrato, vocabulário, passos e limites.

O inverso também acontece: um termo resumido pode ser preciso por referência. “Campos obrigatórios”, por exemplo, é examinável se o contrato lista identificador, valor, moeda e contas. Repetir a lista em cada passo pode prejudicar manutenção. Referências estáveis permitem concisão sem esconder significado.

Ambiguidade e desconhecido também diferem. Ambiguidade está na representação ou definição, permitindo leituras incompatíveis. Desconhecido é estado da informação sobre a instância. Um algoritmo preciso pode receber “autorização desconhecida” e produzir pendência; não deve resolver o desconhecido escolhendo uma interpretação.

## Ordem, descrição finita e término

### Dependências de ordem

Ordem importa quando um passo precisa de resultado anterior ou quando trocar ações altera a saída. Verificar a admissibilidade antes de aplicar classificação evita usar valores fora do domínio. Registrar motivo antes ou depois da categoria talvez seja indiferente se ambos usam as mesmas informações e a pós-condição exige os dois.

Nesta aula reconhecemos dependências, mas não rastreamos valores intermediários. A Aula 08 mostrará estado, transição e efeito da troca de passos.

### Descrição finita não é execução finita

Descrição finita possui quantidade finita de símbolos ou instruções. Isso não garante que toda execução termine. “Aguarde até receber autorização” cabe numa linha e pode esperar para sempre. Inversamente, uma descrição finita pode representar número de passos dependente da entrada; repetição será estudada na Aula 10.

O algoritmo principal desta aula evita essa complexidade: trata uma instância e realiza quantidade fixa ou claramente limitada de verificações, sem coleção, contador ou repetição.

### Condição de término

Terminar significa que, para toda entrada admissível, o procedimento alcança uma saída após número finito de passos. Ter a palavra “FIM” não basta se existe espera indefinida antes dela. Terminar nos exemplos também não garante término no domínio.

Um argumento introdutório de término identifica a unidade processada, o número limitado de verificações, a ausência de retorno ou espera sem contrato e o caminho que leva cada condição a uma saída. Operação externa só pode ser tratada como efetiva se seu contrato e limite estiverem declarados.

Procedimentos contínuos, como monitoramento permanente, podem ser úteis e corretamente especificados, mas não se encaixam diretamente na definição de algoritmo terminante adotada aqui. Essa fronteira é pedagógica, não afirmação de que processos contínuos sejam defeituosos.

### Terminar para o domínio, não apenas no caminho comum

O argumento de término precisa considerar todas as alternativas admitidas. Um caminho pode produzir saída imediatamente enquanto outro aguarda. Se o segundo recebe entrada admissível, o algoritmo não possui término garantido. Chamar esse caminho de exceção não altera o problema.

É comum esconder não término numa operação aparentemente simples. “Localizar a confirmação correta” pode procurar indefinidamente se a fonte não contiver confirmação e não houver condição de parada. “Solicitar até obter resposta” pode depender de evento que nunca ocorre. Nesta aula, substituímos a espera por saída de pendência e deixamos a continuação para outro processo.

Quantidade fixa de verificações torna o argumento mais direto, mas não é definição de algoritmo. Há algoritmos terminantes cujo número de passos depende da entrada. A Aula 10 ensinará como expressar repetição, estado de progresso e parada. Antecipar apenas a ideia impede a conclusão errada de que todo algoritmo precisa ter o mesmo número de passos.

Descrição finita e término também não devem ser confundidos com limite de tempo operacional. Um procedimento pode terminar matematicamente e demorar além do aceitável; isso é questão de eficiência e adequação, aprofundada na Aula 13. Aqui basta separar as propriedades: primeiro, ele termina? depois, em outra etapa, o custo é aceitável?

### Finitude histórica e escolha curricular

Listas clássicas de características de algoritmos ajudam a organizar o tema, mas variam em terminologia e alcance. Algumas destacam finitude, definição, entrada, saída e efetividade; outras formulam algoritmos em modelos mais amplos. O curso não transforma uma lista histórica em consenso universal.

Nossa definição inclui término porque o objeto inicial é algoritmo terminante. Ela evita dependência de linguagem de programação específica para proteger a progressão antes da implementação. Inclui classe e especificação para evitar que uma sequência que funcionou num exemplo seja considerada suficiente. Essas escolhas são pedagógicas e avaliáveis, não tentativa de encerrar teoria da computação.

## Definição operacional de algoritmo

Adotaremos no curso:

> **Algoritmo é um procedimento efetivo que, para cada instância admissível de uma classe declarada de problemas, transforma entradas em saídas que satisfazem a especificação e termina após um número finito de passos; esse procedimento admite descrição finita e precisa.**

É uma definição operacional para o estudo inicial de algoritmos terminantes, compatível com tratamentos clássicos, mas não reivindicada como única definição possível em toda a Computação.

O algoritmo é o procedimento abstrato; texto, fluxograma e pseudocódigo são descrições ou representações dele. **Efetivo** exige passos realizáveis. **Classe** delimita o tipo de problema; **instância**, o caso concreto. **Entrada**, **domínio** e **saída** estabelecem o contrato. **Precisão** reduz interpretações incompatíveis. **Especificação** diz o que deve ser verdadeiro. **Término** vale para todas as entradas admitidas. O algoritmo independe de uma linguagem de programação específica e de sua sintaxe executável, não de toda linguagem, vocabulário, representação ou executor.

Uma fórmula isolada pode participar de algoritmo, mas não declara necessariamente entrada, domínio, procedimento e término. Uma lista de tarefas pode ser procedimento, mas depender de julgamentos. Uma receita é analogia limitada: ingredientes e resultado ajudam a pensar em entrada e saída, porém expressões como “a gosto” e condições físicas tácitas mostram por que ela não serve como definição.

### Como examinar um candidato

Ao receber uma descrição, não comece procurando palavras como “SE”, “INÍCIO” ou “FIM”. Pergunte em ordem: que classe afirma resolver; quais instâncias admite; que entrada recebe; que saída promete; que pré e pós-condições compõem o contrato; que operações realiza; que dependências usa; por que termina; e por que a saída satisfaz a especificação.

Examine também o sentido inverso. Cada passo usa somente informações declaradas? Cada saída está autorizada? Existe passo sem função no contrato? Alguma condição admissível fica sem caminho? O procedimento acrescenta decisão que deveria permanecer humana? Essa leitura encontra excesso, não apenas omissão.

Por fim, diferencie falha de representação e falha algorítmica. Se dois termos nomeiam a mesma entrada de maneira inconsistente, a notação pode ser corrigida sem alterar o procedimento. Se o procedimento trata desconhecido como ausente, o significado e possivelmente a saída mudam. Se não há término para uma entrada admissível, trocar o desenho não resolve.

Esse roteiro será usado na prática com sete candidatas. Ele não é fórmula automática: cada critério precisa ser interpretado segundo classe, domínio e executor declarados.

## Correção intuitiva e contraexemplos

Um algoritmo é correto, no sentido desta aula, quando termina e produz saída que satisfaz a especificação para cada entrada admissível. Não faremos prova formal. Construiremos argumento intuitivo estruturado.

O argumento conecta grupos de entrada às saídas. Se campos obrigatórios estão incompletos, a saída “estruturalmente inválida” contém motivo. Se os campos estão completos e a autorização é desconhecida, “pendente de informação” preserva desconhecido. Se dados estão completos, moeda é admitida e autorização confirmada, “apta para análise posterior” satisfaz o limite porque não aprova financeiramente.

Um caso bem-sucedido mostra possibilidade, não universalidade. Muitos casos favoráveis continuam sem provar correção geral. Um contraexemplo é instância admissível para a qual o procedimento não termina ou produz saída incompatível com a pós-condição.

Considere valor presente sem moeda. No contrato adotado, a ocorrência permanece admissível porque sua estrutura é inspecionável, mas recebe “inadequação estrutural”. Uma estrutura totalmente corrompida, que nem permita localizar a ocorrência, fica fora do domínio. A revisão pode alterar contrato, passos ou ambos; deve preservar versões.

Correção difere de eficiência. Um algoritmo pode estar correto e ser lento; pode ser rápido e errado. Quantidade de passos só aparece aqui para sustentar término, não para comparar crescimento.

### Estrutura de um argumento intuitivo

Um argumento útil pode seguir quatro movimentos. Primeiro, recuperar a pós-condição e os limites. Segundo, dividir o domínio em grupos relevantes definidos pelas condições já presentes no procedimento. Terceiro, mostrar que cada grupo chega a uma saída permitida com motivo compatível. Quarto, confirmar que nenhum passo produz conclusão além do contrato.

Se dois grupos se sobrepõem, o argumento deve explicar a prioridade ou reconhecer lacuna. Se existe entrada admissível que não pertence a nenhum grupo, há saída não especificada. Se um grupo contém estado desconhecido e o procedimento o trata como ausência, a incompatibilidade é semântica, não apenas textual.

Chamaremos, por convenção introdutória desta aula, de **correção total** a combinação de término para toda entrada admissível e satisfação da pós-condição. Não faremos prova formal, apenas argumento intuitivo sobre todo o domínio. Um procedimento correto quando termina, mas que pode não terminar, não satisfaz nossa definição.

### Casos, contraexemplos e revisão

Contraexemplo precisa pertencer ao domínio vigente. Se não pertence, pode revelar que a classe é estreita demais, mas não contradiz diretamente a garantia. Por isso a revisão começa confirmando versão do contrato, admissibilidade da instância e saída esperada.

Preservar versão inicial impede recontar a história como se a lacuna nunca tivesse existido. Registre o caso, a propriedade violada, a causa conceitual, a mudança e seu impacto. Revisar somente o pseudocódigo quando a pós-condição estava incompleta mantém a origem do erro. Alterar apenas o contrato para acomodar uma saída indevida pode salvar o texto e abandonar o problema.

## Determinismo, não determinismo e heurística

Algoritmo determinístico determina, para a mesma entrada e condições declaradas, o mesmo próximo passo e resultado. Isso facilita previsão, mas não é requisito universal de toda formulação de algoritmo.

Por convenção introdutória, não determinismo significa que a descrição admite mais de uma escolha ou caminho permitido de modo preciso e **todas** as escolhas autorizadas preservam a pós-condição. Não é teoria universal de não determinismo, ambiguidade, dado desconhecido nem aleatoriedade. A prática principal será determinística; este ponto é opcional.

Heurística é estratégia orientadora que busca solução útil sem garantir, nas condições declaradas, todas as propriedades exigidas de um algoritmo correto. Ela pode ser expressa por algoritmo. Logo, heurística e algoritmo não são opostos absolutos: um algoritmo pode implementar uma heurística, mas sua garantia é sobre executar a estratégia, não necessariamente encontrar resultado ótimo ou correto para o problema amplo.

“Priorizar casos que parecem incomuns” é heurística vaga até definir “incomum”. Mesmo formalizada, pode servir para selecionar análise sem provar risco ou fraude. Em contextos de decisão humana, algoritmo não deve substituir autoridade apenas porque a saída é reproduzível.

### Não determinismo não é aleatoriedade obrigatória

Não determinismo, aleatoriedade e concorrência não são sinônimos. Uma escolha não determinística em modelo abstrato declara alternativas possíveis sem necessariamente sortear uma delas. Um algoritmo aleatorizado usa fonte de aleatoriedade segundo regras. Processos concorrentes tratam atividades que podem avançar em ordens diferentes. Esses assuntos ficam para aprofundamento futuro.

### Pressupostos e limites

Pressuposto é condição aceita para construir o algoritmo, como “os estados recebidos pertencem ao vocabulário declarado”. Pré-condição integra o domínio de aplicação; pressuposto pode incluir também estabilidade de uma definição ou disponibilidade de recurso. Ambos precisam ser visíveis quando afetam a garantia.

Limite declara o que a saída não autoriza. Na transação, classificação estrutural não avalia legitimidade econômica. No estoque, preparação para análise não determina causa ou reposição. Limites evitam que uma saída correta seja usada como resposta a pergunta diferente.

Um algoritmo pode ser tecnicamente preciso e socialmente inadequado se automatiza decisão que exige autoridade, usa entrada enviesada ou não oferece contestação. Esta aula não desenvolve governança completa, mas exige que dependências humanas, consequências e usos proibidos não sejam apagados pela formalização.

Explicabilidade também não é apenas mostrar passos. Um passo claro baseado em regra inadequada continua inadequado. A pessoa afetada precisa saber que informação entrou, que saída foi produzida, que limite existe e onde uma decisão externa ocorreu. Rastreabilidade da Aula 06 continua útil para ligar contrato, passos e versões.

## Matemática introdutória: função, relação e sequência

Seja `D` o domínio de entradas admissíveis e `S` o conjunto de saídas permitidas. A especificação pode ser vista, em nível inicial, como relação `E ⊆ D × S`. Um par `(d, s) ∈ E` significa que a saída `s` é permitida para a entrada `d`.

Se cada entrada admissível possui exatamente uma saída especificada, a relação pode ser tratada como função `f: D → S`. Isso modela o que deve ser obtido, não como obtê-lo. A função não é o algoritmo. Procedimentos diferentes podem calcular a mesma função; um procedimento pode também produzir justificativa, registros ou efeitos que exigem modelo mais rico.

Quando mais de uma saída é permitida, a especificação permanece relação. Um algoritmo não determinístico pode escolher uma saída permitida, desde que todas as escolhas satisfaçam a relação. Ambiguidade ocorre quando não se sabe que relação foi pretendida, e não simplesmente porque há vários pares autorizados.

Uma instância é um elemento `d ∈ D`. Resolver essa instância produz algum `s` com `(d, s) ∈ E`. Algoritmo precisa cobrir o domínio, não apenas um elemento. Se `d ∉ D`, o contrato precisa indicar que está fora ou outro procedimento precisa tratá-lo.

Os passos podem ser representados por sequência finita `p₁, p₂, …, pₙ` no algoritmo simples desta aula. O índice expressa ordem descritiva, não estado detalhado. Se `p₃` depende do resultado de `p₂`, trocar a ordem pode invalidar o procedimento. A Aula 08 dará significado mais rico às mudanças entre passos.

A pós-condição expressa propriedade `P(d, s)` que deve valer quando o algoritmo termina. A correção intuitiva busca explicar por que o procedimento produz `s` tal que `P(d, s)` para todo `d ∈ D`. Não faremos quantificadores ou prova formal como conteúdo avaliativo; a notação apenas torna domínio, relação e garantia mais precisos.

Esse formalismo tem limites. Entradas corporativas podem conter desconhecidos, versões e dependências externas que precisam ser modelados explicitamente. Escrever `f` não elimina ambiguidade nem prova que o domínio está adequado. A matemática organiza a afirmação; a qualidade depende das definições e evidências.

## Algoritmo e entidades próximas

| Entidade | Relação com algoritmo | Diferença decisiva |
|---|---|---|
| representação | torna conteúdo examinável | não é o conteúdo algorítmico |
| pseudocódigo | notação textual independente | pode representar procedimento não algorítmico |
| fluxograma | representação visual de fluxo | símbolos não provam contrato ou término |
| código | texto em linguagem formal | pode implementar incorretamente |
| programa | artefato executável ou tratável por ambiente | inclui decisões de implementação e ambiente |
| implementação | realização concreta | escolhe linguagem, dados e recursos |
| solução de instância | resultado para um caso | não cobre a classe |
| processo organizacional | coordena pessoas, eventos e responsabilidades | pode conter espera e julgamento externo |
| procedimento genérico | orientação organizada | pode ser vago ou não terminante |
| heurística | estratégia sem garantia completa | pode ser implementada algoritmicamente |

## Caso progressivo do estoque e início do P3

O P2 terminou com ocorrências, estados informacionais, classes, regras, representações e limites. Para iniciar P3, definimos uma classe pequena: preparar **uma ocorrência não atendida por execução** para análise posterior.

Contrato inicial:

| Elemento | Declaração |
|---|---|
| entrada | identificador, centro, produto, histórico e evidência registrada |
| domínio | uma ocorrência individual cuja estrutura seja localizável e inspecionável |
| saída | inadequação estrutural, pendência de evidência ou pronta para análise, com motivo |
| pré-condição | há uma única ocorrência inspecionável, mesmo que algum campo esteja ausente ou não interpretável |
| pós-condição | campo obrigatório ausente ou não interpretável gera inadequação; desconhecido permanece desconhecido; evidência insuficiente gera pendência; somente estrutura adequada com evidência suficiente fica pronta |
| limite | não afirma causa, não escolhe intervenção, não substitui autoridade |

Procedimento candidato em linguagem estruturada:

1. receber uma ocorrência admissível;
2. verificar campos obrigatórios e interpretabilidade;
3. se houver inadequação estrutural, produzir essa categoria e motivo;
4. caso contrário, identificar o estado informado do histórico e a evidência;
5. se houver desconhecido ou evidência insuficiente, produzir pendência com motivo;
6. caso contrário, produzir “pronta para análise posterior” com referência à evidência;
7. encerrar.

Representação em pseudocódigo, sem sintaxe de uma linguagem de programação específica:

> INICIAR preparação de uma ocorrência<br>
> RECEBER a ocorrência admissível<br>
> VERIFICAR campos obrigatórios e interpretabilidade<br>
> SE houver inadequação estrutural<br>
> &nbsp;&nbsp;PRODUZIR inadequação e motivo<br>
> CASO CONTRÁRIO<br>
> &nbsp;&nbsp;IDENTIFICAR histórico e evidência<br>
> &nbsp;&nbsp;SE houver desconhecido ou evidência insuficiente<br>
> &nbsp;&nbsp;&nbsp;&nbsp;PRODUZIR pendência e motivo<br>
> &nbsp;&nbsp;CASO CONTRÁRIO<br>
> &nbsp;&nbsp;&nbsp;&nbsp;PRODUZIR preparação para análise e referência<br>
> ENCERRAR o recorte

Há poucas condições simples, sem lógica completa. Cada execução trata uma ocorrência e chega a uma das saídas após verificações limitadas. Toda saída traz motivo. O procedimento não classifica causa, não prescreve intervenção, não encaminha automaticamente e não atualiza estoque.

O argumento intuitivo diz: todos os estados admitidos do histórico são reconhecidos; desconhecido permanece explícito; ausência de evidência gera pendência; somente ocorrência com informações exigidas recebe indicação de preparação; o limite impede converter preparação em decisão. Na Aula 08, uma ocorrência será escolhida para registrar o estado antes e depois de cada passo.

## Prática guiada interna: agendamento

Classe: determinar se uma solicitação individual de agendamento está estruturalmente pronta para análise, com data, serviço e identificação declarados. Candidata: “Confira tudo e agende se estiver certo.”

“Tudo” não define campos, “certo” não possui critério e “agende” produz efeito que pode depender de disponibilidade e autoridade. Uma especificação melhor limita a saída a “pronta para consulta de disponibilidade”, “pendente de informação” ou “fora do recorte”, com motivo. Ela não confirma horário.

Pré-condição possível: uma solicitação individual legível. Pós-condição: saída contém categoria estrutural e lista de lacunas conhecidas. Passos efetivos verificam presença dos três campos e preservam valor desconhecido. Não aguardam resposta externa.

Contraexemplo: data aparece como “em breve”. O campo está presente, mas não possui formato interpretável. Se o procedimento verifica apenas presença, classifica incorretamente. A revisão distingue presença de interpretabilidade e altera contrato e passo. Esse exemplo mostra que precisão depende da especificação, não de aumentar a aparência formal.

## Atividades, recuperação, reflexão e domínio

### Exercícios essenciais

1. **Objetiva.** Qual afirmação distingue algoritmo de representação? A) algoritmo é necessariamente pseudocódigo; B) algoritmo é o procedimento abstrato, que pode ter descrições distintas; C) trocar notação sempre troca algoritmo; D) código e algoritmo são sinônimos.
2. **Objetiva.** Um registro individual tem valor textual não interpretável. Sua estrutura permite localizar os campos. Neste contrato, ele: A) fica necessariamente fora do domínio; B) é admissível e estruturalmente inadequado; C) fica apto porque o campo está presente; D) prova fraude.
3. **Objetiva.** Qual regra pertence ao contrato didático? A) autorização desconhecida prova ausência; B) autorização ausente prova fraude; C) autorização desconhecida gera pendência; D) dados adequados dispensam motivo.
4. **Dissertativa.** Defina algoritmo e explique por que a definição é operacional e delimitada a algoritmos terminantes.
5. **Classe e instância.** Para validação cadastral, declare classe, duas instâncias e um caso fora do domínio.
6. **Contrato.** Esboce entrada, saída e limite para converter uma medida entre unidades fornecidas.
7. **Efetividade.** Analise “descubra a melhor alternativa” e proponha operação examinável ou dependência externa.
8. **Candidata.** Um fluxograma tem início e fim, mas contém “aguardar aprovação”. Avalie término.
9. **Candidata.** Pseudocódigo recebe “dados”, executa “resolver” e imprime “ok”. Localize quatro lacunas.
10. **Ordem.** Em procedimento com validação de formato e classificação, justifique que dependência existe sem rastrear valores.
11. **Contraexemplo e revisão.** Use “data: em breve” contra o algoritmo de agendamento e preserve duas versões.

### Aprofundamento opcional

12. **Contrato completo.** Preencha os sete elementos do contrato de conversão.
13. **Término e correção.** Produza argumentos sobre todo o domínio para cinco verificações limitadas.
14. **Entidades próximas.** Diferencie algoritmo, pseudocódigo, código, programa e implementação.
15. **Relação de especificação.** Modele pares permitidos e explique por que relação não é algoritmo.
16. **Heurística.** Separe a correção do algoritmo executor da garantia substantiva da heurística.
17. **Não determinismo.** Diferencie escolha permitida, ambiguidade, desconhecido e aleatoriedade.
18. **Procedimento contínuo.** Explique o limite do recorte terminante.
19. **Transferência.** Produza contrato alternativo, duas representações e auditoria de equivalência.

### Recuperação ativa

- O que diferencia classe e instância?
- O que são entrada, domínio e saída?
- Como pré-condição difere de primeiro passo?
- Como pós-condição difere de última instrução?
- O que torna um passo efetivo e preciso?
- Como descrição finita difere de execução finita?
- O que precisa valer para o término?
- Por que exemplos não provam correção?
- Como algoritmo difere de pseudocódigo, programa e heurística?
- Por que não determinismo não é ambiguidade?

### Reflexão

Quem definiu as entradas admissíveis? Que pessoas ou casos foram excluídos? Há julgamento humano escondido como operação? A saída parece decisão que o contrato não autoriza? Como contestar resultado? Quem responde por dependência externa ou procedimento inadequado?

### Síntese e mini glossário

Problema declara transformação; classe reúne instâncias; instância é caso. Entrada, domínio, saída, pré e pós-condição formam contrato. Algoritmo é procedimento abstrato efetivo, descritível com precisão e finitude, que termina e satisfaz a especificação no domínio.

**Problema:** transformação pretendida.<br>
**Classe:** conjunto de instâncias com contrato comum.<br>
**Instância:** caso concreto.<br>
**Entrada:** informação recebida.<br>
**Domínio:** entradas admissíveis.<br>
**Fora do domínio:** caso não admitido pelo contrato.<br>
**Inadequação estrutural:** entrada admissível com campo obrigatório ausente ou não interpretável.<br>
**Saída:** resultado observável.<br>
**Pré-condição:** propriedade anterior exigida pelo domínio.<br>
**Pós-condição:** propriedade exigida do resultado.<br>
**Contrato:** declaração de classe, entradas, saídas, condições e limites.<br>
**Procedimento:** ações organizadas para transformação.<br>
**Passo efetivo:** operação realizável e interpretável pelo executor.<br>
**Precisão:** redução de interpretações incompatíveis.<br>
**Dependência:** necessidade de informação ou resultado anterior.<br>
**Descrição finita:** artefato com extensão finita.<br>
**Término:** alcance de saída em passos finitos para toda entrada admissível.<br>
**Correção intuitiva:** argumento estruturado, não prova formal.<br>
**Algoritmo:** procedimento abstrato efetivo que satisfaz a especificação e termina no domínio.<br>
**Determinístico:** fixa próximo passo e resultado nas condições.<br>
**Não determinismo:** escolha precisa entre alternativas permitidas.<br>
**Representação:** forma examinável do conteúdo.<br>
**Pseudocódigo:** notação textual não vinculada à sintaxe executável específica.<br>
**Código:** texto em linguagem formal.<br>
**Programa:** realização tratável por ambiente computacional.<br>
**Implementação:** concretização técnica.<br>
**Heurística:** estratégia cuja execução algorítmica não garante a propriedade substantiva ampla.<br>
**Processo organizacional:** coordenação de atividades, pessoas e eventos.<br>
**Pressuposto:** condição aceita e declarada.<br>
**Limite:** fronteira do que se pode concluir ou fazer.<br>
**Contraexemplo:** instância admissível que contradiz garantia.

### Critérios de domínio

No Nível 1, o aluno reconhece termos e candidatas. No Nível 2, explica distinções. No Nível 3, formula contrato e algoritmo com roteiro. O início do Nível 4 exige formular autonomamente algoritmo para classe simples, declarar contrato, efetividade, ordem, término, correção intuitiva, pressupostos e limites, aplicar a mais de uma instância e revisar após contraexemplo.

Isso não declara domínio de C07 em algoritmos complexos.

## Conexão com a Aula 08 — Sequência e estado

A Aula 07 produziu contrato, entrada, saída, passos, condições simples, algoritmo inicial e argumentos de término e correção. A Aula 08 perguntará qual é o estado antes de cada passo, o que muda, que valor se preserva, como registrar transição, o efeito da troca de ordem e como localizar passo incorreto.

Não fizemos rastreamento completo, atribuição, variável ou invariante. Esses elementos serão necessários para observar a execução, não para redefinir retroativamente o contrato.

## Referências, métricas e carga

### Referências utilizadas

- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. DOI: [10.1145/3664191](https://doi.org/10.1145/3664191). Competências e independência entre fundamentos e implementação.
- CORMEN, Thomas H. et al. *Introduction to Algorithms*. 4. ed. MIT Press, 2022. Problema, entrada, saída, pseudocódigo e correção, sem formalismo avançado.
- KNUTH, Donald E. *The Art of Computer Programming, Volume 1*. 3. ed. Addison-Wesley, 1997. Características clássicas, sem lista universal.
- PÓLYA, George. *How to Solve It*. 2. ed. Princeton University Press, 1957. Compreensão, revisão e exame do resultado.
- ROSEN, Kenneth H. *Discrete Mathematics and Its Applications*. 8. ed. McGraw-Hill, 2019. Funções, relações e sequências.
- LEHMAN, Eric; LEIGHTON, F. Thomson; MEYER, Albert R. *Mathematics for Computer Science*. MIT OpenCourseWare, 2018. Relações, funções e raciocínio matemático introdutório.

### Carga estimada

- Leitura e anotações: 2h15–2h45.
- Recuperação ativa: 20–30 min.
- Exercícios essenciais: 1h30–2h.
- Prática essencial: 3h15–4h20.
- Solução, revisão e autoavaliação: 30–45 min.
- Trilha essencial: aproximadamente 7h30–9h45.
- Percurso completo opcional: 10h30–14h45, com exercícios adicionais, não determinismo, contrato alternativo e transferência.
