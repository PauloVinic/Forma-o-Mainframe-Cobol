# Aula 01 — O que é pensamento computacional

## Metadados

- **Fase:** Fase 1 — Pensamento Computacional
- **Subtítulo da fase:** De problemas informais a soluções estruturadas
- **Posição:** primeira de 14 aulas
- **Pré-requisitos conceituais:** sistema, dado, processamento, programa, comportamento esperado, erro, falha e evidência, estudados na Fase 0
- **Prática associada:** `../praticas/pratica-01-reconhecendo-pensamento-computacional.md`

## Objetivo da aula

Ao final desta aula introdutória, o aluno deverá conseguir apresentar uma definição operacional de pensamento computacional, explicar por que ela não é a única definição possível e reconhecer dimensões dessa forma de raciocínio em situações simples. Também deverá diferenciar pensamento computacional de programação, uso de ferramentas digitais e qualquer raciocínio meramente organizado; analisar uma situação corporativa sem escrever código; e apontar limites que uma abordagem computacional não resolve sozinha.

A aula oferece um mapa inicial, não uma taxonomia definitiva. Decomposição, abstração, padrões, representação, procedimentos, automação, verificação e revisão serão reconhecidos aqui como dimensões relacionadas. As aulas seguintes desenvolverão cada uma com mais precisão.

## O problema que esta aula resolve

“Pensamento computacional” parece uma expressão autoexplicativa: seria pensar como um computador, aprender programação ou organizar uma sequência de passos. Nenhuma dessas respostas é suficiente. Computadores não atribuem propósito social a uma situação; programar é uma atividade relacionada, mas não esgota o trabalho anterior de entender o que deve ser resolvido; e muitas sequências organizadas dependem de julgamento tácito demais para constituir um procedimento computacionalmente analisável.

Outra dificuldade nasce da divulgação dos chamados “quatro pilares”: decomposição, reconhecimento de padrões, abstração e algoritmos. Esse modelo é útil para uma primeira aproximação, mas vira fonte de erro quando apresentado como definição científica única. Diferentes autores e currículos enfatizam também formulação de problemas, dados, representações, automação, simulação, avaliação, depuração, generalização, limites e consequências sociais. Além disso, os elementos não aparecem necessariamente em quatro etapas sucessivas.

Essas confusões prejudicam a progressão. Confundir pensamento computacional com digitar código leva à sintaxe antes do objetivo; chamar qualquer lista de algoritmo faz instruções ambíguas parecerem precisas; tomar o uso de aplicativo como prova de raciocínio oculta decisões incorporadas; equiparar automação a solução adequada permite reproduzir regras inadequadas ou produzir resultados incorretos em maior escala.

Esta aula estabelece distinções iniciais para que os termos posteriores não sejam usados como rótulos vazios. Ela não formaliza completamente problemas nem ensina a construir algoritmos. Seu papel é ensinar o que observar e que perguntas começar a fazer.

## Ponte com a Fase 0

A Fase 0 forneceu o vocabulário para descrever sistemas: componentes relacionados trabalham com algum propósito; dados dependem de contexto; processamento transforma dados segundo regras; programas participam de comportamentos; e uma execução pode terminar sem que o resultado esteja correto. Ela também mostrou que falha observada, defeito e causa não são sinônimos e que evidências importam para investigar diferenças entre o esperado e o ocorrido.

A Fase 1 muda a pergunta. Em vez de perguntar principalmente “que elementos existem em um sistema?”, começaremos a perguntar “como uma situação pode ser compreendida e representada para que uma solução seja construída e examinada?”. Os conceitos anteriores continuam válidos, mas passam a apoiar uma disciplina de formulação, comparação e revisão. Essa retomada é a ponte necessária; não é uma repetição das 12 aulas anteriores.

## Uma primeira situação: evitar falta de produtos

Uma rede de distribuição opera vários centros e recebe a seguinte solicitação:

> Precisamos evitar que os centros de distribuição fiquem sem produtos.

A frase expressa uma necessidade legítima, mas não esclarece produtos, centros, período nem o significado de “ficar sem”. Também não informa que dados ou estados estão disponíveis, quais regras limitam uma ação ou que evidência indicaria melhora. Saldo físico, saldo registrado e quantidade já comprometida, por exemplo, podem sustentar interpretações diferentes.

Também não há solução inevitável. Aumentar estoque, redistribuir itens, corrigir registros ou rever entregas responderia a diagnósticos distintos. Escolher imediatamente uma ferramenta de previsão transformaria uma alternativa em parte presumida do problema.

Por enquanto, basta distinguir necessidade expressa, informação conhecida e perguntas ainda abertas. A formulação completa pertence à Aula 02; aqui, o caso apenas mostra por que uma intenção compreensível ainda pode ser insuficiente para análise ou automatização.

## Uma definição operacional para a formação

Nesta formação, adotaremos a seguinte definição operacional:

> **Pensamento computacional é uma família de práticas e perspectivas orientadas pela computação para formular problemas e representar soluções de modo compatível com o processamento de informação. Nessas representações, elementos relevantes — como dados, estados, decomposições, relações, regras, procedimentos e limites — podem tornar-se explícitos para análise; estratégias podem ser executadas ou simuladas, resultados verificados e soluções revistas por pessoas, máquinas ou sistemas sociotécnicos. Isso não exige programação nem torna a automação obrigatória.**

“Definição operacional” significa uma convenção explícita para orientar estudo e avaliação. Ela indica o que o aluno deverá reconhecer e fazer, mas não encerra o debate acadêmico. Problema, estado, decomposição, modelo, padrão, representação e algoritmo ganharão tratamento próprio nas próximas aulas.

O trecho **orientadas pela computação** estabelece uma fronteira: não basta que uma atividade humana seja organizada; ela precisa mobilizar práticas ou formas de representação relacionadas ao processamento de informação. Chamar o conceito de **família** evita uma sequência obrigatória. Admitir execução ou simulação por diferentes agentes preserva atividades manuais e sistemas híbridos sem tratar toda solução como programa nem toda automação como desejável.

Essa formulação dialoga, entre outras fontes, com a definição que Wing apresentou em 2010 como usada por ela, Jan Cuny e Larry Snyder, inspirada por uma troca de mensagens com Al Aho. Nela, problemas e soluções são formulados para que um agente de processamento de informação possa realizar a solução; esse agente pode ser humano, máquina ou combinação. A definição do curso acrescenta, para fins pedagógicos, verificação, revisão e limites declarados.

## Por que o conceito permanece debatido

Não existe uma única definição universalmente aceita de pensamento computacional. Autores investigam perguntas diferentes: fundamentos da computação, capacidades ensináveis e observáveis, currículos acessíveis ou aplicações com modelos, dados e simulação. Essas perspectivas se cruzam, mas não são idênticas.

Wing apresentou em 2006 uma visão ampla e, em 2010, colocou formulação e representação para um agente de processamento de informação no centro. O National Research Council registrou em 2010 múltiplas perspectivas, sem buscar uma definição final. Shute, Sun e Asbell-Clarke constataram em 2017 diversidade de definições e modelos. Denning, no mesmo ano, criticou formulações vagas e promessas universais sem evidência suficiente.

A diversidade não torna o conceito inútil. Termos importantes frequentemente possuem mais de uma formulação, desde que cada uso declare seus critérios. O problema surge quando uma definição local é apresentada como consenso, quando qualquer atividade é incluída para tornar o conceito atraente ou quando não há evidência observável para distinguir domínio de simples familiaridade com palavras.

Por isso, esta formação assume três responsabilidades. Primeiro, declara a definição que usará. Segundo, reconhece alternativas e controvérsias relevantes. Terceiro, avalia ações observáveis: explicar distinções, identificar informações ausentes, produzir representações, acompanhar estados, construir procedimentos, testar e justificar escolhas. A falta de unanimidade exige precisão, não abandono do assunto.

## Breve contexto histórico

Práticas hoje associadas ao pensamento computacional são anteriores ao rótulo. Algoritmos, representações, abstrações e procedimentos possuem histórias longas; discussões do século XX sobre programação, modelos computacionais e educação construíram parte desse terreno.

Há registro do uso da expressão por Seymour Papert em *Mindstorms*, publicado em 1980, em contexto ligado a crianças, programação e aprendizagem. Isso impede atribuir com segurança a criação incontestável do termo a Wing. Também seria impreciso concluir que a ocorrência de 1980 já continha toda a formulação desenvolvida décadas depois. Ideias, termo e movimento educacional não nasceram necessariamente no mesmo momento.

O artigo de Wing na *Communications of the ACM*, em 2006, teve papel central na difusão contemporânea do conceito. Sua proposta ampliou a discussão dentro e fora da comunidade de computação e apresentou uma visão de habilidade fundamental, conceitual e não limitada a programar. Nos anos seguintes, oficinas, currículos e pesquisas educacionais tentaram delimitar componentes, métodos de ensino e formas de avaliação.

Essa expansão trouxe refinamentos e críticas. Revisões organizaram componentes recorrentes sem estabelecer modelo único, e Denning alertou contra incluir operação de ferramentas ou qualquer rotina como evidência. A história não vai de um inventor a uma definição final: registra usos, difusão, apropriações e críticas.

## Fronteiras do conceito

Uma definição útil precisa mostrar a relação com a computação e também o que não basta para caracterizar pensamento computacional.

### Relação com a Ciência da Computação

Pensamento computacional se relaciona diretamente com a Ciência da Computação porque mobiliza ideias centrais ao estudo da computação: representar informação, trabalhar em diferentes níveis de abstração, decompor sistemas, construir procedimentos, acompanhar estados, avaliar custos e examinar o que pode ou não ser realizado por determinados meios. O relatório curricular CS2023 inclui, entre características esperadas de egressos, resolução de problemas, decomposição, reconhecimento de padrões de solução, pensamento algorítmico e trabalho em múltiplos níveis de abstração.

Essa relação não transforma pensamento computacional na disciplina completa. Ciência da Computação abrange fundamentos algorítmicos, linguagens, arquitetura, sistemas operacionais, redes, segurança, inteligência artificial, interação humano-computador, dados, engenharia de software e outras áreas. Dominar uma introdução ao pensamento computacional não equivale a dominar essas áreas nem a possuir competência profissional.

Também não é necessário conhecer previamente uma linguagem para começar. A capacidade de tornar uma regra explícita, escolher dados relevantes ou questionar como um resultado será verificado pode anteceder a implementação. Mais tarde, programação permitirá materializar parte dessas decisões e produzir comportamento executável. Neste momento, separar as camadas é pedagogicamente necessário.

### Pensamento computacional não é programação

Programar envolve construir uma implementação em uma linguagem e em um ambiente técnico. Pensamento computacional atua também antes, durante e depois dessa atividade: ajuda a formular o que está em questão, selecionar representações, estruturar uma solução, prever comportamento, verificar resultados e revisar escolhas. Uma pessoa pode escrever código sintaticamente válido para um problema mal entendido; nesse caso, houve programação, mas a formulação continua frágil.

Para preservar o vocabulário da Fase 0, compare os termos sem tentar esgotá-los:

| Conceito | Função inicial nesta progressão | Não deve ser confundido com |
|---|---|---|
| Pensamento computacional | formular e tornar analisáveis problemas e soluções relacionados à computação | uma linguagem ou ferramenta |
| Solução | proposta para levar uma situação em direção a um objetivo | garantia de correção |
| Algoritmo | procedimento suficientemente definido para uma classe de situações; será estudado na Aula 07 | qualquer lista informal |
| Programa | implementação concreta de comportamentos em forma tratável por ambiente computacional | problema ou sistema completo |
| Código-fonte | representação textual formal usada para construir programas | execução ativa |
| Execução | ocorrência efetiva de operações em um ambiente | prova de que o objetivo foi atendido |

Uma progressão didática possível é: situação → problema formulado → modelo → solução → algoritmo → implementação → programa → execução → resultado observado. Ela não é uma linha rígida. Um teste pode levar à revisão do algoritmo; uma limitação técnica pode exigir novo modelo; uma conversa com interessados pode reformular o problema. O valor da progressão está em impedir que código e resultado sejam tratados como se contivessem, sozinhos, todas as decisões anteriores.

### Pensamento computacional não é uso de computador

Uma pessoa pode preencher uma planilha, clicar em um relatório ou aceitar a sugestão de um aplicativo sem compreender quais dados foram usados, quais regras produziram o resultado ou em que condições ele deixa de ser confiável. Há uso de computador, mas não há evidência suficiente de formulação ou projeto computacional por parte do usuário.

Imagine duas atividades. Na primeira, um analista copia números para uma planilha pronta e encaminha o total mostrado. Na segunda, outro analista investiga que registros devem participar do total, explicita tratamento de duplicidades, representa exceções, compara o resultado com uma fonte independente e registra limites. Ambos usam planilha; somente a segunda descrição oferece sinais claros das práticas estudadas aqui. A diferença não está no produto comercial utilizado, mas no trabalho intelectual observável.

O inverso também ocorre. Uma equipe pode representar manualmente estados de pedidos em cartões, examinar transições permitidas e simular casos antes de escolher tecnologia. Não há computador em uso, mas existe preparação genuinamente relacionada à futura computação. O artefato físico funciona como representação examinável.

Operar ferramentas é uma competência real e pode ser necessária. O ponto é não usá-la como substituto para compreender ou projetar o processamento. Ferramentas incorporam decisões tomadas por outras pessoas; saber utilizá-las não demonstra automaticamente saber formular as decisões que elas executam.

### Pensamento computacional não é qualquer pensamento organizado

Se toda atividade organizada fosse pensamento computacional, o termo deixaria de distinguir algo. Planejar uma conversa delicada, interpretar uma obra de arte ou deliberar sobre um valor moral pode envolver disciplina, sequência e revisão sem que seja útil classificar a atividade inteira como computacional. A presença de ordem é insuficiente.

Nesta formação, procuraremos uma combinação de sinais: representação explícita; decomposição controlada; dados ou estados que podem ser acompanhados; regras e procedimentos examináveis; possibilidade de execução ou simulação; repetibilidade nas condições declaradas; verificação entre esperado e observado; consideração de escala, recursos e automação potencial. Nenhum sinal isolado funciona como teste definitivo, e nem todos precisam ter a mesma importância em todo caso.

Essa fronteira é deliberadamente cuidadosa, não rígida. Pensamento computacional se sobrepõe ao pensamento matemático quando usa abstração e precisão; ao científico quando formula hipóteses, trabalha com dados e busca evidências; ao sistêmico quando observa componentes, relações e feedback; ao de engenharia quando projeta sob restrições; e ao design quando investiga necessidades e cria alternativas. As sobreposições não apagam as tradições nem autorizam chamar todo bom raciocínio de computacional.

## Os chamados quatro pilares

Muitos materiais introdutórios organizam pensamento computacional em quatro ideias: decomposição, reconhecimento de padrões, abstração e algoritmos. O modelo é popular porque oferece vocabulário curto e uma rota didática compreensível. Ele ajuda o iniciante a perguntar se um problema pode ser dividido, se casos compartilham regularidades, quais detalhes importam e como uma solução pode ganhar passos explícitos.

Seu valor didático não o transforma em taxonomia universal. A literatura apresenta listas e estruturas diferentes. Shute, Sun e Asbell-Clarke, por exemplo, encontraram com frequência abstração, decomposição, algoritmos e depuração em seu recorte, não exatamente o mesmo conjunto popular. Outras abordagens destacam representação de dados, simulação, automação, avaliação, generalização, colaboração ou impactos sociais. Até o significado de cada componente varia conforme o contexto educacional e disciplinar.

Além disso, os quatro elementos se sobrepõem. Reconhecer regularidades depende dos aspectos que a abstração tornou comparáveis. Decompor exige decidir fronteiras e níveis de detalhe. Construir um procedimento pode revelar que a decomposição perdeu uma dependência. Um resultado inesperado pode levar à revisão da abstração inicial. Não há obrigação de passar por quatro caixas em ordem fixa nem garantia de que percorrê-las produza solução adequada.

Nesta fase, o modelo será usado como porta de entrada. Decomposição, abstração e padrões receberão aulas próprias; algoritmos serão definidos posteriormente; representação, estado, decisões, repetições, modularização, testes, depuração, eficiência e limites completarão a progressão. Em vez de decorar quatro palavras, o aluno aprenderá a produzir evidências do raciocínio que elas nomeiam.

## Dimensões relacionadas, não etapas isoladas

### Decomposição

Decompor é dividir para tornar partes analisáveis, preservando relações necessárias à recomposição. Separar compras, armazenagem e vendas pode ajudar somente se suas dependências continuarem visíveis. A Aula 03 ensinará critérios e riscos; aqui basta reconhecer que dividir exige propósito.

### Abstração e modelos

Abstrair é selecionar aspectos relevantes e omitir outros de forma controlada. Um mapa pode omitir a cor da embalagem, mas não a validade se produtos vencidos estiverem indisponíveis. Modelo é representação deliberada, não cópia completa da realidade. Fronteiras e níveis de detalhe ficam para a Aula 04.

### Padrões e generalização

Reconhecer padrões envolve semelhanças, diferenças e regularidades. Faltas após campanhas sugerem investigação, não causa provada. Generalizar exige procurar exceções e declarar onde a regra parece válida. A Aula 05 desenvolverá essa passagem.

### Procedimentos e algoritmos

Uma intenção como “reponha quando estiver baixo” precisa ganhar precisão antes de orientar execução consistente. Um procedimento informal ainda pode depender de experiência e contexto tácito. A Aula 07 estabelecerá os critérios de um algoritmo; aqui, basta distinguir intenção, orientação informal e procedimento que começa a se tornar examinável.

### Representação

Raciocínio mantido apenas na cabeça é difícil de comparar, comunicar e verificar. Texto estruturado, tabelas, diagramas e modelos tornam aspectos diferentes examináveis; futuramente, pseudocódigo poderá expressar procedimentos. Ele é apenas mencionado aqui, sem notação ou exemplo. Representar não garante qualidade, mas cria uma superfície para localizar lacunas e divergências. A escolha, a combinação e as perdas de cada forma pertencem à Aula 06.

### Verificação, avaliação e revisão

Pensamento computacional não termina quando alguém propõe passos. É preciso perguntar se a proposta atende ao objetivo, em quais condições funciona, que entradas admite, que casos foram esquecidos, qual evidência sustenta o resultado e que limitações permanecem. Também interessa saber se o processo pode ser repetido, se os resultados podem ser explicados e se outra estratégia seria mais adequada.

Testar, depurar e discutir correção ganharão tratamento próprio na Aula 12; custos e eficiência, na Aula 13. Por ora, retenha uma distinção: **executar sem interrupção não demonstra que uma solução está correta, e estar correta em um caso não demonstra que seja adequada a todos os casos**. Revisão é parte do trabalho, não um remendo posterior.

Essas dimensões formam ciclos. Uma tentativa de verificação pode revelar dado ausente e levar à reformulação; uma representação pode mostrar que a decomposição perdeu uma relação; uma exceção pode restringir uma generalização; um limite de automação pode devolver uma decisão ao julgamento humano.

## Pessoas, máquinas, escala e automação

### Distribuição da execução e da responsabilidade

Uma solução estruturada pode ser executada manualmente, automatizada ou dividida entre pessoas e tecnologias. Aqui, **execução** tem sentido amplo: uma pessoa realiza um procedimento; um computador executa instruções de um programa. Reconhecer ambos os agentes não torna as formas idênticas. Uma equipe pode conferir solicitações, sistemas podem calcular indicadores e encaminhar exceções, e pessoas autorizadas podem decidir casos dependentes de contexto. A análise computacional não obriga implementação integral em software.

Chamamos de **sistema sociotécnico** um arranjo no qual pessoas, processos, regras, dados e tecnologias se relacionam para algum propósito. Essa perspectiva mantém a noção de sistema da Fase 0. No controle de estoque, operadores registram movimentos, sensores podem medir quantidades, sistemas consolidam dados, compradores negociam e gestores definem níveis de risco. O resultado não vem de uma máquina isolada.

Automatizar muda a distribuição do trabalho e da responsabilidade; não elimina nenhum dos dois. Pessoas escolhem objetivos, dados e regras, aprovam exceções, operam infraestrutura, interpretam resultados e respondem por consequências. Um sistema também pode ampliar um erro: uma regra equivocada aplicada manualmente a dez itens causa um tipo de impacto; a mesma regra automatizada para milhões de movimentos pode produzir impacto muito maior antes de ser percebida.

Alguns aspectos resistem à automatização porque dependem de informação não registrada, negociação, valores ou julgamento contextual. Outros poderiam ser automatizados, mas não deveriam sê-lo sem controles, explicabilidade ou supervisão. Pensamento computacional ajuda a tornar essas fronteiras discutíveis; não decide sozinho onde colocá-las.

### Quando escala e repetição importam

A abordagem computacional ganha importância quando uma organização lida com grande volume, tarefas recorrentes, múltiplos estados, muitas regras, integrações e necessidade de rastreabilidade. Conferir manualmente cinco movimentos pode ser viável; conferir milhões exige representações e procedimentos que preservem consistência, permitam dividir trabalho e registrem o que ocorreu. Escala torna ambiguidades caras.

Repetição também evidencia diferenças. Se duas pessoas seguem a mesma orientação e produzem resultados incompatíveis, talvez a orientação dependa de conhecimento implícito. Se uma mudança de regra precisa ser aplicada em muitos pontos, uma decomposição inadequada pode espalhar inconsistências. Se dados atravessam vários sistemas, cada transformação precisa preservar significado.

Ainda assim, pensamento computacional não pertence apenas a problemas grandes. Um caso pequeno pode exigir precisão por envolver segurança, direitos ou dinheiro. E nem todo problema de grande volume deve ser automatizado da mesma maneira. Volume, por si só, não define objetivo, legitimidade ou qualidade.

## Alcance e limites

Pensamento computacional oferece meios para formular, representar, executar e examinar soluções, mas não substitui todas as formas de conhecimento. Ele não define sozinho qual objetivo uma organização deveria perseguir. Reduzir faltas no estoque pode competir com reduzir desperdício, custo ou impacto ambiental; selecionar a prioridade requer decisões econômicas, operacionais e éticas.

Também não garante que os dados sejam verdadeiros. Uma base pode estar completa no formato e incorreta em relação ao estoque físico. Um procedimento preciso aplicado a dados ruins pode produzir saída precisa na forma e enganosa no significado. Conhecimento do domínio continua necessário para entender validade, exceções e consequências.

Uma formulação computacional não resolve automaticamente ambiguidades sociais nem prova que uma regra seja justa. Critérios de concessão de benefício podem ser executáveis e ainda excluir grupos de modo indevido. Um modelo pode omitir uma característica importante; uma métrica pode favorecer o que é fácil medir; um resultado eficiente pode contrariar direitos ou responsabilidades. Ética não é um campo que se converte integralmente em cálculo.

Por fim, a abordagem não elimina julgamento, não torna toda decisão automatizável, não garante que uma implementação corresponda ao modelo e não assegura correção apenas porque houve teste. Ela pode tornar pressupostos e consequências mais visíveis, apoiar comparação e produzir evidências. Usá-la responsavelmente inclui saber quando seus modelos são insuficientes e quando outras perspectivas precisam conduzir a decisão.

## Caso progressivo: três versões do estoque

Retomemos a rede de distribuição sem formalizar o problema por completo.

### Versão A — Solicitação vaga

> Evite falta de produtos.

Há uma necessidade aparente, mas “falta”, universo de produtos, horizonte de tempo e critério de sucesso permanecem abertos. Não sabemos se a frase pede prevenção, detecção, resposta ou combinação. Escolher imediatamente uma ferramenta seria inventar parte do problema.

### Versão B — Procedimento informal

> Quando o estoque estiver baixo, peça mais unidades.

A descrição adiciona uma observação e uma ação, mas continua dependente de julgamento implícito. “Estoque” pode ser físico, registrado ou disponível; “baixo” não possui critério; “mais unidades” não considera lote, prazo, demanda, espaço ou autorização. Duas pessoas podem seguir a orientação de boa-fé e agir de modos diferentes.

### Versão C — Formulação inicial estruturada

Sem decidir regras, podemos separar o que já foi dito, o que apenas parece relevante e o que continua desconhecido:

| Aspecto | Conhecido na situação | Hipótese ou inferência a confirmar | Ainda desconhecido |
|---|---|---|---|
| Objetos | há produtos e centros de distribuição | movimentos e pedidos podem afetar disponibilidade | quais produtos e centros pertencem ao escopo? |
| Estados | a indisponibilidade é indesejada | saldos físico, registrado e comprometido podem diferir | que estado caracteriza “falta”? |
| Eventos e dados | nenhuma fonte foi declarada | vendas, recebimentos, transferências e datas podem importar | que dados existem e com que qualidade e atualidade? |
| Regras e ações | nenhuma regra ou ação foi definida | alerta, compra ou transferência são alternativas possíveis | que critérios valem e quem autoriza cada ação? |
| Resultado e evidência | deseja-se reduzir faltas | históricos e contagens podem apoiar verificação | qual resultado será aceito e como será examinado? |

A coluna intermediária não acrescenta fatos: ela registra inferências que precisariam ser confirmadas. A versão C ainda não é problema completamente formulado, especificação ou algoritmo. Sua contribuição é tornar a diferença entre conhecido, inferido e desconhecido comparável, preparando a delimitação que será ensinada na Aula 02.

## Exemplos, contraexemplos e erros de classificação

### Contrastes entre casos

**Exemplo positivo 1 — Conciliação de cobranças.** Uma equipe identifica fontes, representa estados, separa divergências, descreve um procedimento repetível, verifica amostras e registra casos não cobertos. Há sinais relacionados à computação antes de qualquer implementação.

**Exemplo positivo 2 — Rotas de entrega.** Analistas representam pontos, horários e capacidade, comparam estratégias e examinam custos e exceções. O modelo apoia processamento e simulação, mas não decide se rapidez deve prevalecer sobre condições de trabalho ou impacto ambiental.

**Dois contraexemplos com computador.** Uma pessoa cola dados em planilha pronta e envia o total sem conhecer origem, regra ou exclusões. Em outra organização, um gestor pede inteligência artificial contra atrasos sem distinguir tipos, causas, dados, restrições ou sucesso. No primeiro caso há operação sem evidência suficiente de formulação; no segundo, a tecnologia foi escolhida antes do problema.

**Caso limítrofe.** Uma mediadora organiza uma conversa, considera emoções e adapta perguntas a respostas singulares. Há método e revisão, mas talvez nenhuma vantagem explicativa em classificar todo o julgamento relacional como pensamento computacional. A classificação mudaria se parte do processo fosse representada por estados, regras examináveis e formas de verificação, sem reduzir a mediação a esses elementos.

**Caso híbrido.** Um sistema verifica documentos e encaminha solicitações; pessoas interpretam exceções e justificam decisões; auditoria examina registros. A solução combina processamento automatizado, julgamento contextual e responsabilidade distribuída.

### Erros recorrentes ao interpretar as dimensões

Uma lista pode omitir condições e depender de julgamento tácito; por isso, não se torna algoritmo apenas por ordenar passos. Do mesmo modo, decompor não é criar partes arbitrárias, abstrair não é ignorar qualquer detalhe e reconhecer uma regularidade não prova uma regra. Critério, relação, exceção e limite continuam necessários, mas serão desenvolvidos nas aulas próprias.

Automatizar pode reproduzir com consistência uma regra inadequada. Conhecimento do domínio continua necessário para interpretar dados e consequências, e viabilidade técnica não decide legitimidade. Pessoas de outras áreas podem participar de formulações computacionais, mas isso não transforma toda atividade humana em computação. Ferramenta é alternativa de solução, não definição antecipada do problema.

## Prática guiada dentro da aula

Compare duas descrições sobre análise de pagamentos duplicados.

**Descrição 1:** “Use a planilha para eliminar pagamentos repetidos.”

**Descrição 2:** “Antes do fechamento, a equipe precisa identificar lançamentos possivelmente duplicados. Estão disponíveis identificador do fornecedor, documento, valor, data e origem do lançamento. Ainda não se sabe quais combinações caracterizam duplicidade, como tratar correções legítimas nem que evidência autoriza bloquear um pagamento.”

Antes de ler o comentário, identifique em cada descrição: objetivo aparente, informação explícita, suposições, elementos representáveis, partes que poderiam ser examinadas separadamente, regras ausentes, critérios de verificação e possibilidade de automação.

**Análise comentada.** Na primeira descrição, “eliminar pagamentos repetidos” é o objetivo aparente e a planilha já foi escolhida. Não sabemos se “eliminar” significa bloquear, excluir registro ou investigar; também não sabemos como duplicidade será reconhecida. Presumir que valores iguais bastam poderia bloquear pagamentos legítimos. Não há critério para verificar se duplicidades reais foram encontradas sem falsos bloqueios. Automatizar agora seria prematuro.

Na segunda, objetivo e momento estão mais visíveis, e há dados potencialmente representáveis. A descrição separa identificação de suspeitas, tratamento de correções e autorização de bloqueio, embora ainda não ensine uma decomposição formal. Ela distingue informação disponível de regra ausente. É possível imaginar apoio automatizado para selecionar candidatos, mas a adequação depende de critérios, qualidade dos dados e tratamento de exceções. A análise correta não completa silenciosamente essas lacunas; registra perguntas para a próxima etapa.

## Exercícios de recuperação

### Reconhecimento

1. Em qual relato há evidência mais forte de pensamento computacional?

   a. O analista adapta o fluxo recomendado pelo aplicativo depois de dois erros e repete a nova sequência com sucesso.

   b. A equipe identifica a origem dos valores, representa exceções, declara condições e compara o resultado com um registro independente.

   c. O gestor divide o trabalho entre setores, padroniza uma planilha e acompanha o tempo total de atendimento.

   d. A pessoa registra estados e confere o total esperado, mas não sabe que registros devem participar nem por quê.

2. Uma equipe executou uma sequência uma vez e obteve o resultado desejado. Qual conclusão é sustentada sem extrapolação?

   a. Entradas de formato semelhante provavelmente produzirão o mesmo resultado.

   b. Aquele caso produziu o resultado esperado nas condições observadas.

   c. A regra representa corretamente o objetivo organizacional pretendido.

   d. Exceções que não apareceram podem ser desconsideradas nesta classe de casos.

3. Um curso usa decomposição, padrões, abstração e algoritmos, mas também trabalha representação, dados e verificação. Qual interpretação é mais precisa?

   a. Os quatro elementos formam um núcleo necessário; representação, dados e verificação apenas avaliam sua aplicação.

   b. O curso adotou um mapa pedagógico recorrente e reconheceu que outras organizações também são possíveis.

   c. O curso escolheu uma taxonomia operacional local que se torna completa quando recebe os três tópicos adicionais.

   d. O curso usa os quatro elementos como sequência heurística e distribui representação, dados e verificação entre as etapas.

4. Distribua as descrições entre “evidência fraca” e “evidência relevante, ainda inconclusiva”; empates são permitidos. Justifique e indique uma informação adicional que poderia alterar cada grupo: “usa um computador”; “segue uma rotina conhecida”; “registra estados e compara resultado esperado”; “explicita regras e casos não cobertos”.

### Explicação

5. Explique, com palavras próprias, por que pensamento computacional não é sinônimo de programação. Use programa e execução na resposta.

6. Explique por que o uso da expressão por Papert e a difusão promovida por Wing não sustentam uma narrativa simples de “inventor e definição final”.

7. Escolha um elemento da definição operacional e explique que inclusão indevida poderia ocorrer se ele fosse removido. Não basta repetir a definição.

8. No caso de estoque, indique um aspecto que uma decomposição futura precisaria preservar e uma seleção de detalhes que já funcione como abstração inicial. Explique a diferença sem decompor o problema nem criar um modelo.

9. Explique por que admitir execução por pessoas e máquinas não distribui automaticamente responsabilidade nem torna as duas formas de execução idênticas.

### Análise introdutória de casos

10. Uma empresa diz: “Automatize a aprovação de reembolsos para acabar com erros”. Identifique duas reduções conceituais presentes na frase e explique seus riscos, sem formular o problema nem propor solução.

11. Um hospital usa um sistema que ordena atendimentos, mas profissionais podem alterar a prioridade mediante justificativa registrada. Identifique elementos humanos, tecnológicos e de verificação. Explique por que o caso é sociotécnico.

12. Duas equipes aplicam a mesma regra de reposição. Uma recebe saldos atualizados a cada hora; a outra, somente no fim do dia. Explique por que procedimento igual não garante significado ou resultado comparável.

### Reflexão e transferência

13. Escolha uma atividade do seu contexto que use computador. Que evidência permitiria distinguir operação da ferramenta de participação na formulação computacional?

14. Crie um caso limítrofe que apresente alguns sinais de pensamento computacional, mas cuja classificação permaneça discutível. Indique a evidência que sustenta cada lado.

### Contraexemplo

15. Crie uma situação em que os quatro pilares estejam presentes e, ainda assim, a solução seja inadequada por causa do objetivo, dos dados ou de um limite ignorado.

### Orientações de autocorreção

Nas questões objetivas, verifique se sua escolha respeita as qualificações da aula, em vez de procurar apenas uma palavra familiar. Nas respostas abertas, procure distinção explícita, exemplo coerente, limite e justificativa. Em casos ambíguos, separar informação fornecida, inferência e pergunta vale mais que inventar uma solução. Uma resposta pode divergir dos exemplos da aula e ainda ser adequada se declarar critérios e não antecipar fatos.

Se você chama qualquer rotina de algoritmo, qualquer uso de aplicativo de pensamento computacional ou qualquer automatização de solução correta, retome as seções de distinção. Se consegue reconhecer os termos, mas não explicar por que uma descrição é insuficiente, faça a prática associada antes de avançar.

## Recuperação ativa e reflexão

### Perguntas de recuperação ativa

Responda sem consultar o texto e confira depois:

1. Que relação com a computação delimita a definição operacional adotada?
2. Por que pensamento computacional não é sinônimo de programação nem de uso de computador?
3. Por que os quatro pilares não devem ser tratados como taxonomia universal?
4. Como representação e verificação tornam uma solução examinável?
5. O que caracteriza um sistema sociotécnico e onde permanece a responsabilidade?
6. Que limite ético, organizacional ou epistêmico um procedimento não resolve sozinho?

### Perguntas para reflexão

- Quando automatizar uma decisão redistribui responsabilidade em vez de eliminá-la?
- Como uma representação pode tornar um problema tratável e, ao mesmo tempo, ocultar pessoas ou condições relevantes?
- Em que situação recusar automação seria uma decisão tecnicamente responsável, e que evidência apoiaria essa escolha?

## Síntese da aula

Pensamento computacional foi definido, para esta formação, como uma família de práticas e perspectivas orientadas pela computação. Ela ajuda a formular problemas e a representar soluções de modo compatível com o processamento de informação, de forma que elementos relevantes, como dados, estados, relações, regras, procedimentos e limites, possam tornar-se examináveis. Pessoas, máquinas ou sistemas sociotécnicos podem executar ou simular estratégias, verificar resultados e revisar soluções, sem que programação ou automação sejam obrigatórias. A definição é operacional e não encerra o debate acadêmico.

O conceito se relaciona à Ciência da Computação, mas não equivale à disciplina, à programação ou ao uso de computadores. Decomposição, padrões, abstração e algoritmos formam um modelo introdutório útil, não uma taxonomia definitiva. Representação, dados, estados, automação, avaliação, revisão, custos e limites também importam.

Uma abordagem computacional pode aumentar precisão e escala, mas não escolhe objetivos, garante dados verdadeiros, resolve justiça ou substitui conhecimento do domínio. O caso de estoque mostrou a diferença entre necessidade vaga, procedimento informal e organização inicial de elementos e perguntas. A próxima aula transformará essa percepção em trabalho mais disciplinado sobre o que é um problema.

## Mini glossário

**Pensamento computacional:** família de práticas e perspectivas orientadas pela computação para formular problemas e tornar soluções representáveis, analisáveis e verificáveis, sem exigir programação ou automação.

**Problema:** obstáculo relevante entre situação inicial e desejada; será delimitado na Aula 02.

**Formulação:** explicitação de elementos, relações, condições e perguntas do que será tratado.

**Representação:** forma de expressar aspectos de algo; não é o objeto representado.

**Decomposição:** divisão orientada que preserva relações e possibilidade de recompor o todo.

**Abstração:** seleção de aspectos relevantes com omissão controlada de detalhes segundo um propósito.

**Padrão:** regularidade reconhecida por critérios entre casos, dados ou processos.

**Generalização:** extensão justificada a uma classe de casos, com condições e exceções.

**Procedimento:** orientações ou passos organizados para uma tarefa, talvez dependentes de contexto.

**Algoritmo:** procedimento preciso para uma classe delimitada; será definido na Aula 07.

**Automação:** execução de parte de uma atividade por tecnologia segundo regras e condições estabelecidas.

**Verificação:** comparação orientada por critérios entre o esperado e a evidência disponível sobre o observado.

**Modelo:** representação deliberada de aspectos selecionados para descrever, explicar, prever ou decidir.

**Estado:** conjunto de informações relevantes que descreve uma situação em determinado momento.

**Sistema sociotécnico:** arranjo relacionado de pessoas, processos, regras, dados e tecnologias.

## Critérios de domínio da aula

O domínio esperado concentra-se no **Nível 1 — Reconhecimento**, no **Nível 2 — Explicação** e no início do **Nível 3 — Aplicação guiada**. Esta aula não exige formulação autônoma de problema nem domínio das competências C01 e C02.

O aluno demonstra o nível esperado quando consegue:

- explicar pensamento computacional sem reduzi-lo a programação, computador ou lista de passos;
- relacionar pelo menos duas dimensões, explicando por que não operam como caixas isoladas;
- apresentar os quatro pilares como modelo didático útil e não universal;
- identificar sinais de representação, estados, procedimentos ou verificação em caso curto;
- apontar por que uma descrição ainda é insuficiente sem inventar silenciosamente uma regra;
- produzir exemplo e contraexemplo coerentes;
- reconhecer ao menos dois limites, como dados incertos, valor ético ou necessidade de conhecimento do domínio;
- analisar, com perguntas fornecidas, um processo corporativo sem escrever uma implementação.

Reconhecer palavras sem justificativa corresponde apenas a evidência inicial. Explicar distinções com exemplo sustenta o Nível 2. Preencher a análise guiada da prática, separando evidência, inferência e lacuna, inicia o Nível 3. Aplicação autônoma será construída nas aulas posteriores.

## Conexão com a próxima aula

A Aula 01 apresentou um modo geral de observar problemas e soluções. A **Aula 02 — O que é um problema** começará a delimitar situações vagas por objetivos, interessados, estados, restrições e critérios de sucesso. Será a passagem de uma visão panorâmica para uma formulação mais precisa, não para o código.

## Referências e leituras para aprofundamento

### Referências centrais

- PAPERT, Seymour. *Mindstorms: Children, Computers, and Powerful Ideas*. New York: Basic Books, 1980, p. 182.
- WING, Jeannette M. Computational Thinking. *Communications of the ACM*, v. 49, n. 3, p. 33–35, 2006. DOI: 10.1145/1118178.1118215. [Cópia hospedada pela Carnegie Mellon University](https://www.cs.cmu.edu/~CompThink/papers/Wing06.pdf).
- WING, Jeannette M. *Computational Thinking: What and Why?* Documento institucional, Carnegie Mellon University, 17 nov. 2010, 6 p. [Texto em página institucional](https://www.cs.cmu.edu/~CompThink/papers/TheLinkWing.pdf).
- NATIONAL RESEARCH COUNCIL. *Report of a Workshop on the Scope and Nature of Computational Thinking*. Washington, DC: The National Academies Press, 2010. DOI: [10.17226/12840](https://doi.org/10.17226/12840).
- SHUTE, Valerie J.; SUN, Chen; ASBELL-CLARKE, Jodi. Demystifying computational thinking. *Educational Research Review*, v. 22, p. 142–158, 2017. DOI: [10.1016/j.edurev.2017.09.003](https://doi.org/10.1016/j.edurev.2017.09.003).

### Leitura de aprofundamento

- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM Press, IEEE Computer Society Press e AAAI Press, 2023. DOI: 10.1145/3664191. [Relatório oficial](https://ieeecs-media.computer.org/media/education/reports/CS2023.pdf).

### Leitura crítica e contraponto

- DENNING, Peter J. Remaining Trouble Spots with Computational Thinking. *Communications of the ACM*, v. 60, n. 6, p. 33–39, 2017. DOI: 10.1145/2998438. [Texto integral no repositório da Naval Postgraduate School](https://hdl.handle.net/10945/59443).

## Métricas e carga sugerida

A contagem abaixo usa `Measure-Object -Word` do PowerShell:

- **Palavras:** 6.320;
- **Linhas:** 446;
- **Seções de segundo nível:** 24;
- **Exercícios:** 15;
- **Casos ou situações centrais:** 1 caso progressivo em 3 versões, 6 casos de contraste, 1 prática guiada em 2 descrições e 3 casos fornecidos para análise nos exercícios;
- **Fontes efetivamente utilizadas:** 7;
- **Leitura atenta:** 1 h 15 min a 1 h 40 min;
- **Pausas de elaboração e anotações:** 40 min a 55 min;
- **Exercícios da aula:** 1 h 45 min a 2 h 15 min;
- **Tentativa da prática associada antes da solução:** 1 h 45 min a 2 h 15 min;
- **Consulta da solução e revisão da prática:** 45 min a 1 h;
- **Recuperação ativa e síntese final:** 30 min a 40 min;
- **Carga total sugerida:** 6 h 40 min a 8 h 45 min.

Os intervalos tornam explícitos os blocos da estimativa. Na prática associada, tentativa, consulta e revisão somam 2 h 30 min a 3 h 15 min.
