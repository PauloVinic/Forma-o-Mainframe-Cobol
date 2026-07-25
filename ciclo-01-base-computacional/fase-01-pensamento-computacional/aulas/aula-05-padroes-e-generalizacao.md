# Aula 05 — Padrões e generalização

## Metadados e objetivo

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo:** De problemas informais a soluções estruturadas
- **Posição:** quinta de 14 aulas
- **Competência:** C05 — Reconhecer padrões e generalizar
- **Níveis:** Nível 2 — explicação; Nível 3 — aplicação guiada; início do Nível 4 em conjuntos pequenos e delimitados
- **Pré-requisitos:** modelos, propósito, unidade de análise, atributos, relações, omissões e domínio de validade
- **Prática associada:** `../praticas/pratica-05-classificando-e-generalizando.md`
- **Projeto integrado:** continuação do P2, acrescentando classificações, padrões candidatos, regras revisadas e limites aos modelos da Aula 04

Ao concluir, o aluno deverá conseguir declarar unidade e atributos de comparação; distinguir igualdade, diferença e semelhança; criar classificação com critérios; preservar sobreposições e desconhecidos; reconhecer regularidade; formular padrão e regra candidatos; separar descrição, classificação e norma; procurar contraexemplos; qualificar exceções; restringir domínio; aplicar regra revista a caso novo; e registrar nova revisão.

A aula não promete domínio completo de C05 em situações complexas. O início do Nível 4 será demonstrado por classificação e generalização autônomas em conjunto pequeno, com evidência contrária, domínio e limites explícitos.

## Introdução: modelos tornam casos comparáveis

### O problema que a aula resolve

A Aula 04 selecionou objetos, atributos, relações e condições. Isso permite comparar casos, mas não prova que exista padrão. Conclusões como “as ocorrências do Centro Sul são todas iguais”, “histórico incompleto causa ruptura”, “produto P2 sempre apresenta divergência” ou “três repetições provam a regra” ultrapassam a evidência. Chamar o primeiro caso diferente de “mera exceção” apenas protege uma conclusão de revisão.

O erro pode levar a solução para padrão inexistente, categoria mal definida, exclusão de pessoas ou casos, tratamento desigual, generalização para domínio errado, falsa causalidade e regra impossível de examinar. A resposta não é deixar de procurar regularidades, mas disciplinar a comparação.

### Ponte com a Aula 04

Abstração selecionou os aspectos considerados; generalização tentará ampliar o alcance de uma descrição ou regra. Entre ambas, precisamos perguntar: quais casos têm unidades compatíveis? Que atributos sustentam semelhança? Que diferença importa ao propósito? Como formar classes? Que regularidade aparece? Que caso contraria a regra? Até onde o raciocínio pode ser reutilizado?

Semelhança nunca é afirmação completa sobre dois objetos. Ela significa semelhança segundo atributos, propósito, domínio, nível e diferenças deliberadamente ignoradas. Essa retomada é suficiente; não reconstruiremos os modelos da aula anterior.

## Unidade, atributos e comparabilidade

### Unidade de comparação

Unidade de comparação é aquilo que conta como um caso na análise: linha de pedido, ocorrência, movimento, produto, centro, transação, solicitação ou ciclo. Misturar unidades cria padrões artificiais. Comparar um centro inteiro com uma ocorrência individual, um produto com uma linha ou um ciclo com média de vários ciclos combina grandezas que respondem a perguntas diferentes.

Se a pergunta é “que ocorrências apresentam problema de qualidade do registro?”, a unidade é a ocorrência. Se pergunta “que centros diferem na taxa?”, a unidade comparada é o centro, embora o indicador derive de linhas. Declarar unidade não é formalidade: define o que pode receber atributos e pertencer a classes.

### Atributos em contexto

Atributo observado vem de observação ou registro direto no recorte, como centro informado. Atributo derivado resulta de transformação declarada, como “impacto elevado” segundo limite escolhido. Atributo desconhecido é relevante, mas não disponível. Não aplicável significa que o atributo não faz sentido naquele caso. Omitido significa que foi excluído do modelo. Rótulo atribuído, como “prioritário”, é classificação produzida, não fato bruto.

Campo disponível não é automaticamente relevante. Incluir identificador interno numa comparação de impacto apenas porque existe acrescenta distinção sem função. Inversamente, atributo ausente pode continuar relevante e precisar da categoria “desconhecido”.

### Condições de comparabilidade

Casos são comparáveis para uma pergunta quando possuem unidade compatível, pertencem ao recorte, usam definições equivalentes e têm atributos interpretáveis. Desconhecido não pode ser tratado como “não”. Uma ocorrência sem registro sobre divergência não é ocorrência comprovadamente sem divergência.

Comparabilidade também depende do tempo e do contexto. Taxas idênticas calculadas em populações e períodos diferentes não sustentam automaticamente a mesma conclusão. Antes de comparar valores, compare seus significados.

## Igualdade, diferença e semelhança

### Igualdade e diferença

Igualdade, nesta aula, indica coincidência em atributo declarado. Duas ocorrências podem ter o mesmo produto e ainda diferir em centro, momento, condição e consequência. Igualdade de um valor não significa identidade completa dos casos.

Diferença é distinção em atributo relevante. Ela não obriga classes diferentes: duas ocorrências com centros distintos podem pertencer à mesma classe “histórico incompleto”. O efeito da diferença depende do critério.

### Semelhança orientada pelo propósito

Semelhança é uma comparação segundo atributos escolhidos. Pode considerar importância qualitativa, tolerância, nível de detalhe e diferenças ignoradas. Não usaremos distância matemática. Dois casos podem ser semelhantes para gestão porque têm impacto e proteção equivalentes, mas diferentes para investigação porque seus registros e condições divergem.

Uma embalagem semelhante visualmente pode ocultar produtos com consequências diferentes. A mesma taxa pode resultar de populações incompatíveis. O mesmo rótulo pode ter definições distintas. O mesmo sintoma pode acompanhar causas ainda desconhecidas. Aparência, nome ou número isolado não bastam.

Não existe peso “natural” dos atributos. Para segurança, impacto pode prevalecer sobre frequência; para auditoria, completude do histórico pode ser decisiva. A importância precisa ser justificada pelo propósito, sem cálculo formal nesta etapa.

Tolerância também precisa ser declarada. Dois valores arredondados podem parecer iguais embora os registros originais sejam diferentes; duas datas no mesmo mês podem ser semelhantes para relatório mensal e distintas para prazo diário. Escolher tolerância modifica os pares considerados semelhantes e pode alterar classes e padrões.

Uma comparação útil registra tanto semelhanças quanto diferenças ignoradas. Dizer “H1 e H12 são semelhantes quanto a produto, divergência e ação posterior, ignorando o centro” é mais informativo que “os casos são parecidos”. A declaração permite a outra pessoa contestar se centro deveria importar.

Quando atributos têm definições divergentes, não existe comparação responsável apenas por alinhar rótulos. Antes de afirmar igualdade, é preciso harmonizar significado ou separar domínios. A palavra idêntica numa coluna não garante o mesmo conceito.

## Classificação, classes e pertencimento

### Definição operacional

Adotaremos:

> **Classificação é a atribuição de casos a classes segundo atributos e critérios declarados, para um propósito e domínio determinados, preservando casos desconhecidos, sobrepostos ou não classificáveis quando o critério assim exigir.**

Classe ou categoria é um conjunto de casos tratados conjuntamente segundo critério. Pode ser descritiva, como “histórico incompleto”; operacional, como “aguarda evidência”; normativa, quando uma política define tratamento; ou construída para análise. “Classe” aqui não se refere a linguagem de programação.

### Critério de pertencimento

Um critério deve permitir explicar por que o caso entra, por que não entra, o que ocorre quando falta informação, se múltiplo pertencimento é permitido e se as classes precisam cobrir o universo. “Parece problemático” não é critério. “Possui histórico marcado como incompleto no período” é examinável, embora dependa da qualidade do registro.

Critério não transforma categoria em natureza do objeto. Organizações criam rótulos para agir e analisar; essas escolhas podem distribuir atenção, recursos e consequências. Por isso, precisam ser transparentes e contestáveis.

### Exclusivas, sobrepostas, exaustivas e incompletas

Em classificação exclusiva, cada caso recebe uma classe segundo o critério. Em classificação sobreposta, um caso pode pertencer simultaneamente a “histórico incompleto”, “divergência a investigar” e “impacto elevado”. Forçar exclusividade apagaria dimensões.

Classificação exaustiva cobre todo o universo declarado. Uma não exaustiva preserva desconhecido, pendente, não classificável ou fora do escopo. “Outros” só é útil com significado e revisão; não deve esconder critério ausente. Nem toda classificação é partição.

### Casos limítrofes

Caso limítrofe fica próximo de um limite convencional ou admite interpretações justificáveis. Se “impacto elevado” começa em valor definido, um caso exatamente no limite revela se o operador usado e a unidade foram declarados. O limite não é lei natural: é escolha ligada ao propósito.

Casos limítrofes também aparecem sem número. Uma solicitação pode trazer documento parcialmente legível: classificá-la como “documentação completa” ou “incompleta” depende do que completo significa para a pergunta. Se o critério apenas diz “documento presente”, ele pode admitir um arquivo inutilizável. O caso não é inconveniente periférico; ele revela que o pertencimento foi especificado de modo insuficiente.

Quando duas pessoas justificadas classificam o mesmo caso de formas diferentes, não se deve escolher uma resposta por autoridade ou maioria sem examinar o critério. A divergência pode revelar termo ambíguo, atributos ausentes ou classes que deveriam sobrepor-se. Registrar o desacordo fornece evidência para revisão.

### Consequências da classificação

Uma classificação pode ser apenas descritiva e ainda produzir consequências quando incorporada a relatório, prioridade ou distribuição de recursos. A categoria “baixa prioridade” pode alongar espera; “não classificável” pode retirar caso de indicador; “outros” pode tornar um grupo invisível. O efeito não prova que a classificação seja inadequada, mas entra na avaliação de seu propósito.

Por isso, classe precisa ter uso permitido e proibido. “Impacto elevado” pode servir para localizar casos que merecem exame sem autorizar conclusão sobre causa ou culpa. “Histórico incompleto” pode acionar coleta de evidência sem ser tratado como prova de falha operacional. A separação entre rótulo e decisão protege pessoas e melhora a análise.

## Regularidade, padrão e coincidência

### Regularidade e padrão

Regularidade é recorrência ou consistência observada entre casos segundo atributos declarados. Adotaremos:

> **Padrão é uma regularidade estruturada e relevante para uma pergunta, identificada por critérios explícitos em um conjunto de casos e limitada ao domínio e às evidências examinadas.**

Padrão depende da abstração, pode ser provisório e não é automaticamente causal ou universal. Precisa sobreviver à procura de casos contrários. Diferentes modelos podem tornar padrões diferentes visíveis porque selecionam atributos e níveis distintos.

### Repetição não basta

Repetição é ocorrência novamente observada. Coincidência é repetição sem sustentação suficiente para tratá-la como estrutura relevante. Regularidade descreve consistência no conjunto. Padrão candidato é uma interpretação examinável dessa regularidade. Regra sustentada é formulação que passou pelos casos e limites definidos até o momento.

Três ocorrências do mesmo produto não provam padrão se esse produto domina a população. Cinco históricos incompletos acompanharem divergência não prova que incompletude produz divergência. Frequência pode motivar pergunta, nunca substituir critério e evidência.

O denominador importa mesmo sem estatística formal. Se oito de dez casos são do Centro A, encontrar seis ocorrências de uma característica nesse centro não basta para afirmar concentração incomum. Precisamos pelo menos reconhecer a composição do conjunto e evitar comparar contagens como se as oportunidades fossem iguais. Esta aula não estima probabilidades; ensina a não esconder a base da observação.

Também é preciso distinguir ausência observada e ausência de observação. Se nenhum caso conhecido registra condição física inadequada, a conclusão responsável limita-se aos registros disponíveis. Quando várias condições estão desconhecidas, “não encontramos” não pode ser reescrito como “não existe”.

### Onde padrões podem aparecer

Podem aparecer em valores recorrentes, combinações de atributos, diferenças entre grupos, exceções recorrentes, regras de classificação e sequências organizacionais observadas. Uma sequência recorrente não vira fluxo obrigatório nem procedimento executável. O propósito aqui é descrever e comparar, não ensinar algoritmo.

## Regras, descrição e causalidade

### Três sentidos de regra

Regra descritiva candidata formula regularidade observada: “no conjunto examinado, ocorrências com histórico incompleto aparecem em mais de uma classe de divergência”. Ela descreve o recorte sem afirmar causa.

Regra classificatória declara critério de pertencimento: “classificar como qualidade de registro comprometida quando o histórico estiver incompleto”. Regra normativa declara o que deve acontecer por política, lei ou negócio: “ocorrências de impacto elevado devem receber análise adicional”.

O que ocorre, como classificamos e o que deve ocorrer são afirmações diferentes. Frequência não cria obrigação. Política não prova que o comportamento já ocorre. Classificação não é decisão automática: pode organizar atenção sem determinar tratamento.

Uma mesma frase pode ocultar os três sentidos. “Casos incompletos vão para revisão” pode descrever prática observada, definir classe operacional ou prescrever obrigação. Para torná-la examinável, pergunte: o enunciado relata o que aconteceu, estabelece como rotular ou determina o que deve acontecer? Qual fonte sustenta a obrigação? Que evidência sustenta a descrição? Que atributo ativa a classificação?

Misturar estatutos permite erros circulares. Se a organização classifica como “crítico” todo caso enviado à revisão e depois conclui que casos críticos sempre vão à revisão, o padrão repete a própria definição. Não aprendemos algo novo sobre os casos; apenas reencontramos o critério usado para criá-los.

### Coocorrência não é causa

Duas características aparecerem juntas é coocorrência ou associação no recorte. Para afirmar causalidade seriam necessárias perguntas e evidências adicionais. “Histórico incompleto causa linha não atendida” é especialmente inadequado: incompletude pode apenas impedir reconstrução.

Padrões também podem surgir como consequência do processo de registro. Se uma equipe registra mais detalhadamente casos graves, a associação entre detalhe e gravidade pode refletir prática documental. A linguagem deve permanecer: “aparece junto”, “é compatível”, “sustenta ou enfraquece hipótese”, não “produz” sem evidência.

## Generalização, alcance e reutilização

### Definição operacional

Adotaremos:

> **Generalização é a extensão justificada de uma descrição, regra ou raciocínio dos casos examinados para uma classe mais ampla ou para casos novos, dentro de domínio, condições, evidências e limites declarados.**

Abstração seleciona aspectos; generalização amplia alcance. Uma regra pode classificar casos existentes sem prever eventos futuros. Previsão exige condições adicionais. Generalizar não é universalizar.

### Ampla demais, estreita demais e ajustada aos exemplos

Generalização ampla inclui casos que não satisfazem condições. “Todo valor alto é fraude” alcança transações legítimas. Generalização estreita descreve apenas exemplos já vistos e não reutiliza raciocínio. “Ocorrências P2 do Centro A às 10h03 com registro R7” pode memorizar casos sem capturar regularidade útil.

Ajuste excessivo ocorre quando se adicionam detalhes somente para proteger a regra contra cada contraexemplo, até ela repetir a lista conhecida. Não estamos estudando aprendizado de máquina; a ideia é lógica e prática: uma regra reutilizável precisa equilibrar alcance e restrições justificáveis.

Uma forma simples de examinar esse equilíbrio é pedir que cada condição tenha função explicável. Se remover “Centro A” não muda a sustentação nem o propósito, a condição pode ser detalhe memorizado. Se removê-la inclui casos que usam definição incompatível, ela protege o domínio de modo substantivo. A diferença está na justificativa e na evidência, não no número de condições.

Regra estreita pode ser correta e ainda pouco útil. “Nos casos H1 e H12 houve divergência registrada” descreve os exemplos com segurança, mas não generaliza. Regra ampla pode ser útil como hipótese e ainda não estar sustentada. O estatuto “candidata” comunica que sua função atual é orientar exame, não autorizar conclusão.

### Domínio e condições de validade

Declare universo, população, período, atributos, exclusões e condições. “Nas ocorrências hipotéticas com histórico conhecido deste ciclo...” é mais responsável que “sempre”. Se os centros usam definições diferentes, o domínio precisa ser separado ou a comparação suspensa.

Reutilizar raciocínio exige semelhança pertinente. Transferir uma regra do estoque para transações apenas porque ambos têm “impacto” ignora significados diferentes. O método de declarar atributo, procurar contraexemplo e revisar pode ser reutilizado; a conclusão substantiva, não automaticamente.

Domínio não deve ser alterado depois de observar resultado apenas para fazer a regra parecer correta. É legítimo restringi-lo quando o contraexemplo revela condição substantiva antes omitida, mas a mudança precisa ser registrada. “Vale somente para os casos que confirmam” é circular. “Vale para ocorrências com divergência conhecida porque a conclusão usa esse atributo” é restrição examinável, embora ainda precise de evidência.

Condições também podem mudar no tempo. Uma definição administrativa, fonte de dados ou política pode ser revista. Regra sustentada num ciclo deixa de ser automaticamente aplicável ao seguinte. Data, versão da definição e população são partes do alcance, não detalhes documentais.

## Exemplos, contraexemplos, exceções e revisão

### O papel dos casos

Exemplo favorável satisfaz a regra e mostra como interpretá-la, mas não a prova sozinho. Caso novo não participou da formulação e verifica se a regra tem algum alcance além dos exemplos usados.

Contraexemplo é caso dentro do domínio e das condições declaradas que contradiz uma afirmação geral. Um único contraexemplo basta para refutar a forma universal da regra, ainda que não determine a melhor revisão. A equipe pode restringir domínio, alterar condição ou rejeitar a regra.

Exemplos devem variar de modo relevante. Dez casos quase idênticos podem oferecer menos exame que três casos com centros, produtos e condições diferentes. Não faremos amostragem estatística; basta reconhecer que diversidade de situações expõe pressupostos e que quantidade bruta não garante cobertura conceitual.

### Exceção declarada não é proteção retórica

Exceção é caso que a própria regra exclui por condição explícita e justificada. Se uma política diz “salvo transações previamente autorizadas”, uma transação autorizada não refuta a regra normativa. Porém, chamar todo caso contrário de exceção depois de observá-lo torna a regra imune a evidência.

Caso fora do domínio também não é contraexemplo: uma regra sobre três produtos não é refutada por quarto produto, mas esse caso pode mostrar que o domínio é estreito. Caso desconhecido não favorece nem contradiz enquanto faltar informação relevante.

### Procura deliberada

Procure combinações capazes de contrariar a regra: atributo presente sem conclusão, conclusão presente sem atributo, caso no limite, desconhecido, classe sobreposta, centro diferente e período diferente. A intenção não é “derrotar” o modelo, mas localizar seu alcance.

Após feedback, registre versão anterior, evidência, mudança de critério ou domínio, efeito e questão aberta. Revisão pode fortalecer, restringir ou rejeitar a regra.

Há quatro respostas responsáveis a um caso contrário. Primeira: corrigir erro de dado comprovado, sem apagar o registro da correção. Segunda: reconhecer que o caso está fora do domínio previamente declarado. Terceira: restringir ou reformular a regra quando uma condição relevante faltava. Quarta: rejeitar a regra quando a contradição atinge seu núcleo. Escolher entre elas requer justificativa, não preferência por manter a hipótese.

Uma exceção declarada também deve ser testada. Pergunte se sua condição pode ser reconhecida antes de aplicar a regra, se tem relação com o propósito e se não cobre quantidade tão grande que esvazie a afirmação. Exceções numerosas ou vagas sugerem que classes ou domínio precisam ser reconstruídos.

## Método guiado e matemática introdutória

### Roteiro de trabalho

Um percurso possível é: declarar pergunta e unidade; selecionar atributos; verificar comparabilidade; comparar; propor classes e critérios; classificar; preservar sobreposições e desconhecidos; observar regularidades; formular padrão e regra candidatos; buscar exemplos contrários e casos limítrofes; restringir domínio; aplicar a caso novo; registrar limites; revisar. Descobertas podem exigir retorno a qualquer decisão anterior.

Esse roteiro organiza investigação, mas não é algoritmo. Não define execução, término, contrato ou implementação.

Em cada passagem, registre evidência e decisão. Na comparação, anote atributos ignorados. Na classificação, preserve casos que não entram. No padrão, separe observações favoráveis de desconhecidos. Na regra, declare o tipo. No contraexemplo, confirme que o caso pertence ao domínio. Na revisão, explique o que mudou e que uso deixou de ser autorizado.

O roteiro pode começar por contraexemplo já conhecido ou por classificação existente que precisa ser auditada. Não há sequência obrigatória. O requisito é manter rastreabilidade entre pergunta, atributos, casos, regra e revisão.

### Conjuntos e pertencimento

Seja `U` o universo de casos no recorte e `C` uma classe:

`C ⊆ U`

Para um caso `x`, `x ∈ C` significa que pertence à classe; `x ∉ C`, que não pertence segundo o critério. Se classes `C₁` e `C₂` se sobrepõem, casos comuns pertencem a `C₁ ∩ C₂`.

Uma partição é caso particular: classes não vazias cobrem `U` e são disjuntas duas a duas. Só a use quando cada caso precisar de exatamente uma classe. Para desconhecidos, pendentes ou não classificáveis, mantenha `N ⊆ U` explícito; esses casos não desaparecem da análise.

### Classificação como função e semelhança como relação

Somente quando a classificação é exclusiva e definida para cada caso admissível, pode ser expressa por `g: U → K`, onde `K` é o conjunto de classes. Se houver pendentes, restrinja o domínio explicitamente ou inclua categoria controlada. Não introduziremos funções parciais formalmente.

Semelhança pode ser tratada como relação `S ⊆ U × U`: pares de casos considerados semelhantes segundo critério. Isso não significa identidade nem exige, nesta aula, propriedades formais de relação de equivalência.

Comparações como “impacto ≥ limite definido” dependem de unidade, período, definição e propósito. O número não transforma limite convencional em verdade natural.

## Caso progressivo do estoque

### Conjunto didático hipotético

A tabela abaixo é material de ensino; não acrescenta fatos ao projeto. `C` significa conhecido, `I`, incompleto, e `D`, desconhecido. “Elevado” usa limite didático declarado apenas para o exercício.

| Caso | Centro | Produto | Histórico | Divergência | Condição física | Impacto | Ação posterior | Classe inicial |
|---|---|---|---|---|---|---|---|---|
| H1 | A | P1 | C | registrada | conhecida | baixo | revisar registro | divergência |
| H2 | A | P2 | I | desconhecida | desconhecida | elevado | obter evidência | qualidade |
| H3 | B | P2 | C | não registrada | conhecida | baixo | acompanhar | evidência suficiente |
| H4 | B | P3 | I | registrada | conhecida | médio | investigar | qualidade; divergência |
| H5 | A | P3 | C | registrada | desconhecida | elevado | investigar | divergência; impacto |
| H6 | B | P1 | D | desconhecida | desconhecida | elevado | obter evidência | não classificável; impacto |
| H7 | A | P2 | C | não registrada | conhecida | médio | acompanhar | evidência suficiente |
| H8 | B | P2 | I | não registrada | conhecida | baixo | completar histórico | qualidade |
| H9 | A | P1 | C | registrada | conhecida | elevado | investigar | divergência; impacto |
| H10 | B | P3 | C | não registrada | conhecida | médio | acompanhar | evidência suficiente |
| H11 | A | P3 | I | desconhecida | desconhecida | baixo | obter evidência | qualidade |
| H12 | B | P1 | C | registrada | conhecida | baixo | revisar registro | divergência |

As classes se sobrepõem. H4 pertence a qualidade e divergência; H6 permanece não classificável quanto à divergência, mas pode integrar impacto. “Desconhecida” não equivale a “não registrada”.

### Padrões candidatos e contraexemplos

Padrão candidato 1: “históricos incompletos acompanham divergência registrada”. H4 favorece, mas H8 contradiz a formulação ampla e H2/H11 são desconhecidos. A regra não se sustenta como universal; no máximo, “algumas ocorrências incompletas também possuem divergência registrada no conjunto didático”. Isso pouco reutiliza e não estabelece causa.

Padrão candidato 2: “impacto elevado ocorre somente com divergência registrada”. H5 e H9 favorecem; H2 e H6 têm divergência desconhecida, portanto não podem ser usados como confirmação. A regra precisa aguardar evidência ou restringir-se aos casos com divergência conhecida. Mesmo restrita, não explica o impacto.

Padrão candidato 3: “casos com evidência suficiente recebem acompanhamento”. H3, H7 e H10 favorecem, mas H1 e H12 têm histórico e condição conhecidos e recebem revisão. O critério “evidência suficiente” estava vago. A classificação precisa declarar suficiente para qual pergunta.

Esses três candidatos mostram perdas diferentes. O primeiro encontra contraexemplo conhecido; o segundo encontra desconhecidos que impedem conclusão; o terceiro revela rótulo circular ou ambíguo. Nem todo problema de regra é resolvido do mesmo modo. H8 pede revisão da afirmação; H2 e H6 pedem preservação da incerteza; “evidência suficiente” pede novo critério.

Também não se deve escolher apenas o candidato que parece mais fácil de sustentar. O propósito determina utilidade. Uma regularidade forte sobre cor de embalagem seria irrelevante se a pergunta trata qualidade do histórico, salvo evidência de relação pertinente. Procurar padrões sem pergunta aumenta a chance de coincidências decorativas.

### Casos novos

Considere três casos também hipotéticos:

| Caso | Centro | Produto | Histórico | Divergência | Condição | Impacto |
|---|---|---|---|---|---|---|
| N1 | A | P2 | I | registrada | conhecida | médio |
| N2 | B | P3 | C | não registrada | desconhecida | elevado |
| N3 | A | P1 | D | desconhecida | desconhecida | baixo |

N1 pode pertencer a qualidade e divergência. N2 contradiz qualquer regra que associe todo impacto elevado a divergência registrada, desde que esteja no domínio. N3 precisa permanecer pendente nas classificações que exigem histórico ou divergência. Aplicar regra não significa decidir ação automaticamente.

O caso novo tem função específica: reduzir a tentação de moldar a regra aos casos usados em sua criação. Se, após N2, adicionarmos “exceto P3 do Centro B” sem justificativa substantiva, apenas memorizamos o novo caso. Uma revisão melhor questiona se divergência era condição necessária para impacto ou rejeita a afirmação.

Aplicação pode produzir três resultados legítimos: pertencimento sustentado, não pertencimento sustentado ou insuficiência de informação. Forçar somente sim/não apaga N3. A categoria pendente não é falha do exercício; é resultado informativo sobre dados e domínio.

### Resultado do P2 até aqui

O P2 agora reúne modelos operacional e gerencial, matriz de atributos, classificações sobrepostas, padrões candidatos, regras revistas, contraexemplos, domínio, limites e desconhecidos. A forma de registrar e combinar esses elementos com menor ambiguidade fica pendente para a Aula 06.

## Prática guiada interna: transações

Considere a regra superficial: “todas as transações acima de R$ 10.000 são suspeitas”. Os casos são hipotéticos: T1, R$ 15.000, pagamento corporativo autorizado; T2, R$ 800, destinatário desconhecido e contestação registrada; T3, R$ 12.000, autorização desconhecida; T4, R$ 20.000, valor alto e dado cadastral incompleto.

Valor alto é atributo insuficiente para transformar classificação em decisão. T1 é contraexemplo à regra universal se “suspeita” significar problemática apenas pelo valor. T2 mostra que valor baixo não exclui sinais relevantes. T3 permanece desconhecida quanto à autorização. T4 pode pertencer simultaneamente às classes descritivas “valor alto” e “cadastro incompleto”.

Uma revisão responsável separa descrição e decisão: “classificar como valor alto as transações acima do limite convencional; examinar com outros atributos antes de decidir tratamento”. O limite, a moeda, o período, o domínio e o uso proibido precisam ser declarados. A coocorrência de valor e problema não demonstra que o valor causou o problema.

## Atividades, síntese e domínio

### Confusões recorrentes

Casos parecidos não são iguais, e semelhança não é universal. Atributo disponível pode ser irrelevante. Classificação adequada não é necessariamente única, exclusiva ou exaustiva. “Outros” não corrige critério ruim; desconhecido não significa não.

Repetição não prova padrão; padrão não prova causa; frequência não cria norma. Exemplo favorável não valida sozinho. Contraexemplo raro ainda contradiz regra universal. Exceção só protege a regra quando foi declarada e justificada, não quando serve para ignorar evidência.

Generalização não é abstração nem previsão. Regra detalhada pode apenas memorizar exemplos. Classe pequena pode ter alto impacto. Categorias organizacionais não são naturais ou neutras: classificações distribuem atenção e consequências e precisam admitir contestação e revisão.

Outro erro é supor que uma classificação existente já foi validada por estar em uso. Uso frequente demonstra adoção, não adequação. Também é inadequado mudar atributo após cada resultado sem versionar o critério: casos iguais passam a receber rótulos diferentes sem explicação. Finalmente, aplicar regra a caso novo não encerra trabalho; o resultado pode revelar limite e exigir retorno aos atributos ou às classes.

### Exercícios essenciais

1. **Objetiva.** Duas ocorrências têm o mesmo produto. Qual conclusão é mais adequada?
   A) São semelhantes para qualquer pergunta porque compartilham o objeto principal.
   B) São iguais no atributo produto; semelhança adicional depende de propósito e atributos.
   C) Devem pertencer à mesma classe, salvo se os centros forem diferentes.
   D) Formam padrão se o produto também apareceu em terceiro caso.

2. **Objetiva.** Uma classificação contém “divergência”, “impacto elevado” e “histórico incompleto”. Um caso atende aos três critérios. Isso indica:
   A) erro, porque toda classificação precisa de classe única;
   B) sobreposição possível, se cada critério e o propósito permitirem;
   C) partição, porque as três classes cobrem o caso;
   D) desconhecimento, porque três rótulos impedem classificação.

3. **Objetiva.** Uma regra diz “toda ocorrência incompleta possui divergência”. Há caso incompleto, dentro do domínio, com divergência conhecida como não registrada. Ele é:
   A) exceção automática por ser raro;
   B) caso fora do domínio por contrariar a conclusão;
   C) contraexemplo que exige rejeitar ou revisar a regra;
   D) exemplo favorável de incompletude.

4. **Dissertativa.** Defina unidade de comparação e explique como misturar centro, produto e ocorrência pode produzir regularidade falsa.

5. **Dissertativa.** Diferencie atributo observado, derivado, desconhecido, não aplicável, omitido e rótulo atribuído usando cadastro.

6. **Análise de caso.** Duas áreas usam “resolvido” com significados diferentes. Avalie comparabilidade, semelhança aparente e revisão necessária.

7. **Classificação.** Para cinco solicitações fornecidas por você, proponha três classes, ao menos uma sobreposição e uma categoria pendente. Declare critérios.

8. **Dissertativa.** Diferencie regularidade, padrão candidato e regra, explicando por que nenhuma prova causa.

9. **Análise de regra.** “Todo pagamento atrasado deve receber multa” mistura descrição ou norma? Declare domínio, exceção justificável e informação desconhecida.

10. **Contraexemplo e revisão.** Crie contraexemplo para “todo impacto elevado possui divergência” e produza uma versão restrita ou rejeite-a.

11. **Caso novo.** Aplique uma regra revista aos casos N1, N2 e N3. Registre pertencimentos, recusa por insuficiência e necessidade de nova revisão.

### Exercícios de aprofundamento opcional

12. **Conjuntos.** Defina `U`, duas classes `C₁` e `C₂`, um caso em `C₁ ∩ C₂` e conjunto `N` de não classificados. Explique por que não formam necessariamente partição.

13. **Classificação como função.** Proponha `g: U → K` para classificação exclusiva. Depois introduza pendente e explique domínio restrito ou categoria controlada.

14. **Semelhança como relação.** Escreva três pares em `S ⊆ U × U`, declare critérios e mostre par que deixa de ser semelhante quando o propósito muda.

15. **Regra ajustada demais.** Analise uma regra que enumera todos os horários, produtos e centros conhecidos. Explique por que memoriza casos e proponha revisão.

16. **Casos limítrofes.** Um limite de impacto é R$ 10.000. Analise casos abaixo, exatamente e acima, declarando unidade, período e natureza convencional.

17. **Consequências.** Compare duas classificações de solicitações que distribuem prioridade de modo diferente. Identifique pessoas afetadas, direito de contestação e revisão após dano.

18. **Transferência.** Leve o método, não a conclusão, do estoque para transações: formule padrão candidato, contraexemplo, domínio e caso novo sem usar estatística.

### Recuperação ativa

- O que precisa ser definido antes de comparar casos?
- Como igualdade difere de semelhança?
- Por que semelhança depende do propósito?
- O que é critério de pertencimento?
- Quando classes podem se sobrepor?
- O que é regularidade?
- Como padrão difere de repetição?
- Por que padrão não prova causa?
- Como generalização difere de abstração?
- O que é contraexemplo?
- Quando uma exceção não refuta a regra?
- O que fazer com casos desconhecidos?
- Como restringir domínio?
- Como testar regra em caso novo?
- O que caracteriza regra ajustada apenas aos exemplos?

### Reflexão

Quem define categorias e quem sofre suas consequências? Que categoria administrativa está sendo tratada como natural? “Outros” esconde grupos pequenos? Uma regra desloca custo ou acesso para quem? Como contestar uma classe? Que evidência de dano deve obrigar revisão? Classificar é exercer poder sobre atenção e recursos, mesmo sem decisão automática.

### Síntese

Comparar exige unidade, atributos, propósito e definições compatíveis. Igualdade em atributo não é identidade; semelhança depende de critérios. Classificação atribui classes com pertencimento explícito e pode ser sobreposta ou não exaustiva. Desconhecidos permanecem visíveis.

Regularidade pode sustentar padrão candidato, não causa. Regras descritivas, classificatórias e normativas têm estatutos diferentes. Generalização amplia alcance somente dentro de domínio e condições. Exemplos ajudam a interpretar; contraexemplos limitam afirmações; exceções precisam ser declaradas. Caso novo e revisão mostram reutilização responsável.

O percurso não termina quando a regra funciona num caso novo. É preciso registrar a evidência, preservar casos pendentes e continuar autorizado a revisar. Uma classificação útil hoje pode perder adequação se definições, população ou consequências mudarem. Reutilização responsável combina estabilidade suficiente para orientar análise com abertura suficiente para responder a evidências contrárias.

### Mini glossário

**Unidade de comparação:** aquilo que conta como caso.
**Atributo:** característica interpretável usada na comparação.
**Igualdade:** coincidência no atributo declarado.
**Diferença:** distinção relevante segundo critério.
**Semelhança:** proximidade qualitativa segundo propósito e atributos.
**Critério:** condição explícita usada para comparar ou pertencer.
**Classificação:** atribuição de casos a classes por critérios.
**Classe/categoria:** conjunto de casos tratados conjuntamente.
**Pertencimento:** relação entre caso e classe.
**Classificação exclusiva:** atribui uma classe por critério.
**Classificação sobreposta:** permite múltiplas classes.
**Classificação exaustiva:** cobre o universo declarado.
**Caso desconhecido:** caso sem informação necessária.
**Regularidade:** recorrência observada segundo atributos.
**Padrão:** regularidade estruturada e relevante, limitada à evidência.
**Regra descritiva:** formula regularidade observada.
**Regra classificatória:** declara pertencimento.
**Regra normativa:** declara o que deve ocorrer.
**Exemplo:** caso compatível com a regra.
**Contraexemplo:** caso do domínio que contradiz afirmação geral.
**Exceção:** caso excluído por condição explícita e justificada.
**Caso limítrofe:** caso próximo de limite convencional.
**Generalização:** extensão justificada a classe ou caso novo.
**Domínio:** conjunto de casos ao qual a afirmação se aplica.
**Condição de validade:** condição necessária ao uso sustentado.
**Generalização excessiva:** alcance maior que a sustentação.
**Generalização estreita:** alcance que não reutiliza o raciocínio.
**Ajuste excessivo:** regra que memoriza exemplos por detalhes.
**Caso novo:** caso não usado para formular a regra.

### Critérios de domínio

No Nível 1, o aluno reconhece unidade, classe, padrão e contraexemplo. No Nível 2, explica distinções e limites. No Nível 3, classifica e revisa regra com orientação. O início do Nível 4 exige classificação e generalização autônomas em conjunto pequeno: unidade e atributos declarados, sobreposição e desconhecidos preservados, padrão sem causalidade, regra, contraexemplo, domínio, caso novo e revisão.

Isso não declara domínio de C05 em populações complexas, decisões de alto impacto ou contextos que exigem estatística e conhecimento especializado.

## Conexão com a Aula 06 — Representação de problemas e soluções

A Aula 05 produziu atributos, classes, critérios, padrões, regras, exceções e limites. A próxima perguntará como registrá-los sem ambiguidade, quando usar texto, tabela ou diagrama, como converter formas, que informação pode se perder e como manter rastreabilidade.

As tabelas desta aula foram suporte simples. Não comparamos meios nem ensinamos notação, fluxograma ou pseudocódigo; essa seleção pertence à Aula 06.

## Referências, métricas e carga

### Referências utilizadas

- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. DOI: [10.1145/3664191](https://doi.org/10.1145/3664191). Progressão, reconhecimento de padrões e abstração.
- SHUTE, Valerie J.; SUN, Chen; ASBELL-CLARKE, Jodi. Demystifying computational thinking. *Educational Research Review*, v. 22, p. 142–158, 2017. DOI: [10.1016/j.edurev.2017.09.003](https://doi.org/10.1016/j.edurev.2017.09.003). Componentes e avaliação de pensamento computacional, sem taxonomia universal.
- WING, Jeannette M. Computational Thinking. *Communications of the ACM*, v. 49, n. 3, p. 33–35, 2006. DOI: [10.1145/1118178.1118215](https://doi.org/10.1145/1118178.1118215). Abstração e reutilização conceitual, sem definição única de padrões.
- PÓLYA, George. *How to Solve It*. 2. ed. Princeton University Press, 1957. Analogia, casos e revisão, não método universal.
- ROSEN, Kenneth H. *Discrete Mathematics and Its Applications*. 8. ed. McGraw-Hill, 2019. Conjuntos, pertencimento, interseção, partição, relações, funções e contraexemplo.
- LEHMAN, Eric; LEIGHTON, F. Thomson; MEYER, Albert R. *Mathematics for Computer Science*. MIT OpenCourseWare, 2018. Material institucional para conjuntos, relações e contraexemplos, sem antecipar provas.

### Carga estimada

- Estrutura: 15 H2 e 40 H3; 11 exercícios essenciais e sete opcionais.
- Casos: 12 ocorrências e três casos novos na aula; 14 ocorrências, quatro casos novos e quatro transações na prática.
- Fontes: seis.
- Matemática: subconjunto, pertencimento, interseção, partição, conjunto de pendentes, função classificatória e relação de semelhança.
- Leitura e anotações: 2h–2h30.
- Recuperação ativa: 20–30 min.
- Exercícios essenciais: 1h30–2h.
- Prática essencial: 2h30–3h30.
- Solução, revisão e autoavaliação: 30–45 min.
- Trilha essencial: aproximadamente 6h50–9h15.
- Percurso completo opcional: aproximadamente 10h–13h30, com exercícios adicionais, segunda classificação, matemática ampliada, transferência e consequências.
