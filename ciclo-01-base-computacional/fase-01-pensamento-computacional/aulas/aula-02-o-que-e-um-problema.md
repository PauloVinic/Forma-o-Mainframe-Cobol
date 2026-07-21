# Aula 02 — O que é um problema

## Metadados

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo da fase:** De problemas informais a soluções estruturadas
- **Posição:** segunda de 14 aulas
- **Competências introduzidas:** C01 — Formular o problema; C02 — Especificar a transformação
- **Nível esperado:** Nível 2, Nível 3 e início de aplicação autônoma em caso simples e bem delimitado
- **Pré-requisitos conceituais:** sistema, fronteira, dado, informação, processamento, regra, estado, comportamento esperado, evidência, sintoma e causa; panorama de pensamento computacional da Aula 01
- **Prática associada:** `../praticas/pratica-02-formulando-problemas.md`

## Objetivo da aula

Ao final desta aula, o aluno deverá conseguir transformar uma situação vaga, uma necessidade, um sintoma, um risco ou uma oportunidade em uma formulação inicial delimitada, analisável e verificável. Para isso, deverá separar o que foi observado do que foi inferido, manter hipóteses causais como hipóteses, identificar interessados e pessoas afetadas, declarar objetivos e estados, estabelecer escopo e condições, e propor critérios que permitam avaliar resultados sem escolher antecipadamente uma solução.

A aula introduz C01 e C02 em explicação, aplicação guiada e autonomia inicial em caso simples. Não exige domínio complexo nem produz especificação completa, modelo detalhado ou algoritmo.

## O problema que esta aula resolve

Frases como “o sistema está lento”, “os clientes reclamam” ou “precisamos de inteligência artificial” podem apontar algo relevante, mas misturam sintoma, explicação e solução. Termos como “muito” não definem população ou período; uma causa convincente pode continuar sendo hipótese.

Agir sobre essa mistura pode corrigir o componente errado, otimizar métrica inadequada, excluir pessoas afetadas ou transformar preferência em restrição. Formular é explicitar o que se sabe e pretende, para quem, em quais limites e por quais sinais uma resposta será avaliada. Questões abertas e soluções alternativas permanecem visíveis.

## Ponte com a Aula 01 e a Fase 0

A Aula 01 comparou necessidade vaga, procedimento informal e formulação inicial. Agora aprofundaremos o primeiro movimento: formular antes de decompor, representar ou construir procedimentos.

Da Fase 0, retomamos sistema, fronteira, dado contextualizado, processamento, regra, estado, comportamento esperado, evidência, sintoma e causa. A fronteira ajuda a delimitar escopo; dados podem sustentar evidência; entradas, saídas, regras e estados descrevem a transformação esperada em nível inicial. Esses conceitos não serão ensinados novamente, nem se presumirá que todo problema requer software.

## Caso de abertura — falta de produtos não é uma formulação

Retomemos o estoque da Aula 01. Uma rede de distribuição declara:

> Precisamos evitar que os centros fiquem sem produtos. A solução é comprar uma ferramenta de previsão.

A situação envolve centros, pedidos, registros e disponibilidade. A necessidade expressa é evitar falta. “Ficar sem” é um possível sintoma, mas ainda não possui definição operacional: saldo físico igual a zero, saldo disponível insuficiente para um pedido ou ruptura percebida pelo cliente são eventos diferentes. A ferramenta de previsão é uma solução proposta, não uma parte necessária do problema.

Registros quantitativos tornarão a situação mais informativa, mas não demonstrarão sozinhos causa ou impacto. A formulação progressiva deverá situar a observação, identificar perspectivas, delimitar recorte e preservar perguntas sobre contagem, comparabilidade e autoridade, sem dividir o processo nem desenhar solução.

## Situação, necessidade, problema e solução

Uma **situação** é o contexto no qual algo ocorre ou pode ocorrer. Ela pode conter pessoas, sistemas, eventos, condições e interpretações, sem que exista ainda um único problema aceito. “Uma organização recebe pedidos por canais diferentes” descreve uma situação. Situações não são boas ou ruins por natureza; tornam-se relevantes conforme objetivos, efeitos e perspectivas.

Uma **necessidade** expressa algo considerado necessário ou valioso por alguém: reduzir exposição a risco, obter resposta, preservar um direito, aproveitar uma oportunidade. “O solicitante precisa saber se o benefício foi concedido” é uma necessidade. Ela revela propósito, mas talvez não informe a diferença observada, o escopo ou a condição que demonstraria atendimento.

Nesta formação, adotaremos a seguinte definição operacional:

> **Problema é um objeto delimitado de análise que envolve uma diferença, um obstáculo, um risco, uma incerteza relevante, uma decisão necessária, uma necessidade não atendida ou uma oportunidade de melhoria. Sua formulação relaciona a situação a interessados e objetivos e torna explícitos, na medida necessária, estado atual e pretendido, evidências, escopo, condições, restrições, pressupostos, questões em aberto e critérios pelos quais respostas poderão ser avaliadas.**

Essa é uma convenção pedagógica ampla, não uma definição universal nem uma descrição neutra e total da realidade. Formular seleciona uma perspectiva e uma fronteira. Por isso, a formulação deve ser justificável, revisável e proporcional ao uso. Quando o estado desejado ou a causa ainda não forem conhecidos, a resposta correta é registrar a lacuna, não inventá-los.

“Objeto delimitado” nomeia o recorte que a formulação procura construir; não supõe que a situação original chegue delimitada nem que a primeira versão seja final.

Uma **solução proposta** é uma alternativa de intervenção: mudar uma regra, treinar pessoas, reorganizar trabalho, adquirir ferramenta, criar software ou decidir não intervir. Ela será avaliada em relação ao problema; não deve ser incorporada silenciosamente à definição. “Não temos um chatbot” descreve ausência de uma tecnologia. O problema pode ser que usuários não consigam obter respostas confiáveis no prazo necessário — e talvez a melhor resposta não seja um chatbot.

As quatro noções se relacionam, mas não são etapas mecânicas. Uma situação pode conter várias necessidades; interessados podem formular problemas diferentes a partir dela; um problema pode admitir múltiplas soluções; e a investigação pode revelar que a intervenção proposta não é necessária.

## Problema, pergunta, decisão, risco e oportunidade

Nem todo objeto de análise começa com uma diferença já observada. Uma **pergunta** solicita conhecimento: “qual é a taxa de solicitações devolvidas?”. Respondê-la pode apoiar a formulação, mas a pergunta sozinha não informa por que a taxa importa ou que ação será considerada. Uma **decisão** é uma escolha que alguém precisa fazer entre alternativas, como manter ou mudar um prazo. O problema deve mostrar contexto, objetivos e critérios que tornam essa decisão necessária.

Um **risco** combina a possibilidade de um evento ou condição futura com consequências relevantes e incerteza. “Pode haver pagamento duplicado quando mensagens são reenviadas” não afirma que duplicidades já ocorreram; ainda assim, pode justificar análise preventiva. Uma **oportunidade** é uma possibilidade de produzir valor ou melhorar um estado, mesmo sem falha presente: por exemplo, permitir que pessoas acompanhem uma solicitação sem telefonar. Não é preciso fabricar uma reclamação para formular uma oportunidade.

Esses enquadramentos podem coexistir: demora observada, aumento previsto da demanda, acompanhamento e escolha de capacidade podem representar problema atual, risco, oportunidade e decisão. Declare qual objeto ocupa o centro e como os demais o apoiam; reuni-los sob um rótulo esconde a evidência e a avaliação necessárias.

## Sintoma, causa e hipótese causal

Um **sintoma** é uma manifestação percebida ou registrada de uma condição que merece atenção. Filas longas, devoluções frequentes, divergência de saldo e reclamações repetidas podem ser sintomas. O sintoma é informativo; o erro é tratá-lo como explicação suficiente. “A tela trava” informa o que foi percebido, mas não identifica o mecanismo responsável.

Uma **causa** é um fator que contribuiu para produzir um evento ou condição. Em contextos sociotécnicos, efeitos raramente dependem de uma causa isolada. Regras, dados, carga de trabalho, treinamento, comunicação, incentivos e tecnologia podem interagir. Atribuir causa exige uma relação sustentada por evidências adequadas e uma explicação compatível com o caso. Correlação temporal ou relato de uma pessoa pode iniciar a investigação, mas não encerra a questão.

Uma **hipótese causal** é uma explicação provisória que pode orientar busca de evidências. Se parte das solicitações demora após ser reatribuída, pode-se formular: “reatribuições contribuem para o tempo sem ação”. A hipótese deve indicar que observações a fortaleceriam ou enfraqueceriam: comparar tempos de casos semelhantes com e sem reatribuição, verificar a ordem dos eventos e examinar exceções. “A equipe é desorganizada” não é uma boa hipótese: é amplo, culpabilizante e difícil de examinar.

Uma **causa confirmada** é uma contribuição sustentada no recorte; não precisa ser única, suficiente ou necessária. **Correlação** indica associação, enquanto **coincidência** é coocorrência sem relação sustentada. Uma explicação apenas plausível continua hipótese. Condições técnicas e organizacionais podem contribuir juntas. O sintoma oferece evidência da manifestação, não sua explicação completa.

Necessidade, sintoma e causa ocupam papéis distintos. “Receber resposta previsível” é necessidade; “38% passaram de cinco dias” é sintoma quantificado; “pendências documentais explicam parte da demora” é hipótese até que o alcance da relação seja investigado. A formulação pode avançar sem causa confirmada. Ela deve dizer o que se observa, que explicações estão em exame e que decisões não dependem de fingir certeza.

## Evidência, fato, inferência, hipótese e decisão

Uma formulação rastreável distingue o estatuto das afirmações. **Evidência** é o material usado para sustentar ou contestar uma afirmação: registros, documentos, observações, medições, relatos, normas ou resultados de comparação. Ela possui origem, período, método e limitações. Um relatório pode ser evidência mesmo incompleto; a incompletude limita o que se conclui.

Chamaremos de **fato do caso** uma afirmação tratada como observada ou estabelecida dentro do recorte, sempre vinculada à evidência disponível. “O registro técnico marca indisponibilidade entre 10h e 13h” pode ser fato do caso. Isso não prova que a indisponibilidade causou todas as demoras. Em outros contextos, novas evidências podem revisar o que antes era aceito.

Uma **inferência** é uma conclusão derivada dos fatos por raciocínio. Se 95 de 500 solicitações foram devolvidas, inferimos uma taxa de 19%, desde que numerador e denominador sejam comparáveis. Se o relatório inclui apenas casos encerrados, inferir o comportamento de todos os recebidos pode ser indevido. A inferência precisa mostrar sua base e seu alcance.

Uma **hipótese** é uma afirmação ainda não estabelecida, mantida para exame. Ela pode ser causal, mas também pode tratar de necessidade, comportamento futuro ou qualidade dos dados. Uma **decisão** é uma escolha autorizada, como testar uma nova distribuição de trabalho por uma semana. Decisão não prova hipótese; no máximo, pode criar uma oportunidade de observação.

Considere elementos hipotéticos do estoque:

| Afirmação | Estatuto principal | Limite |
|---|---|---|
| tabela de linhas solicitadas e não atendidas | evidência disponível | definições e completude limitam seu uso |
| 192 de 2.400 linhas não foram atendidas integralmente | fato do caso | vale apenas no recorte declarado |
| a taxa total no período é 8% | inferência aritmética | depende de numerador e denominador comparáveis |
| saldo desatualizado contribuiu para as ocorrências | hipótese causal | sequência dos eventos ainda precisa ser examinada |
| a gestão propõe taxa inferior a 3% | decisão ou proposta | não a torna meta validada nem prova causa |

Um sintoma pode ser fato; uma causa alegada pode ser hipótese; uma evidência pode sustentar apenas parte de uma inferência. Portanto, este eixo não substitui as distinções anteriores. Ele informa quanto apoio cada afirmação possui e o que ainda precisa ser investigado.

## Interessados, pessoas afetadas e responsabilidade pela decisão

Um **interessado** é uma pessoa, grupo ou instituição que possui interesse, responsabilidade, influência ou exposição relevante em relação ao problema ou às respostas. Solicitantes, operadores, gestores, áreas de controle, fornecedores, reguladores e equipes técnicas podem ocupar esse papel. A lista deve nascer do caso, não de um formulário preenchido por hábito.

Uma **pessoa afetada** sofre efeitos do estado atual ou de uma intervenção, ainda que não tenha poder, contrato ou participação na reunião. Quem abandona uma fila antes de ser atendido pode desaparecer da métrica e da discussão, embora seja diretamente afetado. Familiares, trabalhadores terceirizados ou pessoas com barreiras de acesso também podem ficar invisíveis quando “o usuário” é tratado como perfil homogêneo.

O **responsável pela decisão** possui autoridade para aprovar ou rejeitar encaminhamento. Não é necessariamente solicitante, usuário, operador, especialista do domínio ou responsável técnico. Esses papéis fornecem perspectivas diferentes; a autoridade competente decide metas e aceita riscos.

Interessados podem discordar legitimamente. Em um serviço de atendimento, usuários desejam previsibilidade e pouca espera; atendentes precisam de regras aplicáveis e tratamento de exceções; gestão observa capacidade e custo; auditoria requer rastreabilidade; pessoas prioritárias precisam de proteção sem exposição indevida. Formular o problema não elimina a divergência. Registra perspectivas, identifica quem não foi ouvido e declara como decisões serão tomadas.

## Objetivo, estados e resultado esperado

O **objetivo** descreve a mudança de valor procurada e responde por que o problema merece ação. “Reduzir devoluções que exigem novo envio, preservando correção e conformidade” é objetivo. “Implantar validação automática” é uma intervenção, não o objetivo final. Um objetivo pode continuar qualitativo no início, desde que posteriormente seja relacionado a observações e critérios.

O **estado atual** descreve condições relevantes no recorte presente ou de referência. Deve usar evidências e declarar limites: “no mês analisado, 95 de 500 solicitações foram devolvidas para correção”. Não é uma narrativa de tudo o que existe no sistema. O **estado desejado** descreve condições pretendidas: menor devolução, resposta dentro de faixa acordada e ausência de piora em correção. Ele não precisa antecipar como a transição acontecerá.

O **resultado esperado** é um efeito observável que indicaria progresso em direção ao objetivo. Ele difere de uma saída produzida por um processo. Um aviso enviado é saída; redução de solicitações sem resposta é resultado. Um relatório gerado é saída; capacidade de reconstruir decisões pode ser resultado. A relação pode ser resumida assim:

| Elemento | Pergunta central | Exemplo |
|---|---|---|
| objetivo | por que mudar? | reduzir retrabalho sem prejudicar conformidade |
| estado atual | que condição relevante foi observada? | 19% das solicitações foram devolvidas no mês |
| estado desejado | que condição se pretende alcançar? | devoluções menos frequentes e respostas previsíveis |
| resultado esperado | que efeito deve aparecer? | menos reenvios e menor tempo até resposta válida |

Estado desejado não significa um futuro perfeito. Pode envolver faixas aceitáveis e proteções. Também não é legítimo deduzi-lo apenas do estado atual: saber que a espera mediana é 42 minutos não torna 25 minutos a meta correta. A meta precisa ser negociada com responsáveis, comparada à linha de base e examinada quanto a efeitos colaterais.

## Escopo e fronteira

O **escopo** declara que parte da situação será analisada e avaliada: população, unidades, produtos, eventos, período, canal e resultado incluídos. Suas **exclusões** dizem o que não pertence ao trabalho atual. “Três produtos críticos, dois centros, linhas solicitadas durante ciclos de 28 dias” é mais útil que “estoque da empresa”. Declarar exclusões não torna o restante irrelevante; impede apenas que a formulação prometa tratar tudo de uma vez.

A **fronteira** separa o objeto formulado de seu ambiente para um propósito. Ela permite perguntar quais eventos atravessam o limite, quem fornece entradas e quem recebe efeitos. Em um problema de benefício, o recebimento da solicitação pode iniciar a medição e a primeira resposta válida pode encerrá-la. Se uma pendência externa pausa o prazo, essa condição precisa ser explícita. Mover a fronteira muda numeradores, responsabilidades e conclusões.

Escopo e fronteira se relacionam, mas não são sinônimos perfeitos. O escopo lista o que o trabalho abrange; a fronteira ajuda a pensar dentro, fora e interações relevantes. Nesta aula, basta declará-los em linguagem natural. Escolher representações detalhadas e modelar componentes será trabalho posterior.

O recorte deve ser relevante, justificável e observável. Um recorte estreito pode deslocar consequências: enviar resposta vazia reduz tempo sem atender a necessidade. Um recorte amplo pode ser impraticável. A fronteira é escolha revisável.

## Restrições, recursos, preferências e pressupostos

Uma **restrição** limita alternativas admissíveis. Pode decorrer de lei, contrato, segurança, prazo, orçamento, capacidade física ou decisão válida: “a área física não poderá ser ampliada nos próximos seis meses”. Uma restrição precisa de origem e alcance. “Tem de usar planilha” pode ser restrição se uma condição externa realmente o exigir; caso contrário, talvez seja apenas solução presumida.

Um **recurso** é um meio disponível: pessoas, tempo, dados, orçamento, equipamentos ou autoridade. “Um analista está disponível oito horas por semana durante seis semanas” declara recurso. Sua quantidade limitada também condiciona o que é viável, mas é útil registrar o que existe, e não apenas o que falta.

Uma **preferência** favorece uma alternativa sem torná-la obrigatória. Uma equipe pode preferir conservar a interface conhecida ou evitar treinamento no mesmo mês. Preferências importam, porém podem ser negociadas e comparadas a objetivos. Disfarçá-las como restrições elimina alternativas sem justificativa.

Um **pressuposto** é uma condição aceita provisoriamente para permitir avanço: por exemplo, supor que dois centros usam a mesma definição de “linha não atendida”. O pressuposto não é fato escondido. Deve ser explícito, acompanhado de consequência e, quando relevante, de forma de verificação. Se as definições diferirem, a comparação e a meta terão de ser revistas.

Compare: “o regulamento proíbe armazenar esse dado” é restrição; “há registros dos últimos seis meses” é recurso; “a gestão prefere manter o canal atual” é preferência; “os registros usam identificadores comparáveis” é pressuposto. Uma mesma condição pode mudar de categoria quando sua base muda. Classificar ajuda a perguntar quem a estabeleceu, quão firme ela é e o que acontece se estiver errada.

## Entradas, saídas, regras e condições

Uma formulação inicial de transformação pergunta o que entra, o que deve sair, que regras governam o domínio e sob quais condições a expectativa vale. Esses elementos introduzem C02 sem descrever ainda uma sequência de execução.

**Entrada** é dado, material, evento ou solicitação recebido pelo objeto em análise. Um pedido com itens e quantidades, um formulário acompanhado de documentos e a chegada de uma pessoa à fila são exemplos. **Saída** é algo produzido ou emitido: uma decisão registrada, uma notificação, uma reserva ou uma resposta. Entrada não é sinônimo de evidência; o documento recebido pode ser entrada do processo e, quando examinado, evidência para uma afirmação.

Uma **regra** estabelece relação, proibição ou obrigação no domínio. Uma **condição** é circunstância de aplicabilidade; uma **pré-condição** precisa valer antes que a transformação esperada se aplique. Condição não é pressuposto aceito provisoriamente. Sua expressão lógica será estudada depois.

Restrições limitam o espaço de resposta; regras governam comportamento ou decisões; condições delimitam quando uma afirmação vale. Há sobreposição possível, mas a pergunta prática muda. “Não expor dado sensível” restringe qualquer solução. “A prioridade deve ser registrada” governa o serviço. “Quando houver risco imediato, a prioridade pode ser alterada por autoridade identificada” declara condição de aplicação.

Esses elementos são identificados quando aplicáveis; uma investigação pode não ter entradas ou saídas completas. Listá-los não produz algoritmo: ainda faltam ordem, decisões, repetição e tratamento de dados. O objetivo é apenas examinar se uma resposta atende ao problema.

## Critério de sucesso, métrica, meta e linha de base

Um **critério de sucesso** é condição observável, quantitativa ou qualitativa, usada para avaliar o resultado. Quando aplicável, declara população, período e método; inclui proteção quando houver risco de dano ou otimização unilateral. “Melhorar o atendimento” não basta. Manter abandono abaixo do limite acordado sem aumentar espera extrema é verificável quando recorte e medição são definidos.

Uma **métrica** é uma forma de medir um atributo: taxa de devolução, mediana de espera, quantidade de ajustes posteriores. Métrica não é objetivo e não é automaticamente um bom critério. A média pode esconder extremos; a mediana pode excluir quem abandonou; “número de tickets fechados” pode incentivar encerramentos prematuros. A escolha precisa corresponder à necessidade.

Uma **meta** atribui valor ou faixa pretendida a uma métrica: taxa menor que 3%, mediana no máximo 25 minutos. Ela expressa decisão ou compromisso, não fato científico nem garantia de qualidade. É preciso saber quem a aprovou, por que é aceitável e quais efeitos não podem piorar. Uma **linha de base** é o valor de referência obtido antes da mudança ou em período comparável. Sem ela, “reduzir em 30%” não tem ponto de partida claro.

Quando há risco relevante, critérios principais precisam de **critérios de proteção**. Se o objetivo é reduzir tempo, proteções podem limitar erro, abandono, exposição de dados ou tratamento desigual. Se o objetivo é reduzir ruptura de estoque, proteções podem acompanhar perda, custo e transferência do problema a outros produtos. Satisfazer uma meta isolada pode piorar o sistema; sucesso é um julgamento sustentado por um conjunto coerente de evidências.

A matemática torna limites explícitos, mas não decide se eles são adequados. Suponha que `r` represente a taxa de linhas não atendidas no escopo e no período definidos. O critério `r < 3%` significa que a taxa deve ser **menor que**, e não igual a, 3%. Já `r ≤ 3%` inclui o valor 3%. Os símbolos `<`, `>`, `≤`, `≥` e `=` significam, respectivamente, menor, maior, menor ou igual, maior ou igual e igual.

Uma taxa precisa de definição. Se `n` é o número de ocorrências e `N > 0` o número de unidades comparáveis, então `r = n/N`. Para 192 ocorrências em 2.400 linhas, `r = 192/2.400 = 0,08 = 8%`. A igualdade não informa impacto nem causa. É preciso definir contagem, cancelamentos e período.

Intervalos representam faixas. A escrita `t ∈ [0, 5]` indica que o tempo `t` pertence ao intervalo de zero a cinco unidades, incluindo os extremos; os colchetes incluem 0 e 5. Em `t ∈ (0, 5)`, os parênteses excluem ambos. Assim, cinco dias satisfaz `t ≤ 5`, mas não satisfaz `t < 5`. Nesta aula, a notação serve apenas para ler fronteiras; critérios reais precisam definir quando a contagem começa, quando termina, que calendário usam e como tratam pausas.

Um conjunto simples explicita valores admissíveis. Se `D = {identidade, residência, renda}` representa tipos de documento aceitos em certo recorte, `d ∈ D` significa que o tipo `d` pertence ao conjunto. Isso não afirma que toda solicitação exige os três documentos nem que o conjunto está correto. A regra de aplicabilidade continua necessária.

Linha de base e meta devem compartilhar método. Se a linha de base é `r₀ = 8%` e a meta candidata é `r < 3%`, a comparação só faz sentido com população, evento, período e contagem compatíveis. Uma redução aparente obtida excluindo casos difíceis não demonstra melhora. Notação precisa não corrige definição ruim, fonte incompleta, meta arbitrária ou efeito colateral ignorado.

## Objetivos conflitantes e efeitos colaterais

Problemas reais raramente possuem um único objetivo sem tensão. Reduzir espera pode elevar custo; aumentar controles pode dificultar acesso; manter estoque maior pode reduzir ruptura e aumentar perdas; automatizar decisões pode acelerar respostas e enfraquecer contestação. O conflito não prova que um objetivo é ilegítimo. Exige responsáveis, prioridades e proteções explícitas.

Considere 600 senhas hipotéticas emitidas em cinco dias: 540 atendimentos concluídos, mediana de espera de 42 minutos e 60 abandonos. Uma proposta de atender primeiro os casos rápidos pode reduzir a mediana entre concluídos, enquanto aumenta a espera extrema e exclui pessoas que saíram da fila. Se a métrica ignora abandonos, o resultado parece melhor justamente quando parte do público desaparece do denominador.

Um **efeito colateral** é consequência relevante produzida junto do efeito pretendido. Deve ser antecipado como possibilidade, não declarado como certeza sem evidência. Critérios de proteção tornam algumas consequências observáveis: acompanhar percentil elevado de espera, taxa de abandono, correção de decisões e possibilidade de revisão. Outros efeitos requerem relato qualitativo e participação das pessoas afetadas.

Formular não resolve o conflito por fórmula. A equipe documenta perspectivas, evidencia trocas, propõe critérios e identifica quem tem autoridade para decidir. Não há problema “bem formulado” apenas porque um número foi otimizado. Há uma formulação responsável quando valores e consequências deixam de ficar escondidos.

## Problemas mal definidos e formulação iterativa

Um problema é frequentemente chamado de **mal definido** ou **pouco estruturado** quando objetivos, condições, estados, critérios ou meios relevantes estão incompletos, ambíguos, instáveis ou em conflito. Isso não significa que seja falso, sem importância ou culpa de quem o relatou. Pode refletir novidade, múltiplas perspectivas e informação que só aparece durante a investigação.

Herbert Simon mostrou que problemas pouco estruturados não formam simplesmente uma classe oposta e perfeitamente separada dos bem estruturados; faltas de definição podem ocorrer em diferentes aspectos e graus. Para esta aula, a consequência pedagógica é simples: não use “mal definido” como rótulo final. Identifique o que está indefinido. O objetivo muda? A população é desconhecida? Há disputa sobre critérios? A evidência é incompleta? Cada lacuna sugere uma pergunta diferente.

Formulação é **iterativa**. Uma primeira versão permite coletar evidências e ouvir pessoas; essas descobertas alteram escopo, pressupostos ou metas; a versão seguinte registra a mudança. Iterar não é reescrever até parecer completo, nem adiar indefinidamente a ação. É manter rastreabilidade: qual afirmação mudou, com base em quê e com qual efeito sobre a decisão.

Questões em aberto são parte legítima da formulação: “casos pendentes foram excluídos do relatório?”, “quem pode aprovar a meta?”, “as categorias se sobrepõem?”. Uma lacuna conhecida é mais segura que uma certeza inventada. A formulação torna a incerteza administrável sem prometer eliminá-la.

Se nem contexto, necessidade ou perspectiva relevante e alguma base examinável puderem ser identificados, ainda não há informação suficiente para uma formulação inicial. O produto adequado é um conjunto de perguntas de esclarecimento, não afirmações inventadas.

## Problema, requisito e especificação

A Fase 0 distinguiu necessidade, objetivo, requisito, regra de negócio e especificação. Aqui retomamos apenas a fronteira necessária. A formulação do **problema** descreve por que e em que condições uma mudança ou decisão importa. Um **requisito** declara uma capacidade, propriedade ou condição que um sistema, serviço ou produto deverá satisfazer. Uma **especificação** organiza requisitos e outras informações de forma apropriada para construção, aquisição, verificação ou acordo.

“Solicitantes precisam conhecer o estado do pedido sem telefonar” expressa necessidade. “Há 38% de pedidos sem atualização por mais de cinco dias no recorte medido” contribui para o problema. “O serviço deve disponibilizar o estado atual a solicitantes autorizados” pode tornar-se requisito, após validação. Regras de identidade, proteção e prazo governam essa capacidade. Uma especificação precisará tratar detalhes, exceções, interfaces e critérios que esta aula não cobre.

A engenharia de requisitos é iterativa e envolve elicitação, análise, conflitos, especificação, validação e gestão. A ISO/IEC/IEEE 29148 e o SWEBOK organizam esse campo profissional. A Aula 02 não o comprime em uma ficha. Ela produz um antecedente útil: uma formulação inicial que não transforma ferramenta em requisito nem trata a primeira fala do solicitante como especificação pronta.

## Um modelo didático de formulação

Para estudar C01 e C02, usaremos um quadro de perguntas, não um formulário universal:

| Bloco | Perguntas de apoio |
|---|---|
| contexto e relevância | que situação, necessidade, risco, decisão ou oportunidade motivou a análise, e para quem? |
| base conhecida | que evidências e fatos existem; que inferências, hipóteses e decisões devem permanecer separadas? |
| transformação pretendida | quais estados atual e desejado, objetivo, entradas, saídas, regras e condições são relevantes? |
| delimitação | que população, período, unidades e eventos estão no escopo; o que fica excluído; onde está a fronteira? |
| viabilidade e responsabilidade | quais restrições, recursos, preferências e pressupostos existem; quem é afetado e quem decide? |
| avaliação | quais resultados, métricas, metas candidatas, linha de base, critérios de sucesso e proteções serão usados? |
| incerteza e alternativas | que questões continuam abertas e que soluções sugeridas devem ficar fora do enunciado do problema? |

Uma declaração flexível pode assumir esta forma: “No contexto e escopo **X**, a evidência **E** indica a condição atual **A**, relevante para **I**. Pretende-se alcançar **D** por causa do objetivo **O**, sob as condições e limites **L**, avaliando **C** e protegendo **P**. As hipóteses **H** e questões **Q** permanecem em exame; nenhuma solução foi ainda escolhida.” Nem todo caso exige essa ordem ou todos os campos na mesma frase. A qualidade está nas relações justificadas, não no preenchimento mecânico.

Perguntas de Pólya sobre incógnita, dados e condições inspiram esclarecimento, não uma sequência universal. O CS2023 sustenta a progressão por competências e o tratamento explícito de formulação e ambiguidade.

## Caso progressivo — formulação inicial do estoque

No caso hipotético de abertura, sabemos que, durante 28 dias, 192 de 2.400 linhas de três produtos críticos não foram atendidas integralmente na primeira separação: 84 de 1.400 no CD Norte e 108 de 1.000 no CD Sul. Em 29 ocorrências falta histórico completo. Há hipóteses sobre saldo desatualizado e entradas atrasadas, mas os grupos observados podem se sobrepor e nenhuma causa foi confirmada. A gestão sugeriu taxa inferior a 3% por centro durante três ciclos; a meta ainda requer aprovação.

Uma formulação inicial possível é:

> Nos três produtos e dois centros incluídos, 192 de 2.400 linhas não foram atendidas integralmente na primeira separação durante 28 dias, com taxas calculadas de 6% no CD Norte e 10,8% no CD Sul. Pretende-se reduzir a ocorrência de modo sustentado; perdas, custo, divergências e deslocamento para outros produtos são proteções candidatas a validar. A taxa inferior a 3% em cada centro por três ciclos é meta candidata, não requisito validado. A formulação pressupõe provisoriamente critérios de contagem comparáveis e mantém abertas a qualidade dos registros, o impacto ao cliente, as causas, as linhas de base das proteções e a autoridade sobre a meta. Aumento de estoque, redistribuição, correção de registros e ferramenta de previsão permanecem alternativas não avaliadas.

A formulação é verificável sem fingir completude: contém observação, recorte, objetivo, proteção e incerteza. Ela não divide compras, armazenagem e separação, não desenha fluxo e não escolhe intervenção. Esse trabalho permanece disponível para as próximas aulas.

## Prática guiada — reformular sem inventar

Considere a solicitação hipotética: “Compre um sistema com inteligência artificial para aprovar automaticamente 80% dos reembolsos”. No último mês, 500 solicitações foram recebidas; 95 voltaram para correção, a mediana até a primeira resposta foi de seis dias úteis e 18 aprovações exigiram ajuste posterior. Uma referência interna menciona quatro dias, mas não define início, término nem exceções.

Antes de ler o comentário, anote: fatos; inferências; hipóteses; objetivo possível; interessados e afetados ausentes; escopo; critérios e questões abertas. Depois escreva duas frases sem nomear tecnologia.

Comentário: `95/500 = 19%` é inferência quantitativa se os registros forem comparáveis. “A inteligência artificial resolverá” não é fato nem causa demonstrada. Um objetivo possível é reduzir retrabalho e tempo até resposta válida sem prejudicar correção, conformidade, contestação e proteção de dados. Quatro dias e 80% são números propostos, não critérios legitimados. Ainda faltam definições de medição, população, autoridade e impacto. Uma boa reescrita preserva essas lacunas e mantém sistema novo, automação e mudança de regra como alternativas.

## Confusões recorrentes e critérios de qualidade

Repetir a reclamação preserva ambiguidade; repetir a solução elimina alternativas; registrar apenas o sintoma não explica o objeto; declarar causa sem evidência produz falsa certeza. Lista de desejos, número isolado e formulário preenchido não substituem raciocínio, nem é preciso ocultar incerteza para avançar.

Revise uma formulação perguntando se ela é relevante para interessados identificados, rastreável a evidências, neutra quanto a soluções ainda não escolhidas, delimitada, internamente coerente, verificável e revisável. Verifique também se distingue preferências de restrições, torna pressupostos visíveis, registra pessoas afetadas ausentes e inclui efeitos a proteger. A formulação deve ser suficiente para a próxima decisão, não uma descrição total da realidade.

## Exercícios

As questões 1 a 3 são objetivas. Justifique a escolha e explique por que as demais são inadequadas, ainda que contenham algum elemento plausível.

1. Um gestor pede um chatbot porque usuários esperam por respostas. Qual formulação inicial é mais adequada? **a)** a ausência do chatbot; **b)** a diferença observada entre o tempo atual e o aceitável, no recorte definido, sem assumir tecnologia; **c)** perguntas repetidas como causa confirmada; **d)** padronizar respostas pela ferramenta como requisito já aprovado.
2. Um relatório registra 240 cobranças duplicadas; a equipe afirma que uma integração pode estar reprocessando mensagens; a gestão decide suspender reenvios durante a investigação. Qual sequência classifica melhor as afirmações? **a)** fato do caso, hipótese causal, decisão; **b)** hipótese, evidência, causa; **c)** sintoma, decisão, evidência; **d)** causa, inferência, requisito.
3. O objetivo é reduzir cadastros inválidos. Qual candidato é mais verificável? **a)** implantar validação automática; **b)** melhorar bastante a qualidade; **c)** reduzir a taxa de 7% para no máximo 2% em dois ciclos, usando a mesma regra de medição e proteção contra rejeições indevidas; **d)** alcançar 80% de satisfação com a interface.

Responda discursivamente:

4. Em uma situação na qual pessoas não recebem atualização de uma solicitação, diferencie situação, necessidade, problema e solução proposta.
5. Explique por que um sintoma não demonstra sua causa e como uma hipótese causal pode orientar a coleta de evidência.
6. Relacione objetivo, estado atual, estado desejado, resultado esperado e critério de sucesso sem tratá-los como sinônimos.
7. Mostre como interessado, pessoa afetada, responsável pela decisão, escopo, restrição e recurso podem mudar uma formulação.
8. Diferencie entrada, saída, regra e condição e explique por que listá-las ainda não constitui algoritmo.

Analise os casos:

9. Um cadastro possui 70 campos vazios em 1.000 registros. A equipe diz que “usuários são descuidados” e pede campos obrigatórios. Separe fato, inferência, hipótese, julgamento indevido, lacuna e solução presumida.
10. Após uma indisponibilidade de três horas, 90 solicitações atrasaram; outras 290 atrasadas não atravessaram o evento. Formule sintoma, hipótese causal limitada, evidência adicional necessária e decisão provisória que não declare causa.
11. Em uma fila, gestão quer reduzir mediana, usuários querem previsão, auditoria quer rastreabilidade e pessoas que abandonaram não foram ouvidas. Identifique dois conflitos, uma pessoa afetada ausente, um responsável plausível pela decisão e dois critérios de proteção.
12. No estoque progressivo, preencha os sete blocos do modelo didático. Preserve como abertas a causa, a qualidade dos registros e a aprovação da meta; não divida o processo em etapas.

13. Considere `r ≤ 2%`, `t ∈ [0, 5]` dias e `D = {identidade, residência, renda}`. Explique os símbolos, diga se `r = 2%` e `t = 5` satisfazem os limites, dê um exemplo de `d ∈ D` e indique quatro definições contextuais necessárias antes de usar esses critérios.
14. Construa um contraexemplo para a afirmação “se o critério é numérico, o problema está bem formulado”. Use uma métrica precisa que meça o aspecto errado ou incentive consequência indesejada.
15. Reescreva “instale inteligência artificial para acabar com reclamações” em 150 a 220 palavras. Inclua fatos fornecidos ou lacunas explícitas, objetivo, estados, interessados, escopo, restrições, critério provisório e proteção. Não invente causa nem mantenha a ferramenta no problema.

### Orientações de correção

Nas objetivas, procure a alternativa que separa problema, evidência, hipótese, decisão, solução e critério; palavras numéricas isoladas não bastam. Nas discursivas, exija relações e exemplo. Nos casos, aceite formulações diferentes quando rastreáveis ao enunciado. Na matemática, verifique fronteiras e contexto. No contraexemplo e na reescrita, avalie se o aluno preserva alternativas, efeitos e questões abertas. Não há uma frase única de gabarito.

## Recuperação ativa, síntese e mini glossário

### Recuperação ativa e reflexão

Sem consultar o texto, responda: qual a diferença entre situação e problema? Por que sintoma não é causa? O que separa hipótese causal de causa confirmada? Por que solução não deve entrar silenciosamente na formulação? Como escopo e fronteira se relacionam? Qual a diferença entre restrição e recurso? Como objetivo, métrica e meta diferem? Por que atingir uma métrica pode não resolver o problema? Quando manter uma questão em aberto? O que torna um critério verificável?

Reflita sobre quem tem poder para formular e decidir. Como pessoas afetadas ausentes, metas inadequadas, automação prematura, objetivos conflitantes e responsabilidade indefinida mudariam um caso de seu trabalho?

### Síntese

Formular um problema é construir um objeto delimitado e revisável para análise. A formulação relaciona situação, necessidade, evidência, interessados, objetivos, estados, escopo, condições e critérios. Ela separa sintoma de causa, fato de hipótese, meta de objetivo e restrição de preferência. Não elimina incerteza nem escolhe ferramenta: torna escolhas visíveis, permite avaliar respostas e prepara o todo para decomposição posterior.

### Mini glossário

| Termo | Definição breve |
|---|---|
| situação | contexto no qual algo ocorre ou pode ocorrer |
| necessidade | condição considerada necessária ou valiosa por alguém |
| problema | objeto delimitado de análise diante de diferença, obstáculo, risco, incerteza, decisão, necessidade ou oportunidade |
| sintoma | manifestação percebida ou registrada |
| causa | fator sustentado como contribuinte de um efeito |
| hipótese causal | explicação provisória e examinável sobre causa |
| evidência | material que sustenta ou contesta afirmação |
| inferência | conclusão derivada de evidências por raciocínio |
| objetivo | mudança de valor que se procura |
| interessado | quem possui interesse, responsabilidade, influência ou exposição |
| pessoa afetada | quem sofre efeitos, mesmo sem poder decisório |
| estado atual | condição relevante observada no recorte de referência |
| estado desejado | condição que se pretende alcançar |
| escopo | população, período e elementos abrangidos pelo trabalho |
| fronteira | limite entre objeto formulado e ambiente |
| restrição | limite obrigatório sobre alternativas admissíveis |
| recurso | meio disponível para análise ou ação |
| preferência | alternativa favorecida, mas negociável |
| pressuposto | condição provisoriamente aceita e revisável |
| entrada | dado, material, evento ou solicitação recebida |
| saída | elemento produzido ou emitido |
| regra | obrigação, proibição ou relação aplicável no domínio |
| condição | circunstância em que expectativa ou regra vale |
| critério de sucesso | condição observável para avaliar resultado |
| métrica | modo de medir um atributo |
| meta | valor ou faixa pretendida para uma métrica |
| linha de base | valor de referência para comparação |
| questão em aberto | lacuna explícita capaz de alterar análise ou decisão |
| formulação | representação inicial, justificada e revisável do problema |
| solução | alternativa de intervenção a ser avaliada |

## Domínio, continuidade, fontes e carga

### Critérios de domínio da aula

No Nível 1, o aluno reconhece termos e exemplos. No Nível 2, explica as diferenças entre situação, necessidade, problema e solução; sintoma, hipótese e evidência; interessado e pessoa afetada; restrição, recurso e preferência; objetivo, métrica e meta. No Nível 3, declara estados, escopo e exclusões, explicita pressupostos e questões abertas, propõe critério verificável e avalia uma formulação com orientação. Inicia o Nível 4 somente quando reformula um caso simples, preserva lacunas, rejeita solução prematura e explica limites. Casos complexos e domínio final de C01/C02 ficam para a progressão da fase.

### Conexão com a Aula 03

Esta aula formulou o problema como um todo. A Aula 03 ensinará a decompô-lo preservando relações e possibilidade de recomposição. Não construímos árvore de problemas, diagrama causal, fluxo, modelo detalhado ou algoritmo; por isso, a decomposição continua necessária e não foi antecipada.

### Referências e leituras para aprofundamento

#### Referências centrais

- PÓLYA, George. *How to Solve It: A New Aspect of Mathematical Method*. 2. ed. Princeton: Princeton University Press, 1957.
- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. DOI: [10.1145/3664191](https://doi.org/10.1145/3664191).

#### Aprofundamento

- SIMON, Herbert A. The Structure of Ill Structured Problems. *Artificial Intelligence*, v. 4, p. 181–201, 1973. DOI: [10.1016/0004-3702(73)90011-8](https://doi.org/10.1016/0004-3702(73)90011-8).
- ROSEN, Kenneth H. *Discrete Mathematics and Its Applications*. 8. ed. New York: McGraw-Hill, 2019.

#### Terminologia e engenharia

- ISO; IEC; IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*. Geneva: ISO, 2017.
- ISO; IEC; IEEE. *ISO/IEC/IEEE 29148:2018 — Systems and software engineering — Life cycle processes — Requirements engineering*. Geneva: ISO, 2018.
- IEEE COMPUTER SOCIETY. *Guide to the Software Engineering Body of Knowledge (SWEBOK Guide)*. Version 4.0a, 2025, cap. 1.

### Métricas e carga sugerida

- **Extensão editorial:** aproximadamente 6.638 palavras, 371 linhas, 25 seções H2 e 11 subseções (8 H3 e 3 H4).
- **Atividades:** 15 exercícios — 3 objetivos, 5 discursivos, 4 análises de caso, 1 exercício matemático, 1 contraexemplo e 1 reescrita —, além da prática guiada e da recuperação ativa.
- **Casos e contrastes substantivos:** estoque, benefício, atendimento, reembolso, cobrança e cadastro, com variações internas.
- **Fontes utilizadas:** 7; a bibliografia distingue resolução de problemas, problemas pouco estruturados, currículo, vocabulário, requisitos e matemática elementar.
- **Matemática introduzida:** igualdade, desigualdades, intervalos inclusivos e exclusivos, conjuntos e pertencimento, taxa, linha de base e meta.
- **Leitura:** 1h35 a 1h55.
- **Exercícios da aula:** 1h40 a 2h10.
- **Prática associada:** 3h a 4h.
- **Revisão e recuperação ativa:** 25 a 35 minutos.
- **Carga total sugerida:** 6h40 a 8h40, ajustável conforme experiência e profundidade das respostas.
