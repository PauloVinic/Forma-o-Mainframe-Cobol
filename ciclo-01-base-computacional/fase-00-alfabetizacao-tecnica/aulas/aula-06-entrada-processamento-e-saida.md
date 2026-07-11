# Aula 06 — Entrada, processamento e saída

## Objetivo da aula

O objetivo desta aula é consolidar o modelo entrada, processamento e saída como uma forma inicial de descrever operações, sistemas e fluxos de informação. Ao final, o aluno deve conseguir observar uma situação simples ou corporativa e identificar que dados, documentos, comandos, eventos ou solicitações entram; que regras, validações, cálculos, decisões ou transformações acontecem; e que resultado é produzido para pessoas, processos ou outros sistemas.

Esta aula não apresenta programação nem ferramenta técnica. Ela organiza uma forma de pensar. Antes de estudar o que é um programa, é necessário entender que muitos problemas computacionais podem ser descritos como um fluxo: algo chega, algo é tratado, algo sai.

## O problema que esta aula resolve

Muitos iniciantes ouvem que computadores trabalham com entrada, processamento e saída, mas entendem essa ideia como uma fórmula decorada. Nessa visão limitada, entrada seria apenas aquilo que uma pessoa digita, processamento seria apenas "o computador fazendo alguma coisa" e saída seria apenas o que aparece na tela. Essa interpretação é insuficiente para compreender sistemas de informação.

Em organizações, entradas podem vir de formulários, arquivos recebidos, mensagens de outros sistemas, documentos, eventos, comandos, sensores, solicitações, parâmetros, regras configuradas e sinais de operação. O processamento pode envolver validação, cálculo, classificação, comparação, consulta, decisão, atualização e dados intermediários. A saída pode ser informação exibida, arquivo produzido, relatório, mensagem, registro atualizado, mudança de status, comprovante, alerta, lançamento contábil, resposta a outro sistema ou evidência de auditoria.

A dificuldade que esta aula resolve é enxergar o fluxo completo. Analisar apenas a tela final esconde a origem da informação. Analisar apenas a entrada ignora regras e transformações. Analisar apenas o processamento esquece que o resultado precisa servir a algum propósito.

## Introdução

Nas aulas anteriores, tecnologia da informação foi apresentada como uso organizado de recursos técnicos, pessoas, processos e métodos para lidar com dados, informação e decisões. Depois, sistema foi explicado como conjunto de componentes relacionados, com objetivo, fronteira, ambiente, interfaces, entradas, transformações e saídas. Em seguida, hardware, software e pessoas foram observados como elementos que atuam em conjunto. A aula sobre dados mostrou que valores registrados precisam de contexto para se tornarem informação. A aula sobre processamento explicou que dados são transformados por regras, instruções, operações e decisões.

Agora esses conceitos se juntam em um modelo de leitura. Entrada, processamento e saída não são três palavras isoladas. Elas formam uma maneira de observar como algo funciona. Uma operação existe porque algum elemento entra em um processo, sofre tratamento e produz algum resultado. Isso vale para processos humanos, administrativos, computacionais e corporativos.

Um atendimento recebe uma solicitação, analisa dados do cliente e produz uma resposta. Uma conferência documental recebe documentos, verifica critérios e produz aprovação ou pendência. Um sistema bancário recebe uma transação, aplica regras, registra movimentações e produz comprovante. Um processo de folha recebe eventos, calcula valores e produz pagamentos, demonstrativos e registros contábeis.

O modelo não substitui uma análise detalhada, mas cria um primeiro mapa para investigar origem, regra aplicada, resultado esperado, destinatário e consequência.

## O modelo entrada, processamento e saída

O modelo entrada–processamento–saída (EPS) é abstração útil para analisar origem, transformação e resultado. Entrada é aquilo que atravessa a fronteira escolhida e influencia o sistema; processamento aplica operações considerando regras, estado e contexto; saída é resultado, mudança ou efeito relevante. O modelo simplifica a realidade: pode ocultar estado persistente, feedback, concorrência, ambiente e interação. É ferramenta de análise, não descrição universal e completa.

Quando uma pessoa calcula o valor total de uma compra, os itens, preços, quantidades e descontos funcionam como entradas. O processamento envolve somar valores, multiplicar quantidades, aplicar desconto e considerar impostos ou regras comerciais. A saída pode ser o total a pagar, um recibo, uma nota, uma autorização de pagamento ou uma atualização no estoque. Mesmo antes de falar em computador, o fluxo já existe.

Em computação, esse modelo aparece porque sistemas recebem dados representados, executam instruções definidas e produzem resultados observáveis ou registráveis. Entender o que entra, o que é feito e o que sai ajuda a analisar comportamento, encontrar falhas e explicar consequências.

O modelo também evita confusões. Se uma saída está errada, a causa pode estar na entrada, na regra de processamento, em dados de referência, no ambiente, em uma integração, no destino da saída ou na interpretação humana do resultado. Sem separar essas partes, a análise vira chute.

## O que é entrada

Entrada é dado, sinal, documento, comando, solicitação, evento ou referência que atravessa a fronteira relevante e influencia o processamento. Não precisa ser digitada: pode vir de arquivo, outro sistema, dispositivo, mensagem ou parâmetro. Estado existente, configuração, versão, horário, identidade e recursos disponíveis nem sempre são entradas explícitas, mas são condições contextuais capazes de alterar resultado.

Um pedido de compra possui entradas como identificação do cliente, produtos solicitados, quantidades, endereço, forma de pagamento e condições comerciais. Uma análise de benefício pode receber documentos, dados cadastrais, histórico, datas, comprovantes e regras de elegibilidade. Uma rotina de cobrança pode receber contratos em aberto, valores, vencimentos, juros, pagamentos já registrados e parâmetros sobre quando cobrar.

Também existem entradas que não parecem dados no sentido comum. Um comando dado por uma pessoa é uma entrada. Uma regra configurada para determinada campanha é uma entrada. Um evento de "pagamento recebido" é uma entrada. Uma solicitação de consulta enviada por outro sistema é uma entrada. Um sinal de sensor, uma marcação de presença, uma autorização, uma senha, uma opção selecionada, uma data de referência e uma lista de registros também podem ser entradas.

Pensar entrada de forma ampla é essencial porque sistemas corporativos raramente dependem apenas de uma tela. Eles recebem dados de várias origens. Algumas entradas vêm de usuários, outras de sistemas internos, parceiros, arquivos, cadastros, tabelas de referência, eventos de negócio e configurações operacionais.

## Entrada em sistemas computacionais

Em sistemas computacionais, entrada é aquilo que o sistema consegue receber, ler ou recuperar para iniciar ou orientar uma operação. Um formulário preenchido por usuário é uma entrada visível. Um sistema que recebe um arquivo de uma área parceira também está recebendo entrada. Uma interface que recebe uma solicitação de outro sistema trabalha com dados de entrada. Uma rotina que recebe parâmetros de execução usa esses parâmetros como entrada para definir período, tipo de processamento ou conjunto de registros.

Um comando em terminal também pode ser entrada, porque orienta uma ferramenta ou sistema. Um sistema que lê dados armazenados para calcular um resultado trata esses dados como entrada daquele processamento. Um processo que recebe evento, como confirmação de pagamento, alteração cadastral ou solicitação de cancelamento, também reage a uma entrada.

O ponto importante é não aprofundar agora detalhes de rede, arquivos, interfaces técnicas ou programação. A ideia necessária nesta fase é conceitual: para que algo seja processado, alguma informação precisa estar disponível para o processo. Essa informação pode chegar no momento da operação ou já estar registrada em algum lugar acessível.

Entrada também tem origem e contexto. Não basta saber que um valor entrou no sistema; é preciso perguntar de onde veio, em que formato chegou, que significado tinha, se estava completo, se foi autorizado e se correspondia ao processo correto.

## O que é processamento dentro do modelo

Processamento, dentro do modelo, é o conjunto de tratamentos aplicados às entradas para produzir um resultado. Esse tratamento pode transformar dados, validar condições, calcular valores, comparar registros, classificar situações, consultar referências, tomar decisões, atualizar estados, rejeitar ocorrências ou preparar saídas.

Se a entrada é um pedido, o processamento pode verificar cadastro do cliente, conferir estoque, calcular total, aplicar regra de frete, avaliar forma de pagamento e definir se o pedido pode prosseguir. Se a entrada é uma solicitação de crédito, o processamento pode validar documentos, consultar histórico, comparar renda com limite desejado, aplicar políticas internas e classificar o risco. Se a entrada é uma lista de pagamentos, o processamento pode conferir valores, identificar duplicidades, atualizar contratos e gerar comprovantes.

Na computação, o processamento é orientado por instruções e regras. O sistema não entende intenção por conta própria. Ele executa aquilo que foi definido em software, configuração, regra de negócio ou procedimento operacional. Mesmo quando o resultado parece simples, há critérios por trás. Um status "aprovado" ou "rejeitado" pode depender de várias verificações anteriores.

O processamento não precisa ser visível para o usuário. Muitas transformações acontecem internamente. Um sistema pode consultar um cadastro, combinar registros, validar permissões, gerar identificadores e preparar uma mensagem de retorno antes de mostrar qualquer coisa. Por isso, não é correto avaliar o processo apenas pelo que aparece no final.

## Dados intermediários

Dados intermediários são dados criados, calculados, separados, classificados ou ajustados durante o processamento, antes da saída final. Eles não são necessariamente a entrada original nem a saída que será entregue ao usuário ou a outro processo. São passos de trabalho que ajudam o processamento a chegar ao resultado.

Em uma folha de pagamento, a entrada inclui cadastro do funcionário, salário base, eventos de horas, descontos, benefícios, dependentes, afastamentos e regras do período. Durante o processamento, podem surgir valores intermediários como salário proporcional, base de cálculo, total de descontos, total de benefícios, imposto estimado e valor líquido preliminar. A saída final pode ser pagamento, demonstrativo, arquivo para banco, registros contábeis e relatórios de conferência.

Em uma aprovação de crédito, as entradas podem ser dados cadastrais, renda, histórico, valor solicitado, prazo e relacionamento com a instituição. O processamento pode produzir pontuação, classificação de risco, limite sugerido, motivo de recusa ou necessidade de análise manual. Esses dados intermediários orientam a decisão, mas nem todos aparecem integralmente para o cliente.

Em um boleto, as entradas podem ser contrato, valor original, vencimento, descontos, juros, multa, dados do pagador e instruções de cobrança. O processamento pode calcular valor atualizado, identificar linha de cobrança, definir instruções de pagamento e registrar controle interno. A saída pode ser o boleto apresentado, arquivo de remessa, registro no sistema de cobrança e evidência para acompanhamento.

Em estoque, uma venda pode gerar dados intermediários como saldo reservado, saldo disponível, quantidade pendente, necessidade de reposição ou divergência de inventário. Em cobrança, um atraso pode gerar classificação de inadimplência, faixa de atraso, valor atualizado, estratégia de contato e status de negociação. Ignorar dados intermediários torna difícil explicar como o resultado foi alcançado.

## O que é saída

Saída é aquilo que atravessa a fronteira analisada ou representa resultado relevante. Pode ser dado, arquivo, mensagem, decisão, rejeição, registro, atualização de estado ou efeito operacional. Assim como entrada não é apenas digitação, saída não é apenas tela. A fronteira muda a classificação: arquivo é saída do cálculo, entrada do banco e parte de resultado para o processo organizacional.

Uma saída pode ser informação exibida em consulta, arquivo gerado, relatório, mensagem, registro atualizado, mudança de status, comprovante, alerta, lançamento contábil, resposta enviada a outro sistema, notificação, histórico, protocolo, evidência de auditoria ou dado preparado para outro processamento. Em alguns casos, a saída principal é uma atualização silenciosa: o usuário não vê grande mudança na tela, mas o estado de um contrato, pedido, pagamento ou cadastro foi alterado.

A saída precisa ser analisada pelo seu destino e pela sua finalidade. Uma mesma operação pode produzir várias saídas. Ao registrar um pagamento, o sistema pode atualizar saldo, baixar uma cobrança, gerar comprovante, alimentar extrato, enviar mensagem de confirmação, registrar histórico e criar evidência para auditoria. Cada saída atende a uma necessidade diferente.

Também é possível que uma saída seja apenas técnica e não seja útil para o negócio. Um arquivo pode ter sido gerado no formato esperado, mas conter registros incorretos. Uma mensagem pode ter sido enviada, mas não ser compreensível para quem precisa agir. Um relatório pode estar completo em colunas, mas não responder à pergunta da área responsável.

## Saída técnica e saída útil para o negócio

Saída técnica é o resultado produzido em uma forma que o sistema, a operação ou outra ferramenta consegue reconhecer. Pode ser um arquivo com estrutura correta, uma mensagem enviada, um registro gravado, uma resposta retornada ou um relatório gerado. Saída útil para o negócio é aquela que, além de existir tecnicamente, ajuda uma pessoa, área ou processo a cumprir uma finalidade.

Um relatório pode ser tecnicamente correto porque foi emitido sem falha e contém os campos previstos. Mesmo assim, pode não ser útil se não organiza os dados por período, mistura situações diferentes ou não mostra totais necessários para decisão. A existência do relatório não garante que ele apoie o trabalho.

Um arquivo pode respeitar o formato combinado, mas trazer conteúdo errado porque os filtros de entrada foram inadequados ou porque uma regra de seleção ignorou determinada situação. Tecnicamente, ele pode ser aceito pelo sistema que recebe. Organizacionalmente, pode gerar cobrança indevida, pagamento incorreto ou conciliação problemática.

Mensagens de sistema também mostram essa diferença. Uma mensagem muito técnica pode indicar o que aconteceu para uma equipe especializada, mas não orientar o usuário sobre a ação necessária. Uma resposta "operação rejeitada" pode ser verdadeira, porém insuficiente se não informa se o problema está no cadastro, no limite, no documento, na permissão ou no prazo.

Portanto, saída deve ser avaliada por correção técnica, significado, clareza, completude, destino e capacidade de apoiar decisão ou continuidade do processo.

## Entrada ruim, saída ruim

A expressão "entrada ruim, saída ruim" resume uma ideia importante: se os dados de entrada estão errados, incompletos, duplicados, fora de formato, fora de contexto ou interpretados de maneira inadequada, a saída pode ser errada mesmo que o sistema execute sem falha técnica. O processamento pode ser fiel às regras e ainda assim produzir resultado inadequado porque trabalhou sobre dados ruins.

Se um cadastro contém endereço errado, uma comunicação pode ser enviada ao local incorreto. Se uma data de admissão foi registrada com mês trocado, cálculos trabalhistas podem ser afetados. Se um pagamento aparece duplicado na entrada, a baixa de cobrança pode ficar inconsistente. Se um documento foi identificado como pertencente à pessoa errada, uma análise pode chegar a conclusão incorreta.

Entrada ruim não significa apenas erro de digitação. Pode haver entrada incompleta, como solicitação sem documento obrigatório. Pode haver entrada duplicada, como o mesmo pedido enviado duas vezes. Pode haver entrada em formato inadequado, como data interpretada com ordem diferente. Pode haver entrada fora de contexto, como usar tabela de preços de período errado. Pode haver entrada interpretada incorretamente, como tratar cancelamento como suspensão temporária.

Esse princípio não absolve processamento mal definido. Ele apenas mostra que boa parte da confiabilidade começa na qualidade, origem e validação das entradas.

## Validação de entrada

Validação de entrada é a verificação feita antes ou durante o processamento para avaliar se a entrada pode ser usada. Ela não serve apenas para evitar erro técnico. Serve para proteger o processo, melhorar a qualidade dos dados e impedir que resultados incorretos sejam produzidos a partir de informações inadequadas.

Uma validação pode verificar se dados obrigatórios foram informados, se o formato está correto, se o tamanho do campo é aceitável, se o tipo do valor corresponde ao esperado, se o valor está dentro de faixa permitida, se o código existe em um cadastro, se há compatibilidade entre campos, se a pessoa possui permissão, se a solicitação está duplicada, se as datas são coerentes e se uma regra de negócio permite a operação.

Em uma contratação, não basta receber nome e documento. Pode ser necessário validar cargo, faixa salarial, unidade, data de início, aprovação, orçamento e regra interna. Em uma venda, não basta receber produto e quantidade. Pode ser necessário validar estoque, preço vigente, endereço, forma de pagamento, limite de crédito e política comercial.

Validação não transforma uma entrada ruim em boa por mágica. Ela identifica, rejeita, alerta, corrige com controle ou encaminha para tratamento. Em alguns casos, impede o processamento; em outros, permite continuar com ressalva ou gera pendência. Validar entrada é parte essencial do fluxo.

## Processamento correto depende de mais que entrada correta

Embora entrada correta seja fundamental, ela não garante sozinha saída correta. O processamento também depende de regras adequadas, contexto correto, ambiente estável, dados de referência atualizados, integrações funcionando e interpretação correta da saída.

Uma entrada pode estar completa, mas a regra usada pode estar desatualizada. Um cálculo de benefício pode receber todos os dados necessários, mas aplicar alíquota antiga. Uma aprovação de crédito pode receber cadastro correto, mas consultar uma referência desatualizada. Uma cobrança pode ser gerada a partir de contrato correto, mas considerar calendário errado de vencimentos. Um relatório pode reunir dados corretos, mas ser interpretado como se tratasse de outro período.

O ambiente também influencia. Um processo pode depender de permissões, configurações, tabelas de referência, horários, disponibilidade de sistemas integrados e versões coerentes de componentes. Se uma integração não retornou informação necessária, o processamento pode ficar incompleto. Se uma tabela de preços não foi atualizada, o cálculo pode seguir regra antiga.

A saída ainda precisa chegar ao destino certo e ser compreendida corretamente. Um arquivo correto enviado ao lugar errado não cumpre sua finalidade. Uma mensagem correta ignorada por quem deveria agir pode produzir atraso. Um relatório correto lido sem conhecimento do contexto pode levar a decisão equivocada. Por isso, análise de qualidade exige olhar o fluxo inteiro.

## Saídas como novas entradas

Em sistemas organizacionais, a saída de um processo frequentemente se torna entrada de outro. Esse encadeamento é uma das razões pelas quais pequenas falhas podem se espalhar. Um resultado não termina necessariamente no momento em que é produzido; ele pode alimentar a próxima etapa.

Na folha de pagamento, a saída de cálculo pode se tornar entrada para geração de arquivo bancário. Esse arquivo pode orientar o pagamento dos funcionários. As mesmas informações podem alimentar contabilidade, obrigações fiscais, relatórios gerenciais e controles internos. Se o cálculo inicial estiver incorreto, vários processos posteriores serão afetados.

Em vendas, pedidos aprovados podem se tornar entrada para faturamento. O faturamento produz documentos, registros fiscais, atualização financeira e informações para entrega. Em cobrança, títulos gerados podem ser enviados a instituições financeiras, e o retorno bancário com pagamentos, rejeições ou ocorrências se torna nova entrada para baixa e conciliação.

Dados recebidos de governo podem se tornar entrada para controle interno de uma empresa ou instituição. Lançamentos contábeis gerados por sistemas operacionais podem se tornar entrada para fechamento contábil. Um status atualizado em atendimento pode se tornar entrada para logística, cobrança ou relacionamento com o cliente.

Essa cadeia de processamento exige cuidado. Quando uma saída vira entrada, ela precisa ser compreensível, consistente, completa e compatível com o próximo processo. Uma saída pobre pode apenas deslocar o problema para a etapa seguinte.

## Estado, feedback, ciclos e processamento parcial

EPS pode ocorrer em ciclos: entrada atualiza estado, produz saída, aguarda evento e volta a processar. Em sistemas interativos, resposta gera nova entrada; em sistemas orientados a eventos, pagamento recebido, arquivo disponibilizado ou prazo vencido pode iniciar novo tratamento; em fluxos contínuos, uma entrada e uma saída isoladas podem ser apenas recorte analítico. Diferentes atividades podem ocorrer simultaneamente ou intercaladas, o que pode afetar ordem e consistência; concorrência será aprofundada futuramente.

Saída técnica não é necessariamente resultado útil. Um arquivo pode ser gerado corretamente e enviado ao destino errado; parte dos itens pode ser processada antes de falha; reexecução pode duplicar efeito se contexto não for controlado. Rejeitados, registros intermediários e evidências são saídas importantes porque permitem encadeamento, conferência e retomada. Feedback não é só opinião: é retorno que influencia processamento posterior, como limite atualizado após transação ou fila de reprocessamento.

## Entrada, processamento e saída em processos manuais

O modelo também serve para processos manuais. Uma análise de pedido recebe dados do solicitante, descrição da necessidade, documentos de apoio e critérios internos. O processamento é a leitura, conferência, comparação com regras, consulta a responsáveis e decisão. A saída pode ser aprovação, recusa, pendência, encaminhamento ou solicitação de ajuste.

Na conferência de documentos, as entradas são formulários, cópias, comprovantes, datas, assinaturas e exigências. O processamento é verificar se tudo está completo, se os documentos pertencem à pessoa correta, se estão dentro do prazo e se atendem ao critério esperado. A saída pode ser "documentação aceita", "documentação pendente" ou "necessário complementar".

Um cálculo manual de comissão recebe vendas, percentuais, metas, cancelamentos, períodos e regras comerciais. O processamento envolve selecionar vendas válidas, aplicar percentuais, descontar cancelamentos e consolidar valores. A saída pode ser valor de comissão, relatório de conferência ou lista de divergências.

Na aprovação de cadastro, entradas podem incluir dados pessoais, documentos, comprovantes, referências e regras de aceitação. O processamento confere consistência, valida obrigatórios e classifica a situação. A saída pode ser cadastro aprovado, recusado ou enviado para análise adicional. Em uma triagem de atendimento, entradas são relato, categoria do problema, prioridade e histórico; o processamento classifica o caso e a saída define fila, orientação ou encaminhamento.

Observar processos manuais dessa forma ajuda a perceber que computação automatiza ou apoia fluxos que já possuem lógica. O computador não inventa sozinho a finalidade do processo; ele executa regras e manipula dados dentro de um contexto definido.

## Entrada, processamento e saída em sistemas corporativos

Em um banco, uma transferência pode receber como entradas conta de origem, conta de destino, valor, data, canal, autenticação e limites. O processamento valida identificação, confere saldo, verifica regras de limite, registra débito e crédito, atualiza extrato e cria histórico. As saídas podem ser comprovante, atualização de saldo, mensagem de confirmação, registro contábil e evidência para auditoria. A consequência organizacional é manter confiança sobre dinheiro, responsabilidade e rastreabilidade.

Em um órgão público, uma solicitação de benefício pode receber documentos, cadastro do cidadão, renda declarada, histórico, vínculos e data de solicitação. O processamento valida elegibilidade, confere documentos, consulta bases de referência, classifica situação e decide encaminhamento. As saídas podem ser deferimento, indeferimento, pedido de complemento, registro de decisão e relatório de acompanhamento. A consequência organizacional é atender direitos, controlar recursos e justificar decisões.

Em uma seguradora, um aviso de sinistro pode receber dados do segurado, apólice, ocorrência, laudos, fotos, boletins e valores estimados. O processamento verifica cobertura, vigência, franquia, relação com contrato, documentação e necessidade de vistoria. As saídas podem ser autorização de pagamento, recusa fundamentada, solicitação de documento, alteração de status e registro de reserva. A consequência organizacional é controlar risco, custo, atendimento e obrigação contratual.

No comércio, uma venda recebe produtos, quantidades, cliente, preço, promoção, estoque, forma de pagamento e endereço. O processamento valida disponibilidade, calcula total, aplica descontos, reserva estoque, autoriza pagamento e organiza entrega. As saídas podem ser pedido confirmado, nota, baixa de estoque, ordem de separação, comprovante e mensagem ao cliente. A consequência organizacional é transformar intenção de compra em operação registrada e atendida.

Na folha de pagamento, as entradas incluem cadastro de funcionários, salários, jornadas, horas, benefícios, descontos, afastamentos, impostos e eventos do período. O processamento calcula bases, proventos, descontos, líquido, encargos e consistências. As saídas podem ser demonstrativos, arquivos de pagamento, lançamentos contábeis, relatórios de conferência e evidências legais. A consequência organizacional é pagar corretamente e manter obrigações trabalhistas e financeiras.

Em cobrança, contratos em atraso, valores, vencimentos, pagamentos recebidos, política de juros, dados de contato e acordos anteriores funcionam como entradas. O processamento calcula valor atualizado, classifica atraso, define régua de contato, registra negociação e acompanha retorno bancário. As saídas podem ser aviso, boleto atualizado, baixa, renegociação, relatório de inadimplência e evidência de contato. A consequência organizacional é recuperar valores sem perder controle, histórico e conformidade.

## O modelo como ferramenta de análise

O modelo entrada, processamento e saída é uma ferramenta de análise porque orienta perguntas. Quando um resultado parece errado, a primeira pergunta não deve ser apenas "o sistema falhou?". É preciso reconstruir o fluxo.

Uma análise cuidadosa pergunta quais entradas foram usadas, de onde vieram, se estavam completas, se eram do período correto, se foram validadas e se havia duplicidade. Depois pergunta que dados de referência foram consultados, que regra foi aplicada, se a regra correspondia ao contexto e se houve exceção, rejeição ou pendência.

Depois, a análise observa a saída. A saída foi gerada? Foi gerada no formato correto? Continha os dados esperados? Foi enviada ao destino correto? Chegou no momento correto? Foi interpretada corretamente pela pessoa, área ou sistema que a recebeu? O resultado final apoiava a finalidade do processo?

Esse tipo de pergunta ajuda a separar causa e efeito. Um relatório incorreto pode ter origem em entrada incompleta, filtro errado, regra inadequada, dado de referência desatualizado, processamento interrompido, saída enviada incompleta ou interpretação equivocada. Sem o modelo, tudo parece um único problema. Com o modelo, a investigação ganha ordem.

## Relação com sistemas, dados, hardware, software e pessoas

Entrada, processamento e saída retomam os elementos estudados nas aulas anteriores. Pessoas fornecem entradas, interpretam saídas, definem regras, validam resultados e percebem problemas. Elas podem ser usuárias, analistas, operadores, gestores, clientes, atendentes ou responsáveis por conferência.

Software organiza o comportamento esperado: que campos receber, que validações aplicar, que cálculos fazer, que dados consultar, que status alterar e que saídas produzir. Hardware permite execução, armazenamento, leitura, gravação e transmissão. Sem software, o hardware não teria regra de negócio organizada para seguir.

Dados são a matéria-prima do fluxo. Podem aparecer como entrada, dados intermediários, dados de referência, dados de saída, histórico ou evidência. Sistemas organizam todos esses componentes dentro de fronteiras, interfaces, propósitos e relações com o ambiente. Tecnologia da informação coordena pessoas, processos, dados e tecnologia para produzir resultados úteis e controlados.

Essa relação mostra que o modelo cruza responsabilidade humana, regra de negócio, infraestrutura, qualidade de dados, comunicação entre áreas e finalidade organizacional.

## Conexão futura com programas

Na próxima etapa da formação, programa será apresentado como um conjunto organizado de instruções que orienta processamento. A conexão com esta aula é direta: um programa recebe alguma forma de entrada, executa instruções sobre dados e produz alguma saída.

Ainda não é necessário estudar sintaxe, linguagem ou código. O ponto preparatório é entender o papel do programa dentro do fluxo. Ele não é apenas um ícone, uma tela ou um nome no computador. Ele descreve comportamento esperado: que dados considerar, que validações aplicar, que cálculos executar, que decisões tomar e que resultados produzir.

Quando o aluno compreende entrada, processamento e saída, a ideia de programa deixa de parecer abstrata. Programa passa a ser uma forma de organizar a transformação. A Aula 07 aprofundará essa ideia sem exigir que o aluno escreva instruções.

## Conexão futura com Mainframe e COBOL

Em ambientes corporativos de grande porte, muitos sistemas lidam com grandes volumes de dados, regras estáveis, processos repetitivos, saídas controladas e forte necessidade de rastreabilidade. Mainframe e COBOL serão estudados mais adiante nesse contexto. Neste momento, a conexão deve permanecer conceitual.

Muitos programas corporativos recebem arquivos, registros, parâmetros ou solicitações; leem dados; validam condições; aplicam regras de negócio; atualizam informações; produzem relatórios, arquivos de saída, mensagens e evidências. Esse fluxo é uma aplicação direta do modelo entrada, processamento e saída.

O importante agora não é aprender uma linguagem nem uma técnica operacional. É perceber que tecnologias futuras serão mais fáceis de entender quando o aluno souber perguntar: quais dados entram, que processamento ocorre, que saídas são geradas, quem depende dessas saídas e que risco existe se alguma parte estiver errada.

## Confusões comuns de iniciantes

Uma confusão comum é pensar que entrada é apenas dado digitado. Digitação é uma forma de entrada, mas não é a única. Arquivos recebidos, mensagens de sistemas, eventos, comandos, documentos, dados armazenados, parâmetros e regras configuradas também podem orientar um processamento.

Outra confusão é tratar saída como sinônimo de tela. A tela é apenas um destino possível. Saída pode ser arquivo, relatório, mensagem, registro atualizado, mudança de status, comprovante, alerta, lançamento contábil, resposta a outro sistema ou evidência de auditoria.

Também é comum imaginar que processamento, por ser invisível, não precisa ser entendido. Em muitos sistemas, a parte mais importante acontece entre a entrada e a saída. Regras, validações, consultas, cálculos, classificações e decisões podem não aparecer diretamente para o usuário, mas explicam o resultado.

Outra interpretação equivocada é concluir que todo resultado errado significa programa errado. O programa pode estar errado, mas também pode ter recebido entrada incorreta, usado referência desatualizada, executado com contexto inadequado, enviado saída ao destino errado ou produzido mensagem interpretada de forma indevida.

Há quem ignore validação de entrada e trate qualquer dado recebido como se fosse confiável. Isso enfraquece o processo. Uma entrada precisa ser avaliada quanto a obrigatoriedade, formato, coerência, permissão, duplicidade, compatibilidade e regra de negócio antes de sustentar uma decisão.

Outra confusão é ignorar dados intermediários. O aluno vê apenas entrada inicial e saída final, mas não percebe valores calculados, classificações, bases, status temporários e registros auxiliares que explicam como a saída foi alcançada.

Também é frequente esquecer que a saída de um sistema pode ser entrada de outro. Uma informação produzida em uma etapa pode alimentar faturamento, cobrança, contabilidade, atendimento, auditoria ou integração. Se a saída está ruim, o problema pode se propagar.

Outra confusão é achar que relatório é automaticamente informação útil. Um relatório pode existir, estar formatado e ainda assim não responder à pergunta necessária. Saída útil exige contexto, clareza, completude e finalidade.

Há ainda a ideia de que, se o sistema gerou alguma coisa, o processo está correto. Um sistema pode gerar arquivo, mensagem ou relatório mesmo quando usou dados errados, regra inadequada ou contexto incorreto. Produzir saída não é o mesmo que produzir saída correta.

Por fim, muitos iniciantes analisam erro apenas pelo resultado final. O resultado é importante, mas não conta a história inteira. A análise precisa voltar às entradas, regras, dados de referência, execução do processamento, geração da saída, destino e interpretação.

## Perguntas para reflexão

- Em uma operação de cadastro, quais entradas são fornecidas por pessoas e quais podem vir de dados já existentes?
- Em uma cobrança, que dados intermediários podem existir antes da saída final enviada ao cliente?
- Por que uma saída tecnicamente gerada pode não ser útil para uma área de negócio?
- Quando um resultado está errado, que perguntas ajudam a investigar entrada, processamento e saída separadamente?
- Em que situações a saída de um processo pode virar entrada de outro?
- Que riscos aparecem quando uma entrada é aceita sem validação suficiente?

## Síntese da aula

O modelo entrada, processamento e saída é uma forma fundamental de observar operações e sistemas. Entrada é aquilo que chega ao processo ou está disponível para ser usado: dados digitados, arquivos, mensagens, documentos, eventos, comandos, parâmetros, regras, sinais ou registros armazenados. Processamento é o tratamento aplicado: validação, cálculo, comparação, classificação, consulta, decisão, atualização e preparação de resultados. Saída é aquilo que o processo produz: informação exibida, arquivo, relatório, mensagem, registro atualizado, status, comprovante, alerta, lançamento, resposta ou evidência.

Esse modelo ajuda a compreender sistemas computacionais, mas também se aplica a processos humanos e administrativos. Ele mostra que uma saída ruim pode nascer de entrada ruim, regra inadequada, contexto errado, referência desatualizada, integração falha, ambiente incorreto ou interpretação equivocada. Também mostra que saídas frequentemente alimentam novos processos, formando cadeias de dependência.

A aula prepara a compreensão futura de programas. Um programa será entendido como uma organização de instruções que recebe entradas, executa processamento e produz saídas. Também prepara a leitura futura de sistemas corporativos, Mainframe e COBOL, sem antecipar detalhes técnicos.

## Mini glossário da aula

**Entrada**: qualquer dado, documento, comando, evento, mensagem, parâmetro, regra ou sinal usado por um processo.

**Processamento**: tratamento aplicado às entradas por regras, instruções, operações, validações, cálculos ou decisões.

**Saída**: resultado produzido por um processo, podendo ser exibido, gravado, enviado, registrado ou usado por outra etapa.

**Dado de entrada**: dado recebido, recuperado ou disponibilizado para orientar um processamento.

**Dado intermediário**: dado criado ou ajustado durante o processamento antes da saída final.

**Dado de saída**: dado produzido como resultado de um processamento.

**Validação de entrada**: verificação feita para avaliar se uma entrada está completa, coerente, permitida e adequada ao processo.

**Regra de processamento**: critério que define como os dados devem ser tratados, calculados, comparados, aceitos, rejeitados ou transformados.

**Saída técnica**: resultado produzido em forma reconhecível pelo sistema ou operação, como arquivo, mensagem, registro ou resposta.

**Saída útil**: saída que atende uma finalidade de negócio, decisão, conferência, continuidade operacional ou responsabilidade.

**Cadeia de processamento**: sequência em que saídas de um processo se tornam entradas de outros processos.

**Interface**: ponto de contato pelo qual pessoas, sistemas ou processos trocam entradas e saídas.

**Relatório**: saída organizada para apresentar informações, totais, ocorrências, exceções ou evidências.

**Arquivo de saída**: arquivo produzido por um processamento para armazenamento, envio, integração, conferência ou uso posterior.

**Mensagem**: saída textual, técnica ou operacional enviada a pessoa, sistema ou componente para indicar resultado, aviso ou condição.

**Resposta**: retorno produzido por um sistema ou processo após receber uma solicitação.

**Evento**: ocorrência significativa que pode iniciar, orientar ou alterar um processamento.

**Parâmetro**: valor ou opção usado para orientar como um processamento deve ocorrer.

**Evidência**: registro que permite demonstrar que uma operação ocorreu, que regra foi aplicada ou que resultado foi produzido.

**Integração**: relação organizada entre sistemas ou processos que trocam entradas e saídas.

**Análise de erro**: investigação que busca identificar onde o fluxo falhou, considerando entrada, processamento, saída, contexto e interpretação.

## Referências e leituras para aprofundamento

- IBM. *Transaction processing terms and concepts*.
- IBM. *Mainframe workloads: Batch and online transaction processing*.
- National Institute of Standards and Technology. *Computer Security Resource Center Glossary: Transaction*.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir explicar o modelo entrada, processamento e saída sem reduzi-lo a teclado, computador e tela. Deve reconhecer entradas amplas, como arquivos, mensagens, documentos, eventos, comandos, parâmetros, regras e dados armazenados.

O aluno deve conseguir descrever o processamento como transformação orientada por regras, validações, cálculos, comparações, consultas, classificações e decisões. Também deve reconhecer que dados intermediários podem existir e que eles ajudam a explicar o resultado produzido.

O aluno deve diferenciar saída técnica de saída útil para o negócio, identificando que relatório, arquivo, mensagem ou registro gerado não garantem, por si só, valor operacional. Deve compreender que entrada ruim pode gerar saída ruim mesmo quando o sistema executa, e que processamento correto depende também de regra, contexto, ambiente, dados de referência, integração e interpretação.

Por fim, o aluno deve conseguir analisar uma situação simples perguntando quais entradas foram usadas, que processamento ocorreu, que saídas foram geradas, para onde foram enviadas e se foram compreendidas corretamente. Esse domínio prepara a próxima aula, na qual programa será estudado como organização de instruções para transformar entradas em saídas.
