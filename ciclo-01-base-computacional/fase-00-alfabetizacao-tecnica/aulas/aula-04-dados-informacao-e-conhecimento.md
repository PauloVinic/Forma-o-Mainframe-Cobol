# Aula 04 — Dados, informação e conhecimento

## Objetivo da aula

O objetivo desta aula é construir uma compreensão inicial, cuidadosa e útil sobre dado, informação e conhecimento. Ao final, o aluno deve conseguir usar esses termos em situações de sistemas sem tratá-los como sinônimos nem como etapas automáticas de uma escada universal. Deve reconhecer que sistemas armazenam e transformam representações; pessoas e organizações interpretam essas representações segundo contextos, propósitos, regras e evidências.

Esta aula também prepara o estudo de processamento. Para entender o que será transformado na Aula 05, é necessário perceber que um valor não chega ao sistema com significado completo e garantido. Há origem, formato, unidade, momento, regra, finalidade e possíveis problemas de qualidade. A transformação técnica de um registro é importante, mas não basta para provar que uma decisão baseada nele é correta.

## O problema que esta aula resolve

No uso cotidiano, dado, informação e conhecimento costumam ser empregados como se fossem a mesma coisa. Em um sistema, alguém diz que “tem a informação”; em outro momento, diz que “o dado está errado”; depois, afirma que “a equipe já conhece o cliente”. As três frases podem fazer sentido, mas apontam para coisas diferentes. Confundi-las dificulta identificar o que foi registrado, o que foi interpretado, o que sustenta uma conclusão e qual parte de uma decisão pode ser questionada.

Há ainda um risco comum: imaginar que o caminho dado → informação → conhecimento ocorre por si só. Um sistema pode registrar milhões de valores e ainda não produzir entendimento útil. Pode processar uma tabela corretamente e exibir uma saída sem relevância para a pergunta que alguém precisa responder. Uma pessoa pode receber um relatório bem organizado e ainda não ter conhecimento suficiente para decidir, porque faltam experiência, comparação, justificativa ou informação sobre limites.

Esta aula adota definições operacionais para apoiar o restante da formação. Elas não são as únicas definições legítimas. Computação, Ciência da Informação, estatística, filosofia, administração, engenharia e sistemas de informação usam esses termos com ênfases diferentes. Reconhecer essa variação não confunde o iniciante; ajuda a evitar a falsa segurança de uma definição curta apresentada como universal.

## Introdução: representações, pessoas e sistemas

Nas aulas anteriores, tecnologia da informação foi apresentada como relação entre pessoas, processos, dados e tecnologia. Sistema foi apresentado como conjunto de componentes relacionados. Hardware, software e pessoas mostraram que o processamento depende tanto de recursos técnicos quanto de decisões humanas. Agora o foco recai sobre aquilo que circula, é registrado, transformado, consultado e usado nesses sistemas.

Quando um cliente solicita crédito, quando uma empresa calcula uma cobrança ou quando uma instituição analisa um benefício, não lida diretamente com toda a realidade. Lida com representações: números, textos, documentos, datas, códigos, medições, classificações e registros de eventos. Essas representações podem ser úteis, incompletas, antigas, estimadas ou incorretas. O sistema não vê a pessoa, o pagamento ou o fato em si; ele opera sobre formas registradas que foram definidas, coletadas e interpretadas por pessoas e processos.

Essa observação não reduz a importância dos dados. Ao contrário: mostra por que precisam ser tratados com cuidado. Uma boa decisão depende de saber o que uma representação pretende indicar, de onde veio, quando foi produzida, qual regra a transformou e até que ponto merece confiança. Dados são parte importante da evidência, mas não são automaticamente a realidade nem uma conclusão pronta.

## Por que não existe uma única definição simples

Em computação, é comum chamar de dado aquilo que um programa recebe, armazena ou manipula. Em estatística, dado pode ser observação, medida ou resultado de levantamento. Em administração e sistemas de informação, a preocupação muitas vezes está na utilidade para processos e decisões. Na Ciência da Informação, autores discutem em profundidade a relação entre dados, informação, conhecimento, documentos, significado e pessoas. Na filosofia, perguntas sobre verdade, justificação e conhecimento têm alcance ainda maior.

Portanto, o curso não tentará decretar uma definição definitiva para todas as áreas. A definição operacional adotada aqui é a seguinte: **dado é uma representação registrada, recebida, produzida ou usada por um processo, que pode ser interpretada em determinado contexto**. Essa formulação inclui valores observados no mundo, mas não exige que sejam verdadeiros. Também inclui resultados calculados, estimativas, classificações, registros simulados e hipóteses usados para analisar ou executar uma atividade.

Para esta fase, **informação** será entendida como dados organizados, comunicados ou interpretados de modo significativo para uma pergunta, atividade ou decisão. E **conhecimento** será entendido como capacidade de compreender relações, explicar, prever, avaliar limites e agir ou investigar com base em informações, experiência, modelos e justificativas disponíveis. Essas definições são úteis para aprender sistemas; serão refinadas quando a formação tratar dados, algoritmos, bancos de dados, lógica e tomada de decisão com mais profundidade.

## O que pode ser considerado dado

Um dado pode ser um valor, mas não se limita a um número em uma célula. Pode ser um símbolo, um texto, uma imagem, uma medição de sensor, uma observação feita por pessoa, uma data, uma classificação, um identificador, um registro de evento ou o resultado de um cálculo. A palavra “representação” é importante: o dado representa algo, uma condição, uma medida, uma afirmação ou uma hipótese segundo regras de registro e interpretação.

Considere uma análise de crédito. O valor de renda informado por uma pessoa é um dado declarado. A renda calculada a partir de registros de pagamento é um dado derivado. Uma faixa de risco atribuída por um modelo é uma classificação. Uma renda projetada para o próximo período é uma estimativa. Um conjunto de perfis criado para testar um sistema antes de usar dados reais é dado sintético. Um cenário que pergunta “e se a renda cair 20%?” usa dado hipotético. Todos podem ser úteis, mas não têm a mesma origem, finalidade ou grau de confiança.

Um **dado observado** resulta de observar ou medir alguma condição: temperatura registrada por sensor, horário de acesso, quantidade entregue. Um **dado informado** é declarado por alguém ou recebido de outra fonte: endereço preenchido em formulário, código enviado por parceiro. Um **dado derivado** é obtido a partir de outros dados por cálculo, combinação ou regra: total de compras do mês, média de atraso, saldo calculado. Um **dado sintético** é produzido artificialmente para teste, treinamento, simulação ou pesquisa. Um **dado hipotético** representa condição suposta para explorar consequências, como projeção de demanda ou cenário de risco.

Essas categorias podem se sobrepor. Uma estimativa pode ser derivada de dados observados; uma classificação pode ser calculada por um modelo e depois registrada como dado para outro processo. A finalidade aqui não é decorar uma taxonomia fechada, mas fazer perguntas melhores: esse valor foi observado, informado, calculado, estimado ou simulado? Qual regra o produziu? Ele representa o presente, o passado, uma previsão ou uma hipótese?

## Dado não é sinônimo de fato verdadeiro

Definir dado apenas como “fato registrado” seria impreciso. Um sistema pode registrar algo que corresponde à realidade, mas também pode guardar erro de digitação, valor desatualizado, informação incompleta, declaração fraudulenta, estimativa ou simulação. O registro existe; sua exatidão e sua utilidade ainda precisam ser avaliadas.

Um **fato** é algo que efetivamente ocorreu ou é o caso, independentemente de ter sido registrado. Uma **observação** é o resultado de alguém ou algum instrumento observar uma condição. Uma **representação** é a forma usada para expressar algo: um número, texto, código ou imagem. Um **registro** é a preservação dessa representação em algum suporte. Uma **afirmação** é o que alguém declara sobre uma situação. Uma **evidência** é um elemento que pode sustentar ou enfraquecer uma conclusão, sempre considerado com origem, método e contexto.

Imagine que o cadastro registra “renda mensal: 8.000”. O valor pode ter sido informado pelo cliente, extraído de documento, calculado, copiado de outra base ou inserido por engano. O campo não prova sozinho que a renda real é exatamente essa. Ainda assim, pode ser um dado necessário ao processo. A organização precisa decidir quais fontes aceita, que verificações realiza, por quanto tempo o valor permanece válido e quais decisões podem depender dele.

Esse cuidado é especialmente importante em sistemas corporativos. Um dado válido no formato pode estar incorreto no conteúdo. Um CPF pode ter quantidade de dígitos aceitável e pertencer a outra pessoa. Uma data pode respeitar o padrão esperado e ainda representar o mês errado. Uma conta pode existir tecnicamente e estar encerrada para a finalidade da operação. Validar formato reduz certos riscos; não estabelece verdade absoluta.

## Contexto, metadados e interpretação

O valor “1500” é ambíguo. Pode indicar reais, unidades, pontos, código, quantidade de clientes ou horário sem separador. Para interpretar, é preciso contexto: unidade, origem, momento, sujeito, finalidade, convenção, domínio de valores aceitos e relação com outros registros. O mesmo vale para um status como “pendente”: pendente de quê, desde quando, para qual processo, segundo qual regra e com qual responsável?

Uma parte desse contexto pode ser registrada como **metadado**, expressão que significa, em nível inicial, “dado sobre outros dados”. O nome de um campo, sua unidade, formato, origem, data de coleta, responsável, versão, regra de cálculo e nível de confidencialidade são exemplos de metadados. Eles ajudam pessoas e sistemas a localizar, interpretar, administrar e auditar dados. Não é necessário estudar governança de dados agora; basta perceber que sem descrição adequada uma coleção de valores pode se tornar difícil de usar ou perigosa de reutilizar.

Contexto não é apenas uma etiqueta. Ele depende de convenções e propósitos. A data `03/04/2026` pode ser 3 de abril ou 4 de março conforme a convenção. Uma taxa pode ser mensal ou anual. Um valor pode ser bruto ou líquido. Um código pode representar categoria em um sistema e estado em outro. A confiabilidade também faz parte do contexto: é diferente usar uma leitura de sensor calibrado, uma declaração sem comprovação e uma estimativa produzida por modelo.

Interpretar é relacionar dados e contexto para responder a alguma questão. Essa atividade pode ser feita por pessoa, por regra de software ou por ambos. Um programa pode interpretar um código conforme tabela definida e decidir qual procedimento executar. Uma pessoa pode interpretar um conjunto de indicadores considerando exceções, histórico e consequências. Nenhuma das duas interpretações é automaticamente infalível: a regra pode estar errada, os dados podem estar incompletos e a pessoa pode usar suposições inadequadas.

## Informação: organização significativa, não efeito automático

Nesta formação, informação é o resultado de dados organizados, comunicados ou interpretados de maneira significativa para uma finalidade. A formulação é operacional e outras áreas podem usar definições diferentes. O ponto central é que processamento técnico, por si só, não garante que haja informação útil.

Uma rotina pode ordenar registros, somar valores e gerar um relatório impecável do ponto de vista do formato. Se o período estiver errado, a unidade não estiver clara ou o relatório não responder à pergunta de quem o recebe, a saída pode ser tecnicamente correta e pouco informativa. Do mesmo modo, uma coleção de dados bem estruturada pode não ajudar alguém que não conhece sua origem, convenções ou limitações.

No caso de crédito, uma tabela pode informar à equipe operacional quais solicitações possuem documentos pendentes. Para uma equipe de risco, a mesma tabela pode ser apenas parte de uma análise maior, que exige histórico, políticas e comparação com outros sinais. Para o sistema que distribui tarefas, ela pode ser entrada para priorização. A mesma coleção não tem um único significado independente de uso. Organização, propósito e capacidade de interpretação participam do que ela informa.

Também é possível que uma informação gere novos dados. A decisão de pedir documento adicional, tomada após interpretar um risco, registra um novo evento. E conhecimento prévio influencia quais dados serão coletados: uma organização que sabe que determinada exceção é relevante pode criar campo específico para registrá-la. Por isso, a relação entre dados, informação e conhecimento não deve ser tratada como linha de mão única.

## Conhecimento: compreensão, ação e limites

Conhecimento não é apenas informação acumulada, nem é sinônimo de possuir muitos relatórios. Em sentido operacional para esta fase, envolve capacidade de relacionar informações, explicar por que algo ocorre, reconhecer padrões e limites, justificar uma conclusão e agir ou investigar de forma responsável.

Uma analista que observa atrasos recorrentes em solicitações não demonstra conhecimento somente por ler uma lista. Ela compara períodos, reconhece como o processo funciona, verifica se a mudança de regra coincidiu com o aumento, procura exceções e sabe quais perguntas ainda não podem ser respondidas. Essa capacidade combina informações disponíveis com experiência, modelos mentais, critérios de qualidade e disposição para revisar uma hipótese.

Filosofia e Ciência da Informação discutem extensamente o que torna uma crença conhecimento e como conhecimento pode ser pessoal, coletivo, explícito ou prático. Esta aula não resolverá esses debates. O uso adotado aqui é suficiente para evitar duas simplificações: que conhecimento seja simplesmente uma pilha de dados e que uma decisão seja correta apenas porque possui números associados.

Conhecimento prático pode existir sem estar todo registrado em um sistema. Um operador experiente pode perceber que uma rotina terminou em horário incomum e investigar antes de receber alerta formal. Ao mesmo tempo, esse conhecimento precisa ser documentado e compartilhado quando se torna essencial à operação; caso contrário, a organização depende de uma pessoa específica e perde capacidade de explicar ou repetir procedimentos.

## O modelo DIKW: utilidade e limites

DIKW é sigla usada para representar data, information, knowledge e wisdom — em português, dado, informação, conhecimento e sabedoria. A hierarquia é influente em literatura de informação e gestão do conhecimento e costuma ser desenhada como pirâmide ou sequência. Ela pode ajudar o iniciante a perceber que registrar valores não é o mesmo que compreender uma situação e agir com bom julgamento.

O modelo, porém, deve ser usado como lente didática, não como descrição universal de como pessoas, organizações ou computadores aprendem. A literatura registra diferentes representações e críticas à hierarquia. Nem toda informação nasce de dados em uma sequência simples; conhecimento prévio orienta a observação e a coleta; dados podem ser produzidos a partir de modelos; e grandes volumes de registros não criam automaticamente conhecimento ou sabedoria.

No caso de crédito, a política da organização — uma forma de conhecimento institucional — define quais dados serão pedidos. As respostas coletadas são registros. A combinação delas com regras e contexto pode informar uma análise. A decisão gera novos eventos, que viram dados para auditoria e aprendizado. O fluxo tem retornos, escolhas e incertezas; não é uma escada automática.

Sabedoria aparece na sigla apenas para contextualizar o modelo. Nesta fase, não será definida como competência técnica mensurável. O importante é entender por que a pirâmide é atraente e onde ela falha: ela simplifica relações complexas entre representação, significado, experiência, julgamento e ação.

## Qualidade dos dados e adequação ao uso

Qualidade de dados não é uma única propriedade e não equivale a verdade absoluta. Diferentes organizações e finalidades escolhem dimensões e métricas diferentes. Em nível inicial, algumas dimensões recorrentes são exatidão, validade, completude, consistência, atualidade, unicidade, integridade e relevância.

**Exatidão** pergunta até que ponto o valor representa corretamente aquilo que pretende representar. **Validade** pergunta se ele atende a formato, domínio ou regra definida. **Completude** pergunta se os elementos necessários estão presentes. **Consistência** observa ausência de contradição entre valores ou fontes. **Atualidade** considera se o dado ainda serve ao momento de uso. **Unicidade** procura evitar registros duplicados indevidamente. **Integridade** observa relações que precisam ser preservadas, como vínculo válido entre conta e cliente. **Relevância** pergunta se o dado é necessário para a finalidade em questão.

Essas dimensões não formam lista universal e podem entrar em conflito. Para enviar uma mensagem de cobrança hoje, atualidade do endereço pode ser decisiva. Para auditoria de uma decisão passada, preservar o valor histórico pode ser mais importante que substituí-lo pelo endereço atual. Um dado pode ser completo e inexato, válido no formato e irrelevante, ou consistente entre sistemas que repetem o mesmo erro. Qualidade significa adequação ao uso sob critérios explícitos, não selo definitivo de verdade.

## Evidência, interpretação e decisão

Dado pode apoiar decisão sem provar sozinho uma conclusão. Um **indício** é algo que sugere possibilidade e orienta investigação. Uma **evidência** é um elemento considerado para sustentar ou questionar uma afirmação, levando em conta origem, método, qualidade e relação com outras evidências. **Interpretação** atribui sentido a esse conjunto. **Conclusão** é uma afirmação que se considera sustentada provisoriamente. **Decisão** é uma escolha ou ação tomada sob regras, objetivos e responsabilidade.

No caso progressivo, renda declarada alta pode ser indício de capacidade de pagamento. Documento verificável, histórico de pagamento e regra de política podem fortalecer ou enfraquecer a análise. Mesmo assim, uma concessão de crédito envolve risco e não uma certeza sobre o futuro. O sistema ajuda a registrar, calcular, comparar e aplicar regras; pessoas e processos precisam definir critérios, lidar com exceções e responder pelas consequências.

Essa distinção protege contra dois extremos: desconfiar de todo dado a ponto de não conseguir operar e confiar em qualquer dado porque foi armazenado por um sistema. O trabalho técnico responsável pergunta o que o valor representa, de onde veio, para que serve, que limitações tem e que decisão ele pode ou não sustentar.

## Dados em sistemas corporativos

Sistemas corporativos organizam cadastros, movimentações, eventos, documentos e históricos para sustentar atividades reais. Um cadastro descreve entidades relevantes, como cliente, produto, contrato ou conta. Uma movimentação registra algo que ocorreu ao longo do tempo, como pagamento, alteração, transferência ou venda. Um evento marca ocorrência significativa, como solicitação recebida, aprovação, falha ou tentativa de acesso. Um histórico preserva versões e acontecimentos para consulta e explicação posterior.

No caso de crédito, o cadastro identifica a pessoa e suas relações; documentos e declarações registram fontes; consultas externas produzem dados recebidos; cálculos geram indicadores derivados; a decisão registra status, justificativa e responsável; mudanças posteriores integram o histórico. O sistema não deve apagar a diferença entre valor atual, valor usado em uma decisão passada e estimativa projetada para o futuro.

Rastreabilidade é a capacidade de acompanhar origem, transformação e destino de dados, decisões ou eventos. Ela permite perguntar quem registrou um valor, qual versão de regra foi aplicada, que fonte foi usada e como uma classificação foi calculada. Auditoria usa essa capacidade para examinar ações, controles e resultados. Rastreabilidade não torna uma decisão automaticamente correta; torna possível investigar e justificar o que ocorreu.

## Relação com as aulas anteriores e posteriores

Na Aula 02, sistema foi apresentado como conjunto de componentes relacionados. Nesta aula, dados mostram uma das coisas que esses componentes recebem, preservam e transformam. Na Aula 03, hardware, software e pessoas foram diferenciados. Hardware oferece recursos para armazenar e processar representações; software aplica estruturas e regras; pessoas definem significado, corrigem registros, interpretam resultados e assumem responsabilidade.

A próxima aula estudará processamento: como entradas podem ser transformadas por operações, regras e decisões. Depois, o modelo entrada, processamento e saída ajudará a descrever fluxos. Mais adiante, programa, arquivo, ambiente e erro dependerão desta base: programa manipula representações segundo regras; arquivo preserva dados e metadados; ambiente influencia como são usados; e problemas podem surgir de dados, regras, interpretação ou operação.

## Conexão futura com Mainframe e COBOL

Mainframe e COBOL serão estudados em contextos nos quais registros, campos, valores monetários, datas, códigos, históricos e regras de negócio precisam ser tratados com precisão. A preparação não é apenas aprender a mover valores entre campos. É compreender o que eles representam, que formato e origem possuem, em que período valem e que consequência pode surgir se forem interpretados ou processados incorretamente.

Em processamento batch, um arquivo pode conter dados de entrada, dados derivados, rejeições e resultados de conferência. Uma rotina pode executar corretamente e ainda produzir saída inadequada se a fonte estiver desatualizada, se a regra não corresponder à política vigente ou se a evidência for insuficiente para a decisão. A base construída aqui ajuda a fazer perguntas antes de alterar um processo ou confiar em um relatório.

## Confusões comuns de iniciantes

Uma confusão comum é chamar todo valor armazenado de fato verdadeiro. Registro não é prova automática: pode ser observação, declaração, estimativa, simulação ou erro. Outra é pensar que dado bruto é necessariamente “sem significado”; um dado pode já vir de processo rico, mas ainda exigir contexto para quem o reutiliza.

Também é comum imaginar que processar produz informação automaticamente. Um cálculo pode ser correto e responder à pergunta errada. Informação depende de organização, finalidade e interpretação. Da mesma forma, receber informação não garante conhecimento: podem faltar comparação, experiência, explicação, evidência ou compreensão dos limites.

Há quem trate DIKW como regra natural e sempre ascendente. O modelo é útil para discussão, mas conhecimento pode orientar coleta de dados, dados podem ser derivados de modelos e decisões produzem novos registros. Por fim, validar formato não é provar conteúdo: validade, exatidão, completude e atualidade são dimensões diferentes de qualidade.

## Perguntas para reflexão

- O valor `1500` é dado, informação ou ambos? Que contexto muda sua interpretação?
- Como distinguir uma observação de uma afirmação registrada por alguém?
- Por que um dado válido no formato pode estar incorreto para a decisão?
- Em uma análise de crédito, que diferença existe entre renda declarada, renda calculada e renda projetada?
- Como metadados ajudam a interpretar um relatório meses depois de sua geração?
- Por que grandes volumes de registros não garantem conhecimento útil?
- Em que sentido conhecimento anterior pode influenciar quais dados serão coletados?
- Que evidências seriam necessárias antes de transformar um indício em conclusão operacional?

## Síntese da aula

Dados são representações usadas por pessoas e sistemas. Podem ser observados, informados, derivados, estimados, sintéticos ou hipotéticos; por isso, não devem ser confundidos com fatos verdadeiros por definição. Seu significado depende de contexto, metadados, convenções, origem, qualidade e finalidade.

Nesta formação, informação é entendida como dados organizados, comunicados ou interpretados de modo significativo para uma atividade ou pergunta. Conhecimento envolve compreender relações, explicar, reconhecer limites e agir ou investigar de forma responsável. O modelo DIKW ajuda a visualizar essas diferenças, mas não descreve fluxo obrigatório ou universal.

Qualidade não é selo único: exatidão, validade, completude, consistência, atualidade, unicidade, integridade e relevância podem ser avaliadas conforme o uso. Dados podem apoiar evidências e decisões, mas não provam sozinhos uma conclusão. A próxima aula mostrará como dados e regras participam do processamento, sem perder de vista o contexto que lhes dá sentido.

## Mini glossário da aula

**Dado**: representação registrada, recebida, produzida ou usada por um processo, interpretável em contexto; pode ser observada, declarada, calculada, estimada, sintética ou hipotética.

**Dado observado**: dado obtido por observação ou medição de condição ou evento.

**Dado derivado**: dado produzido a partir de outros dados por cálculo, combinação ou regra.

**Dado sintético**: dado criado artificialmente para teste, simulação, treinamento ou pesquisa.

**Metadado**: dado que descreve, localiza, interpreta ou administra outros dados, como origem, unidade, formato ou data de coleta.

**Contexto**: elementos que permitem interpretar uma representação, como finalidade, unidade, origem, momento, regra e domínio.

**Informação**: dados organizados, comunicados ou interpretados de modo significativo para determinado propósito; definição operacional desta fase.

**Conhecimento**: capacidade de compreender relações, explicar, reconhecer limites e agir ou investigar com base em informações, experiência, modelos e justificativas.

**DIKW**: modelo que relaciona dado, informação, conhecimento e sabedoria; útil como lente didática, não como sequência universal.

**Evidência**: elemento usado para sustentar ou questionar uma afirmação, considerado com sua origem, método e limitações.

**Interpretação**: atribuição de sentido a dados e evidências em determinado contexto.

**Qualidade dos dados**: adequação de dados ao uso pretendido segundo dimensões e critérios explícitos.

**Exatidão**: grau em que um dado representa corretamente aquilo que pretende representar.

**Validade**: atendimento a formato, domínio ou regra definida; não garante exatidão no mundo real.

**Consistência**: ausência de contradições relevantes entre valores, regras ou fontes.

**Atualidade**: adequação temporal do dado para o uso pretendido.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir explicar por que dado, informação e conhecimento possuem definições diferentes conforme a área e declarar a definição operacional adotada pela fase. Deve reconhecer dado observado, informado, derivado, sintético e hipotético, sem assumir que todo dado é fato verdadeiro.

Deve explicar como contexto, metadados, origem, convenção, qualidade e finalidade influenciam interpretação. Também deve diferenciar validade de exatidão e mostrar por que qualidade de dados não é sinônimo de verdade absoluta.

O aluno deve apresentar o DIKW como modelo didático influente e discutido, indicando ao menos um limite: conhecimento pode orientar coleta, dados podem ser derivados e processamento não produz automaticamente informação útil. Deve distinguir dado, indício, evidência, interpretação, conclusão e decisão em cenário simples.

Por fim, deve analisar o caso de crédito ou situação equivalente, identificando fontes, dados derivados, incertezas, regras, evidências e riscos de decisão. Essa base será necessária para estudar processamento, programas, arquivos, ambientes e erros sem reduzir sistemas a valores isolados.

## Referências e leituras para aprofundamento

- ZINS, Chaim. *Conceptual approaches for defining data, information, and knowledge*. Journal of the American Society for Information Science and Technology, 2007.
- ROWLEY, Jennifer. *The wisdom hierarchy: representations of the DIKW hierarchy*. Journal of Information Science, 2007.
- DAMA International. *DAMA-DMBOK 2.0 Revision* e materiais institucionais sobre qualidade e metadados.
- Governo do Reino Unido. *The Government Data Quality Framework*.
