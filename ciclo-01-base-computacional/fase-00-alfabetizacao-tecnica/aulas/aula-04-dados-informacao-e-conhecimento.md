# Aula 04 — Dados, informação e conhecimento

## Objetivo da aula

O objetivo desta aula é construir uma compreensão sólida da diferença entre dado, informação e conhecimento. Ao final, o aluno deve conseguir explicar que um dado é uma representação registrada de algum fato, valor, evento ou característica; que informação surge quando dados são interpretados em contexto; e que conhecimento envolve a capacidade humana ou organizacional de usar informações compreendidas para decidir, agir, investigar ou formular novas perguntas.

Esta aula também prepara a sequência da Fase 0. As aulas anteriores mostraram que tecnologia da informação existe para lidar com informação, que sistemas são conjuntos de componentes relacionados e que hardware, software e pessoas participam desses sistemas. Agora, o foco passa para aquilo que circula entre esses elementos: os dados. Entender dados é necessário antes de estudar processamento, entrada e saída, programas, arquivos, ambientes e erros.

## O problema que esta aula resolve

Muitos iniciantes tratam dado, informação e conhecimento como se fossem palavras equivalentes. Em conversas informais, isso pode não causar grande problema. Em tecnologia, porém, a confusão prejudica a análise de sistemas. Um número armazenado não é automaticamente informação útil. Um relatório gerado não garante compreensão. Uma pessoa que recebeu uma informação pode ainda não ter conhecimento suficiente para tomar uma boa decisão.

Essa confusão atrapalha sistemas computacionais porque programas não trabalham com "significado" da mesma forma que pessoas. Eles manipulam representações. Se o dado foi registrado errado, se o campo foi mal entendido, se a unidade não foi informada, se a origem é duvidosa ou se a regra de negócio foi aplicada fora de contexto, o sistema pode executar tecnicamente e ainda produzir resultado inadequado. Em sistemas corporativos, isso pode gerar cobrança indevida, pagamento errado, relatório distorcido, atendimento ruim, falha de auditoria ou decisão gerencial frágil.

## Introdução

Na Aula 01, tecnologia da informação foi apresentada como uso organizado de recursos técnicos, pessoas, processos e métodos para lidar com informações. Na Aula 02, o conceito de sistema mostrou que partes relacionadas atuam com uma finalidade. Na Aula 03, hardware, software e pessoas foram observados como componentes centrais de sistemas computacionais e sistemas de informação.

A partir desse ponto, surge uma pergunta inevitável: o que esses sistemas manipulam? Pessoas informam dados, softwares aplicam regras sobre dados, hardwares armazenam e processam dados, processos definem por que certos dados importam, e organizações usam resultados para decidir. Portanto, dados não são detalhes periféricos. Eles são o conteúdo sobre o qual muitos sistemas trabalham.

Mesmo assim, dados não falam sozinhos. O valor "1000" pode estar em uma tela, em um relatório ou em um arquivo, mas ainda não diz o que significa. Pode ser salário, saldo, código, quantidade, limite, agência, pontuação, parcela, tarifa ou outra coisa. Para virar informação, o valor precisa de contexto. Para apoiar decisão, a informação precisa ser compreendida. Para gerar ação correta, essa compreensão precisa ser ligada a regras, experiência e finalidade.

## Por que dados estão no centro da tecnologia da informação

Tecnologia da informação existe, em grande parte, para lidar com dados e transformá-los em informação útil para pessoas, processos e organizações. Uma empresa registra vendas, clientes, contratos, pagamentos, produtos, documentos, eventos e decisões. Um banco registra contas, movimentações, saldos, limites, autorizações e transações. Um órgão público registra solicitações, benefícios, documentos, análises e históricos. Em todos esses casos, sistemas existem para capturar, armazenar, proteger, validar, processar, consultar e apresentar dados.

Computadores não entendem o mundo como pessoas entendem. Uma pessoa pode olhar para uma situação e reconhecer intenção, urgência, risco, exceção ou contexto social. Um computador manipula representações segundo regras definidas. Para que ele trate um pagamento, por exemplo, valores, datas, contas, identificadores, status e autorizações precisam estar representados de algum modo. Essas representações precisam ser registráveis e manipuláveis.

Essa ideia é importante porque evita uma ilusão comum: achar que o sistema "sabe" o que está acontecendo. O sistema pode armazenar um código de cliente, calcular um saldo, marcar um status ou gerar uma mensagem. Mas o significado desses elementos depende de campos, regras, tabelas de referência, processos e interpretação humana. A TI organiza essa relação para que representações computacionais possam apoiar o trabalho real.

## O que é dado

Dado é uma representação registrada de um fato, valor, observação, evento ou característica. Um dado pode ser um número, texto, data, código, status, valor monetário, identificador, marcação, opção, sinal ou qualquer outra forma que possa ser registrada e processada. Um CPF informado em um cadastro, uma data de vencimento, um valor de compra, um código de produto, uma situação cadastral e uma marcação de aprovação são exemplos de dados.

O dado não precisa estar em um computador para existir. Uma anotação em papel, uma ficha preenchida, um formulário impresso, uma etiqueta, um protocolo e uma planilha manual também podem conter dados. Em computação, porém, o dado precisa assumir alguma forma que possa ser registrada, armazenada, transmitida, comparada, validada ou processada por um sistema. Isso exige estrutura: campo, formato, unidade, origem, identificação e relação com outros dados.

Em uma empresa, "data de admissão" é um dado porque representa um fato relevante sobre um funcionário. Em um comércio, "quantidade em estoque" é um dado porque representa uma condição operacional de um produto. Em um banco, "saldo disponível" é um dado calculado ou mantido segundo regras. Em um órgão público, "situação do benefício" é um dado que representa o estado de um processo. Cada exemplo só faz sentido porque existe uma finalidade associada.

## Dado bruto, dado registrado e dado processado

Dado bruto é uma representação ainda pouco tratada, recebida ou observada antes de organização suficiente para uso confiável. Pode ser uma resposta livre em um formulário, uma leitura capturada por um dispositivo, um valor recebido de outro sistema ou uma informação digitada antes de validação. Ele pode ser útil, mas ainda precisa de conferência, estrutura ou contexto.

Dado registrado é aquele que foi gravado em algum suporte ou sistema com uma forma definida. Quando um atendente informa nome, documento, telefone e endereço em campos específicos, esses valores deixam de ser apenas observações soltas e passam a fazer parte de um registro. O registro não garante automaticamente que tudo esteja correto, mas permite que o dado seja consultado, validado, relacionado e usado em processos posteriores.

Dado processado é aquele que passou por alguma transformação, cálculo, classificação, validação, combinação ou seleção. Um valor total de compra pode ser resultado da soma de itens. Um saldo pode refletir créditos, débitos, bloqueios e regras de disponibilidade. Um status "aprovado" pode resultar da aplicação de critérios sobre documentos e renda. O mesmo valor pode mudar de utilidade conforme o contexto: "1000" isolado comunica pouco; "saldo disponível: R$ 1.000,00 em 03/07/2026" já comunica muito mais.

## O que é informação

Informação é dado interpretado em contexto, organizado de forma que reduza incerteza ou apoie entendimento. A informação depende de significado, contexto, estrutura e finalidade. Um valor solto pode ser dado; esse mesmo valor, quando apresentado como parte de uma consulta, relatório, mensagem ou extrato, pode se tornar informação para alguém.

Um saldo de conta é informação quando o cliente entende que aquele valor representa recursos disponíveis segundo determinada regra e em determinado momento. Um extrato bancário organiza dados de movimentação para que a pessoa compreenda entradas, saídas, datas, descrições e saldos. Um relatório de vendas transforma registros de operações em informação sobre desempenho, produtos vendidos, períodos e valores. Uma situação cadastral informa se uma pessoa ou empresa está ativa, bloqueada, pendente ou irregular dentro de um processo.

Na folha de pagamento, dados como salário base, horas extras, descontos, benefícios e impostos se tornam informação quando organizados em demonstrativo compreensível. Em movimentação financeira, registros de débito e crédito se tornam informação quando permitem entender origem, destino, data, valor e situação de uma operação. A informação não está apenas no dado, mas na forma como o dado é situado para responder a uma necessidade.

## O que é conhecimento

Conhecimento é a capacidade de usar informações compreendidas para interpretar situações, tomar decisões, reconhecer padrões, agir corretamente ou formular novas perguntas. Conhecimento não é apenas acumular dados nem apenas ler relatórios. Ele envolve compreensão, experiência, interpretação, julgamento e relação com regras ou objetivos.

Um analista que interpreta rejeições em um arquivo não está apenas lendo mensagens. Ele reconhece padrões, compara ocorrências, entende regras e identifica possíveis causas. Um gerente que observa aumento de inadimplência não olha apenas para uma porcentagem; ele interpreta tendência, compara períodos, considera contexto econômico, avalia risco e decide que ação tomar. Um operador que acompanha uma rotina pode reconhecer comportamento anormal porque conhece horários, volumes esperados, mensagens usuais e consequências de atraso.

Um desenvolvedor, futuramente, não deverá alterar uma regra apenas porque localizou um campo ou uma condição. Ele precisará compreender que informação aquele dado representa, que processo depende dele, que exceções existem e que impacto a alteração pode produzir. Esse tipo de conhecimento conecta dado, informação, regra, sistema e responsabilidade.

## A relação entre dado, informação e conhecimento

A relação pode ser vista como uma progressão: dado → informação → conhecimento. O dado é a representação registrada. A informação surge quando esse dado ganha contexto e significado para uma finalidade. O conhecimento aparece quando a informação é compreendida e usada para decidir, agir ou investigar.

Essa progressão não é automática. Um sistema pode armazenar milhões de dados e ainda produzir pouca informação útil. Isso acontece quando dados são mal organizados, têm baixa qualidade, não possuem contexto ou são apresentados de forma inadequada. Da mesma forma, uma pessoa pode receber informação e ainda não ter conhecimento suficiente para tomar boa decisão. Um relatório pode mostrar queda de vendas, mas a interpretação exige entender produto, período, canal, preço, estoque, sazonalidade e comportamento do cliente.

Qualidade, contexto, organização e interpretação são essenciais. Sem qualidade, a informação fica contaminada. Sem contexto, o significado fica instável. Sem organização, o volume atrapalha em vez de ajudar. Sem interpretação, a informação pode ser ignorada, mal usada ou aplicada fora da situação correta.

## Contexto: o que dá significado ao dado

Contexto é o conjunto de elementos que permite interpretar um dado corretamente. Um dado precisa de campo, unidade, origem, data, regra, formato, finalidade e relação com outros dados. Sem esses elementos, o valor pode existir, mas seu significado permanece incerto.

Um valor monetário sem moeda pode ser ambíguo. Cem unidades podem representar reais, dólares, pontos, parcelas ou quantidade de itens. Uma data sem contexto também é frágil: pode ser nascimento, vencimento, pagamento, cadastro, atualização ou cancelamento. Um código sem tabela de referência é apenas uma sequência de caracteres. Um status sem regra de negócio pode ser interpretado de várias formas: "pendente" pode significar aguardando documento, aguardando aprovação, aguardando pagamento ou aguardando integração.

Um número de conta sem agência pode não identificar corretamente uma relação bancária. Um CPF sem papel associado também pode confundir: ele pode ser do titular, dependente, beneficiário, representante, procurador ou responsável legal. O dado precisa ser ligado à pergunta que está sendo respondida. "Quem é essa pessoa no processo?" é diferente de "quem recebeu o pagamento?" ou "quem autorizou a operação?".

## Dados em sistemas corporativos

Em um cadastro de clientes, dados descrevem entidades relativamente estáveis: nome, documento, endereço, telefone, e-mail, situação cadastral e preferências autorizadas. Esses dados sustentam atendimento, cobrança, entrega, análise de crédito, emissão de documentos e comunicação. Se o endereço está incorreto ou se o documento foi cadastrado com erro, várias áreas podem ser afetadas.

Em um cadastro de contas, dados representam relações financeiras: número de conta, agência, titularidade, tipo, status, limites, permissões e datas relevantes. Esses dados orientam consultas, movimentações, bloqueios, liberações e auditoria. Uma conta ativa ou bloqueada não é apenas uma informação visual; é uma condição usada por regras de operação.

Na folha de pagamento, dados de funcionário, cargo, salário, jornada, faltas, horas extras, benefícios e descontos alimentam cálculos e obrigações legais. Um dado incompleto pode impedir pagamento; um dado incorreto pode gerar valor errado; um dado desatualizado pode afetar imposto, benefício ou relatório contábil.

Em estoque, dados de produto, quantidade, localização, entrada, saída, reserva e custo ajudam a controlar disponibilidade. Uma venda depende desses dados para saber se o produto existe, se pode ser entregue e qual consequência terá no saldo de estoque. Em emissão de nota, dados de cliente, produto, valor, tributação e operação precisam estar coerentes para que o documento represente corretamente a transação.

Na concessão de benefício público, dados de cidadão, documentos, critérios legais, renda, vínculos, análise, decisão e histórico sustentam um processo sensível. A decisão precisa ser explicável, e os dados usados precisam ser rastreáveis. Em movimentação bancária, cada débito, crédito, autorização, horário e identificador participa de saldos, extratos, conciliações e controles antifraude.

## Cadastro, movimentação, evento, registro e histórico

Cadastro é um conjunto organizado de dados sobre entidades relevantes, como clientes, produtos, contas, contratos, funcionários ou beneficiários. Ele descreve algo que tende a permanecer válido por algum tempo, ainda que possa mudar. Nome, documento, endereço, situação e tipo de conta são exemplos de dados cadastrais.

Movimentação é o registro de uma ação ou alteração que acontece ao longo do tempo. Uma compra, pagamento, transferência, entrada de estoque, saída de produto, desconto aplicado ou atualização salarial pode ser uma movimentação. Enquanto cadastro descreve uma entidade, movimentação descreve acontecimentos associados a ela.

Evento é uma ocorrência significativa para o sistema ou processo. Pode ser uma solicitação recebida, uma aprovação, uma recusa, uma alteração de status, uma tentativa de acesso, uma emissão de documento ou uma falha registrada. Registro é uma unidade organizada de dados que descreve uma entidade, movimentação ou evento. Histórico é a preservação de registros ao longo do tempo para consulta, análise, auditoria ou reconstrução do que ocorreu.

Essa distinção é inicial, mas importante. Cadastro de cliente não é a mesma coisa que histórico de transações do cliente. O cadastro pode dizer quem é o cliente; o histórico mostra o que aconteceu com ele em determinado período. Fases futuras tratarão arquivos, bancos de dados e estruturas com mais detalhe, mas a base conceitual começa aqui.

## Qualidade dos dados

Dados precisam ter qualidade porque decisões, processos e sistemas dependem deles. Dado incorreto representa algo de forma errada, como CPF digitado com número trocado, valor de salário errado ou produto vinculado a código indevido. A consequência pode ser pagamento errado, cobrança indevida, erro de identificação ou relatório distorcido.

Dado incompleto não possui todos os elementos necessários para uso. Um cadastro sem documento, uma cobrança sem vencimento, uma conta sem titularidade clara ou uma solicitação sem comprovação podem bloquear processo ou levar a decisão insegura. Dado duplicado ocorre quando a mesma entidade ou ocorrência aparece mais de uma vez sem controle adequado. Isso pode gerar cobrança repetida, cliente duplicado, estoque inflado ou análise estatística distorcida.

Dado inconsistente entra em conflito com outro dado ou regra. Um pagamento marcado como realizado em um sistema e pendente em outro cria divergência operacional. Uma data de pagamento anterior à data de emissão pode indicar erro ou exceção que precisa ser explicada. Dado desatualizado já não representa corretamente a situação atual, como endereço antigo, cargo alterado, conta encerrada ou regra vencida.

Dado ambíguo permite mais de uma interpretação. Um campo "responsável" pode significar responsável financeiro, responsável legal ou usuário que registrou a operação, se o sistema não define claramente. Dado fora de formato pode impedir validação, comparação ou integração. Dado sem origem confiável prejudica credibilidade. Dado sem rastreabilidade dificulta saber quem registrou, quando registrou, por que registrou e que processo gerou aquela informação.

## Dados, regras e validação

Dados não são tratados isoladamente. Eles são avaliados segundo regras. Uma regra pode determinar que um campo é obrigatório, que uma data precisa estar em formato válido, que um valor não pode ser negativo, que um código deve existir em uma referência, que determinada operação exige permissão ou que uma situação cadastral impede uma ação.

Validar dados significa verificar se eles atendem a expectativas definidas. Uma validação pode conferir formato, obrigatoriedade, limite, relação entre campos, compatibilidade de datas, existência de código, autorização de usuário ou consistência com dados já registrados. Em um cadastro, o sistema pode exigir documento válido e endereço mínimo. Em uma folha, pode verificar se o evento informado é permitido para aquele tipo de vínculo. Em uma cobrança, pode conferir se valor, vencimento e contrato estão compatíveis.

Validação não é garantia absoluta de verdade. Um dado pode passar por validações formais e ainda estar errado no mundo real. Um telefone pode ter formato correto e não pertencer mais ao cliente. Um endereço pode estar completo e desatualizado. Por isso, sistemas combinam validações técnicas, regras de negócio, procedimentos humanos e revisões quando necessário.

## Rastreabilidade, histórico e auditoria

Sistemas corporativos precisam saber de onde veio um dado, quando foi registrado, quem alterou, qual processo gerou, qual regra foi aplicada e qual resultado foi produzido. Essa capacidade é chamada de rastreabilidade. Ela permite reconstruir acontecimentos, investigar problemas e demonstrar responsabilidade.

Histórico preserva mudanças e eventos ao longo do tempo. Sem histórico, uma organização pode até saber o estado atual de um cadastro, mas não consegue explicar como chegou ali. Saber que um benefício está aprovado é importante; saber quando foi solicitado, quem analisou, quais documentos foram usados e que regra sustentou a decisão pode ser igualmente necessário.

Auditoria depende de rastreabilidade e histórico. Bancos, órgãos públicos, seguradoras e sistemas críticos precisam demonstrar que dados e decisões foram tratados corretamente. Quando há cobrança contestada, pagamento divergente, benefício negado ou alteração cadastral suspeita, não basta olhar a tela atual. É preciso examinar registros, eventos, origens, regras aplicadas e responsáveis.

## Dados e os elementos das aulas anteriores

Dados se conectam diretamente com tecnologia da informação porque TI organiza coleta, armazenamento, processamento, proteção, transmissão, consulta e uso de informações. Sem dados, a tecnologia perde parte central de sua finalidade. Com dados ruins, a tecnologia pode acelerar erros.

Dados se conectam com o conceito de sistema porque circulam entre componentes. Uma entrada recebida por um usuário pode ser validada por software, armazenada em hardware, consultada por outro processo e apresentada como saída. A relação entre componentes define como o dado entra, muda, permanece e é usado.

Hardware armazena e processa dados fisicamente, por meio de memória, armazenamento, CPU, rede e dispositivos. Software organiza estruturas, aplica regras, valida formatos, calcula resultados e apresenta informações. Pessoas informam, interpretam, corrigem, autorizam e decidem. Processos definem finalidade, etapas e responsabilidades. Sistemas coordenam esses elementos para produzir resultado útil.

## Conexão futura com Mainframe e COBOL

Mainframe e COBOL serão estudados futuramente em ambientes onde dados são estruturados, validados, processados e preservados com grande rigor. Muitas organizações usam sistemas corporativos para lidar com cadastros, movimentações, arquivos, registros, valores monetários, códigos, históricos e regras de negócio que precisam permanecer consistentes por muito tempo.

COBOL será apresentado futuramente como uma linguagem historicamente forte em lidar com dados de negócio. O interesse não estará apenas na sintaxe da linguagem, mas no tipo de problema que ela expressa: ler dados, organizar registros, aplicar regras, calcular valores, produzir saídas e preservar significado em processos corporativos. Mainframe será entendido como ambiente em que essas responsabilidades podem aparecer em escala, com operação, segurança, controle e continuidade.

Esta aula não ensina COBOL, arquivos técnicos ou bancos de dados. Ela prepara a compreensão necessária: antes de manipular dados em qualquer tecnologia, é preciso entender o que os dados representam, que contexto dá significado a eles, que qualidade precisam ter e que consequências surgem quando são tratados incorretamente.

## Confusões comuns de iniciantes

Uma confusão comum é achar que dado e informação são a mesma coisa. O dado é uma representação registrada; a informação depende de interpretação em contexto. Um número em uma coluna pode ser dado. Esse mesmo número, com nome do campo, unidade, período e finalidade, pode informar algo.

Outra confusão é achar que qualquer relatório é automaticamente útil. Um relatório pode ser tecnicamente gerado e ainda ser confuso, incompleto, atrasado ou baseado em dados ruins. Para ser útil, precisa responder a uma pergunta, apresentar contexto e permitir interpretação adequada.

Também é comum achar que dado errado é problema pequeno. Em sistemas corporativos, um único campo incorreto pode afetar cobrança, pagamento, atendimento, auditoria, integração e decisão. O erro pode se espalhar porque sistemas reutilizam dados em vários processos.

Muitos iniciantes acham que basta armazenar dados. Guardar dados sem qualidade, contexto, organização e finalidade pode apenas acumular volume. O valor está em permitir recuperação, interpretação, processamento e uso responsável.

Ignorar contexto é outra falha frequente. Um valor, data, código ou status sem campo, origem e regra pode ser interpretado de forma errada. Ignorar origem do dado também é perigoso, porque dados vindos de fontes diferentes podem ter níveis diferentes de confiabilidade, atualização e significado.

Há ainda a tendência de ignorar qualidade. Dados duplicados, inconsistentes, desatualizados ou ambíguos geram trabalho extra e decisões ruins. Confundir cadastro com movimentação também causa problemas: dados cadastrais descrevem entidades; movimentações registram acontecimentos. Misturar essas noções dificulta entender histórico.

Outra confusão é tratar dado como tela. A tela apresenta ou coleta dados, mas não é o dado em si. O dado pode estar armazenado, processado, transmitido, validado e usado por outras partes do sistema. Por fim, muitos iniciantes imaginam que o sistema entende significado como uma pessoa entende. Na prática, o sistema aplica regras sobre representações; o significado precisa ser modelado, registrado, validado e interpretado.

## Perguntas para reflexão

- Que informações faltam para interpretar corretamente o valor "1000" em um sistema?
- Por que um relatório gerado sem erro técnico pode ainda não apoiar uma decisão?
- Em um cadastro de clientes, quais dados descrevem a entidade e quais dados poderiam representar movimentações?
- Como um dado incorreto em uma folha de pagamento pode afetar outros processos?
- Que diferença existe entre registrar uma data e saber o significado dessa data?
- Por que a origem de um dado importa em uma auditoria?
- Em que situações uma informação pode ser recebida, mas não gerar conhecimento suficiente para agir?
- Como dados de baixa qualidade podem comprometer software, pessoas e processos ao mesmo tempo?

## Síntese da aula

Dados são centrais em tecnologia da informação porque representam fatos, eventos, valores e características que sistemas registram, armazenam, processam, protegem e apresentam. Mas dados isolados não bastam. Para se tornarem informação, precisam de contexto, estrutura, finalidade e interpretação. Para sustentarem conhecimento, precisam ser compreendidos e usados com julgamento.

Nesta aula, diferenciamos dado bruto, dado registrado, dado processado, informação apresentada e conhecimento aplicado. Também vimos que cadastros, movimentações, eventos, registros e históricos ajudam a organizar dados em sistemas corporativos, e que qualidade de dados é condição para decisões confiáveis. Dados incorretos, incompletos, duplicados, inconsistentes, desatualizados, ambíguos ou sem origem confiável podem produzir consequências sérias.

A próxima aula tratará de processamento. Depois de entender que dados precisam de significado, será possível estudar como sistemas transformam entradas em saídas por meio de regras, cálculos, comparações, validações e decisões.

## Mini glossário da aula

**Dado**: representação registrada de um fato, valor, observação, evento ou característica.

**Informação**: dado interpretado em contexto, organizado de modo a reduzir incerteza ou apoiar entendimento.

**Conhecimento**: capacidade de usar informações compreendidas para interpretar, decidir, agir ou investigar.

**Contexto**: conjunto de elementos que permite interpretar um dado, como campo, origem, unidade, regra, data e finalidade.

**Significado**: sentido atribuído a um dado quando ele é relacionado a contexto, estrutura e finalidade.

**Interpretação**: ato de compreender o que uma informação indica dentro de uma situação.

**Dado bruto**: dado recebido ou observado antes de tratamento, validação ou organização suficiente.

**Dado registrado**: dado gravado em algum suporte ou sistema com forma definida.

**Dado processado**: dado que passou por transformação, cálculo, validação, classificação ou combinação.

**Qualidade de dados**: grau em que dados são corretos, completos, consistentes, atualizados, claros e rastreáveis para uso pretendido.

**Cadastro**: conjunto organizado de dados sobre entidades relevantes, como clientes, produtos, contas ou funcionários.

**Movimentação**: registro de uma ação ou acontecimento que altera ou descreve atividade ao longo do tempo.

**Evento**: ocorrência significativa para um processo ou sistema, como solicitação, aprovação, pagamento, acesso ou falha.

**Registro**: unidade organizada de dados que descreve uma entidade, movimentação ou evento.

**Histórico**: preservação de registros e eventos ao longo do tempo para consulta, análise ou auditoria.

**Validação**: verificação de que dados atendem a formatos, regras, limites, relações e permissões esperadas.

**Consistência**: condição em que dados não entram em conflito entre si, com regras ou com o estado esperado do processo.

**Duplicidade**: ocorrência em que a mesma entidade ou evento aparece mais de uma vez sem controle adequado.

**Ambiguidade**: situação em que um dado ou campo permite mais de uma interpretação.

**Rastreabilidade**: capacidade de acompanhar origem, alteração, regra aplicada e destino de um dado ou decisão.

**Auditoria**: verificação de dados, ações e controles para demonstrar o que ocorreu e se regras foram respeitadas.

**Origem do dado**: fonte ou processo a partir do qual um dado foi obtido ou registrado.

**Regra de negócio**: condição, cálculo, restrição ou decisão que expressa uma necessidade organizacional.

**Decisão**: escolha ou ação tomada com base em informação, regra, contexto e responsabilidade.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir diferenciar dado, informação e conhecimento com exemplos próprios. Deve explicar por que contexto muda o significado de um dado e por que um valor isolado pode ser insuficiente para apoiar entendimento.

O aluno deve reconhecer dados em sistemas corporativos, como cadastros, contas, folha de pagamento, estoque, cobrança, emissão de nota, benefícios públicos e movimentações bancárias. Também deve diferenciar, em nível inicial, cadastro, movimentação, evento, registro e histórico.

Também é esperado que o aluno explique por que qualidade de dados importa. Ele deve identificar exemplos de dados incorretos, incompletos, duplicados, inconsistentes, desatualizados e ambíguos, relacionando esses problemas a consequências como pagamento errado, cobrança indevida, relatório distorcido, falha de auditoria ou decisão ruim.

O aluno deve compreender a relação entre dados, regras e validação, sem transformar isso ainda em programação. Deve conectar dados com tecnologia da informação, sistemas, hardware, software, pessoas e processos. Por fim, deve explicar por que dados serão essenciais para entender futuramente Mainframe e COBOL como temas ligados a registros, arquivos, processamento, regras de negócio e sistemas corporativos.
