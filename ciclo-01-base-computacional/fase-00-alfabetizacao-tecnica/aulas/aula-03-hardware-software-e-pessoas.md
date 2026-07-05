# Aula 03 — Hardware, software e pessoas

## Objetivo da aula

O objetivo desta aula é explicar como hardware, software e pessoas participam de sistemas computacionais e sistemas de informação. Ao final, o aluno deve conseguir ir além das definições curtas de que hardware é a parte física e software é a parte lógica, compreendendo que equipamentos fornecem recursos materiais, programas organizam instruções e comportamentos, e pessoas definem necessidades, executam processos, interpretam resultados, tratam exceções e mantêm a operação funcionando.

Esta aula também prepara a continuidade da Fase 0. Depois de entender tecnologia da informação como relação entre pessoas, processos, dados e tecnologia, e depois de estudar sistema como conjunto organizado de componentes relacionados, o próximo passo é observar alguns componentes centrais dos sistemas computacionais: a base material, a organização lógica e a participação humana.

## O problema que esta aula resolve

Muitos iniciantes decoram que hardware é a parte física do computador e software é a parte lógica. Essas frases ajudam como primeira aproximação, mas deixam várias perguntas sem resposta. Que parte física? Para que ela serve? Como o software usa essa parte física? Onde entram os dados? Quem define o que o software deve fazer? Quem opera, confere, corrige, autoriza e interpreta o resultado?

Quando essas perguntas não são feitas, o aluno pode imaginar que sistemas reais são apenas máquinas com programas instalados. Essa visão é insuficiente. Um sistema de folha de pagamento, uma operação bancária, um controle de estoque ou um atendimento público não dependem apenas de computador e tela. Dependem de regras de negócio, dados confiáveis, infraestrutura disponível, usuários treinados, operação acompanhada, suporte, manutenção e decisões humanas. Esta aula resolve a lacuna entre a definição decorada e o funcionamento real.

## Introdução

Na Aula 01, tecnologia da informação foi apresentada como uso organizado de recursos técnicos, pessoas, processos e métodos para lidar com informações. Na Aula 02, sistema foi explicado como conjunto de componentes relacionados que atuam com uma finalidade. Essas duas ideias precisam caminhar juntas: tecnologia da informação aparece por meio de sistemas, e sistemas só funcionam quando seus componentes se relacionam de forma coerente.

Agora, a fase passa a observar três elementos que aparecem em praticamente todo sistema computacional: hardware, software e pessoas. O hardware fornece recursos físicos para receber, armazenar, processar, transmitir e apresentar dados. O software organiza instruções, regras, formatos, permissões, cálculos e comportamentos esperados. As pessoas dão finalidade ao sistema, informam dados, definem regras, operam rotinas, analisam exceções, tomam decisões e mantêm a continuidade do trabalho.

Separar esses elementos ajuda a estudar, mas eles não existem isolados no uso real. Um servidor sem programa não calcula folha de pagamento. Um programa sem hardware não executa. Um sistema sem pessoas não sabe qual problema organizacional deve resolver nem como seus resultados serão interpretados. A compreensão inicial de computação começa quando o aluno percebe essa dependência mútua.

## A definição rasa de hardware e software não é suficiente

Dizer que hardware é a parte física e software é a parte lógica não está completamente errado. A frase indica uma distinção básica: existe aquilo que pode ser tocado, como equipamentos e dispositivos, e existe aquilo que organiza instruções e comportamento, como programas e sistemas. O problema é tratar essa frase como explicação final.

Hardware não é apenas "peça". Uma CPU, um disco, uma memória, um monitor, um leitor, uma placa de rede e um servidor não têm a mesma função. Cada componente participa de uma forma diferente da entrada, do armazenamento, do processamento, da comunicação ou da saída de dados. Se o aluno chama tudo apenas de parte física, perde a capacidade de entender por que uma falha de memória é diferente de uma falha de armazenamento, por que rede indisponível afeta acesso remoto ou por que um servidor precisa ser mais controlado que um equipamento doméstico.

Software também não é apenas "parte lógica" como se fosse uma ideia solta. Software existe para orientar recursos computacionais. Ele expressa instruções, regras, fluxos, validações, cálculos, permissões, formatos e integrações. Uma tela vista pelo usuário pode ser apenas a interface de uma cadeia maior de programas, serviços, bancos, arquivos e rotinas. Portanto, a definição curta serve como ponto de partida, mas não ensina como sistemas funcionam.

## Hardware como base material da computação

Hardware é o conjunto de componentes físicos usados para entrada, armazenamento, processamento, comunicação e saída de dados. Ele é a base material sobre a qual a computação acontece. Sem hardware, não há onde executar instruções, onde manter dados durante uma execução, onde preservar arquivos, nem por onde receber entradas ou apresentar resultados.

A CPU, ou unidade central de processamento, é o componente associado à execução de instruções e à coordenação de operações básicas. Em nível introdutório, ela pode ser entendida como a parte que realiza processamento conforme instruções fornecidas pelo software. Ela não trabalha sozinha: precisa acessar dados e instruções em memória, receber ou enviar informações para dispositivos e depender do sistema operacional para organizar recursos.

Memória é o recurso usado para manter dados e instruções acessíveis durante a execução. Ela é diferente do armazenamento persistente. A memória costuma ser mais rápida e temporária; o armazenamento preserva arquivos e dados para uso posterior. Um cadastro salvo, um relatório gerado, uma configuração e um arquivo de entrada precisam estar em algum meio de armazenamento, como discos, unidades de estado sólido ou estruturas equivalentes em servidores.

Dispositivos de entrada permitem fornecer dados ou comandos ao sistema. Teclado, leitor de código, scanner, sensor, tela sensível ao toque e arquivos recebidos podem servir como origem de entrada. Dispositivos de saída apresentam ou enviam resultados, como monitor, impressora, arquivo gerado, mensagem transmitida ou relatório produzido. Rede permite comunicação entre equipamentos e sistemas, tornando possível acessar servidores, integrar áreas, transmitir arquivos e usar serviços remotos.

Periféricos são equipamentos auxiliares conectados a um computador ou ambiente, como impressoras, leitores, equipamentos de autenticação e dispositivos de captura. Servidores são equipamentos ou ambientes preparados para oferecer recursos a vários usuários, aplicações ou sistemas, geralmente com maior controle de disponibilidade, segurança e armazenamento. Terminais são meios de acesso a sistemas, especialmente quando a execução principal ocorre em outro ambiente. Dispositivos móveis, como celulares e tablets, também são hardware, mas normalmente funcionam como canais de acesso e coleta de dados, não como o centro de todos os processos corporativos.

Esta aula não aprofunda arquitetura de computadores. O ponto necessário agora é entender que hardware fornece capacidades concretas e limitadas. Software não executa no vazio; ele precisa de processamento, memória, armazenamento, comunicação e dispositivos para interagir com o mundo.

## Software como instrução, regra e comportamento

Software é o conjunto organizado de instruções, regras, estruturas e componentes lógicos que orientam o hardware a executar tarefas. Ele define o que deve acontecer quando um dado é recebido, quando uma opção é selecionada, quando uma regra é satisfeita, quando uma validação falha ou quando uma saída precisa ser produzida.

Software não é algo mágico e também não é apenas a tela que aparece ao usuário. A tela pode apresentar campos, botões e mensagens, mas por trás dela pode haver validações de formato, consulta a cadastro, verificação de permissão, cálculo de valores, comunicação com outro sistema, gravação em banco de dados, geração de log e atualização de histórico. O comportamento visível é apenas uma parte da organização lógica.

O sistema operacional é um tipo de software responsável por gerenciar recursos computacionais e oferecer condições para que programas sejam executados. Ele controla processos, memória, arquivos, dispositivos, usuários e permissões em nível apropriado ao ambiente. Aplicativo é um software voltado a uma finalidade de uso, como atendimento, edição, consulta, venda ou comunicação. Programa é uma unidade organizada de instruções, que pode fazer parte de uma aplicação maior ou executar uma tarefa específica.

Um sistema corporativo costuma reunir vários softwares: interfaces para usuários, programas de validação, serviços de integração, bancos de dados, rotinas de processamento, utilitários de administração e mecanismos de segurança. Banco de dados, neste nível introdutório, pode ser entendido como software destinado a organizar, armazenar, consultar e controlar dados. Utilitários são softwares que apoiam tarefas técnicas ou operacionais, como cópia, conferência, compactação, monitoramento ou organização de recursos. Ferramentas de desenvolvimento são softwares usados por profissionais para criar, alterar, verificar ou acompanhar outros softwares, mas esta fase ainda não entra em programação.

## A dependência entre hardware e software

Software precisa de hardware para executar. Uma instrução só produz efeito quando existe um ambiente físico capaz de processá-la, manter dados em memória, buscar informações no armazenamento e enviar saídas por algum dispositivo ou rede. Um programa guardado em um arquivo não está agindo por si só. Ele precisa ser colocado em execução em um ambiente computacional.

Hardware, por sua vez, precisa de software para realizar tarefas úteis. Um servidor ligado, com processadores, memória e armazenamento, não sabe sozinho calcular salários, validar documentos ou emitir boletos. Ele fornece capacidade. O software organiza essa capacidade em comportamento esperado. A relação entre os dois é parecida com a diferença entre ter recursos disponíveis e ter uma forma de usá-los para uma finalidade.

Em uma empresa, um sistema de cobrança pode executar em servidores, acessar armazenamento, usar rede para integração bancária e enviar saídas aos usuários. Mas a cobrança só acontece porque softwares aplicam regras de vencimento, calculam valores, identificam clientes, geram registros e produzem relatórios. Se o hardware falha, o software pode não executar. Se o software está incorreto, o hardware pode executar rapidamente uma regra errada. A qualidade do sistema depende da relação entre ambos.

## Pessoas como parte do sistema

Pessoas não são elementos externos irrelevantes. Em sistemas de informação, elas definem objetivos, descrevem necessidades, criam e interpretam regras, inserem dados, conferem resultados, autorizam exceções, tomam decisões, corrigem problemas e mantêm o funcionamento organizacional. Um sistema usado por pessoas precisa considerar linguagem, responsabilidade, treinamento, acesso, rotina real e consequências das decisões.

O usuário final utiliza o sistema para executar uma tarefa, consultar informação ou registrar dados. Ele pode ser atendente, analista de uma área, cliente, servidor público, vendedor ou gestor. O operador acompanha ou executa rotinas planejadas, como processamentos, verificações, liberações ou procedimentos de produção. Em ambientes corporativos, operação não significa uso casual; significa conduzir atividades necessárias para que sistemas e processos aconteçam no momento correto.

O analista de negócio entende regras, necessidades, exceções e objetivos da área que será atendida. Ele ajuda a traduzir o processo real em requisitos compreensíveis. O analista de sistemas observa a relação entre necessidade, dados, regras, integração, software e ambiente, buscando uma solução técnica coerente. O desenvolvedor transforma parte dessa solução em programas, serviços, ajustes ou componentes de software, sempre dependendo de regras, dados e contexto.

O administrador de infraestrutura cuida de recursos como servidores, rede, armazenamento, permissões técnicas, disponibilidade e capacidade. O administrador de banco de dados cuida de estruturas de dados, acessos, integridade, desempenho, recuperação e organização de bases. O gestor responde por prioridades, riscos, decisões de negócio, recursos e impactos organizacionais. O auditor verifica se ações, dados e controles podem ser demonstrados e se regras foram respeitadas.

A equipe de suporte atende dúvidas, registra incidentes, orienta usuários e aciona áreas responsáveis quando o problema exige investigação técnica. A equipe de operação monitora execuções, acompanha rotinas, observa alertas, verifica resultados e segue procedimentos para tratar falhas. Cada papel tem responsabilidade diferente. Confundir todos como "usuários" ou "pessoal de TI" impede entender como sistemas reais são mantidos.

## Pessoas, processos, dados, hardware e software

Um sistema de informação não é formado apenas por computador e programa. Ele envolve pessoas que executam processos, dados que representam fatos, software que organiza regras e hardware que permite execução, armazenamento e comunicação. A Aula 01 apresentou essa relação no contexto da tecnologia da informação. A Aula 02 mostrou que sistema é conjunto de componentes relacionados. Agora, esses componentes começam a ganhar forma.

Pessoas definem e executam processos. Processos indicam etapas, responsáveis, decisões e resultados esperados. Dados registram fatos relevantes desses processos, como cliente, produto, documento, valor, data, situação e autorização. Software aplica regras sobre esses dados e conduz fluxos de validação, cálculo, consulta ou registro. Hardware fornece os recursos para que tudo isso seja executado, preservado e transmitido.

Quando esses elementos estão alinhados, o sistema tende a ser mais compreensível e confiável. Quando estão desalinhados, surgem problemas: dados sem significado, telas que não refletem o processo real, regras mal entendidas, usuários sobrecarregados, infraestrutura insuficiente ou resultados difíceis de interpretar.

## Quando a tecnologia ignora pessoas

Sistemas falham quando são desenhados considerando apenas a ferramenta e ignorando usuários, processos reais, exceções, treinamento, operação e contexto organizacional. Um sistema de atendimento, por exemplo, pode exigir que o atendente informe dados que ele não possui no momento da ligação. A tela pode estar tecnicamente correta, os campos podem existir e o banco pode gravar tudo, mas o processo trava porque a informação exigida não está disponível na realidade do atendimento.

Em um sistema bancário, uma operação pode ser tecnicamente aceita, mas incompatível com uma regra de negócio. Imagine uma alteração cadastral permitida pela tela sem considerar que determinado tipo de conta exige aprovação adicional. O software recebeu dados válidos e o hardware executou a operação, mas a organização produziu um risco porque a regra humana e normativa não foi adequadamente representada.

Um sistema governamental pode coletar informações de cidadãos sem orientar claramente o preenchimento. O cidadão informa dados em campos ambíguos, envia documentação incompleta ou interpreta uma pergunta de forma diferente da esperada. Depois, a área interna precisa corrigir, pedir complementação ou negar solicitações. O problema não é apenas técnico; envolve linguagem, processo, contexto e responsabilidade pública.

Também ocorre falha quando uma empresa muda uma rotina interna sem treinar os usuários. O sistema passa a exigir nova classificação, novo fluxo de aprovação ou novo campo obrigatório, mas as pessoas não entendem a finalidade da mudança. O resultado pode ser preenchimento improvisado, aumento de chamados, atrasos e dados pouco confiáveis. Outro exemplo é o relatório tecnicamente correto, mas incompreensível para quem decide. Se a saída não comunica significado, o sistema produziu dados organizados, mas não apoiou a decisão.

## Hardware, software e pessoas em uma empresa

Em uma folha de pagamento, o processo começa com dados de funcionários, cargos, jornadas, eventos, benefícios, descontos e regras legais ou internas. Pessoas registram admissões, informam eventos, conferem exceções e autorizam mudanças. O software aplica cálculos, valida dados, gera valores, registra histórico e produz relatórios. O hardware sustenta armazenamento, processamento e saída dos resultados. A consequência de alinhamento é pagamento correto e rastreável; a consequência de falha pode ser salário incorreto, obrigação legal afetada ou divergência contábil.

Na abertura de conta, o começo está na solicitação do cliente e na coleta de documentos e dados cadastrais. O fluxo envolve identificação, validações, análise de risco, aceite de condições, aprovação e criação de registros. Pessoas participam como cliente, atendente, analista, gestor de regra, suporte e auditoria. O software organiza validações e registra decisões; o hardware permite captura, consulta e armazenamento. A consequência esperada é uma conta criada com dados confiáveis e permissões adequadas. Se uma etapa falha, pode haver recusa indevida, fraude, retrabalho ou registro incorreto.

Em uma venda no comércio, o começo pode ser a escolha do produto pelo cliente. O fluxo envolve consulta de preço, verificação de estoque, registro dos itens, cálculo de descontos, pagamento, emissão de documento e atualização de estoque. Pessoas atendem, conferem, autorizam exceções e resolvem problemas. O software aplica regras comerciais, fiscais e de estoque. O hardware inclui terminais de venda, leitores, impressoras, servidores, rede e dispositivos de pagamento. A consequência de bom funcionamento é venda registrada, estoque atualizado e documento emitido; a consequência de falha pode ser cobrança errada, produto vendido sem estoque ou informação fiscal incorreta.

Na concessão de benefício público, o começo está na solicitação do cidadão. O fluxo envolve coleta de dados, documentação, análise de critérios, decisão, comunicação, pagamento e registro para auditoria. Pessoas interpretam regras, verificam exceções e respondem por decisões. O software ajuda a organizar etapas, validar critérios e preservar histórico. O hardware sustenta atendimento, processamento, armazenamento e consulta. A consequência correta é uma decisão explicável; a falha pode afetar direito, prazo, orçamento e confiança institucional.

## Hardware e software em sistemas corporativos

Sistemas corporativos exigem infraestrutura mais robusta que aplicações simples porque sustentam processos com impacto operacional. Servidores precisam estar dimensionados para atender usuários, integrações e rotinas de processamento. Armazenamento precisa ser confiável porque dados corporativos devem sobreviver ao encerramento de execuções, falhas pontuais e consultas futuras. Controle de acesso é necessário porque nem toda pessoa pode consultar, alterar, aprovar ou excluir qualquer informação.

Backups existem para permitir recuperação quando há perda, corrupção ou falha grave. Logs registram eventos, acessos, erros e execuções, criando base para suporte, auditoria e diagnóstico. Disponibilidade indica que o sistema precisa estar acessível quando a operação depende dele; em muitos ambientes, ficar indisponível por pouco tempo já afeta atendimento, pagamento, venda ou fechamento.

Segurança protege dados, operações e recursos contra uso indevido. Desempenho importa porque um sistema correto, mas lento demais para a rotina, prejudica o processo. Integração é necessária porque cadastro, financeiro, estoque, atendimento, cobrança e relatórios costumam depender uns dos outros. Manutenção preserva e evolui o sistema ao longo do tempo, corrigindo problemas e adaptando regras. Operação e monitoramento acompanham execuções, alertas, recursos e resultados para que falhas sejam percebidas e tratadas antes de se espalharem.

Esses elementos mostram que hardware e software corporativos não devem ser vistos apenas como "computador e programa". Eles formam um ambiente controlado, com responsabilidades, evidências e dependências.

## O papel dos dados nessa relação

Hardware, software e pessoas existem, em sistemas de informação, em torno do tratamento de dados e informação. Pessoas ou outros sistemas fornecem entradas. O hardware permite capturar, transmitir, guardar e processar essas entradas. O software organiza o que deve ser feito com elas. O resultado é interpretado por usuários, gestores, auditores, processos automáticos ou outras partes da organização.

Dados podem representar clientes, contas, produtos, benefícios, pagamentos, eventos, autorizações e estados de um processo. Se os dados são incorretos, incompletos ou ambíguos, o software pode aplicar regras sobre uma base ruim e o hardware pode preservar resultados igualmente ruins. Por isso, dados conectam a parte técnica com a finalidade organizacional.

A próxima aula tratará com mais cuidado da diferença entre dados, informação e conhecimento. Por enquanto, basta perceber que hardware, software e pessoas não são estudados por si mesmos: eles participam do ciclo de entrada, registro, processamento, saída, interpretação e decisão.

## Conexão futura com Mainframe e COBOL

Mainframe será estudado futuramente como uma plataforma computacional voltada a necessidades corporativas de processamento, continuidade, segurança, armazenamento, integração e operação. Em vez de ser visto apenas como uma máquina grande, ele deverá ser compreendido como ambiente composto por hardware, sistema operacional, recursos de armazenamento, mecanismos de execução, controles de acesso, rotinas operacionais e integração com outros sistemas.

COBOL será estudado futuramente como uma linguagem usada para expressar regras de negócio, processar dados, manipular arquivos, participar de rotinas corporativas e integrar sistemas em contextos específicos. Nesta fase, não é necessário aprender detalhes da linguagem nem do ambiente mainframe. A conexão importante é conceitual: Mainframe e COBOL fazem parte da relação entre hardware, software, dados, processos e pessoas.

Quando o aluno encontrar programas, arquivos, rotinas, permissões, operadores e relatórios em fases posteriores, não deverá olhar para esses elementos como peças soltas. Eles estarão dentro de sistemas que existem para sustentar processos reais.

## Confusões comuns de iniciantes

Uma confusão comum é achar que hardware é apenas "peça de computador". Essa visão não mostra função. CPU, memória, armazenamento, rede, periféricos, servidores e terminais participam de formas diferentes do funcionamento de um sistema. Entender hardware exige perguntar que recurso físico está sendo usado e para qual finalidade.

Outra confusão é achar que software é apenas "programa com tela". Muitos softwares não aparecem diretamente ao usuário final. Serviços, bancos de dados, utilitários, rotinas internas, sistemas operacionais e componentes de integração podem funcionar sem uma tela principal. A tela é apenas uma forma de interação.

Também é comum achar que sistema é igual a software. A Aula 02 já mostrou que sistema envolve componentes relacionados e propósito. Software pode ser componente de um sistema, mas o sistema real também inclui dados, usuários, permissões, processos, infraestrutura, operação e manutenção.

Muitos iniciantes ignoram o papel dos usuários. Quando isso acontece, qualquer dificuldade de uso parece falta de atenção da pessoa. Na realidade, um sistema pode induzir erro se a tela é ambígua, se o processo é contraditório, se o treinamento foi insuficiente ou se os dados exigidos não estão disponíveis no momento correto.

Outra confusão é imaginar que tecnologia resolve problemas sozinha. Comprar equipamentos, instalar software ou criar uma tela não corrige processo mal definido, regra contraditória ou dado sem qualidade. Tecnologia ajuda quando está integrada a uma forma de trabalho.

Há também a confusão entre usar ferramenta e compreender sistema. Uma pessoa pode saber clicar nas opções de uma aplicação e ainda não entender que dados são alterados, que regras são aplicadas, que permissões existem ou que impactos surgem depois da operação.

Alguns iniciantes acham que todo erro é culpa do usuário. Outros acham que todo erro é culpa do programa. As duas respostas são apressadas. Falhas podem nascer de dados incorretos, regra mal definida, infraestrutura indisponível, permissão inadequada, integração falha, procedimento operacional ou software com comportamento errado.

Também é frequente ignorar infraestrutura, operação e manutenção. Sistemas corporativos precisam de ambiente, recursos, monitoramento, suporte, atualização, controle e recuperação. Um sistema não termina quando uma versão é entregue; ele continua existindo enquanto sustenta processos e precisa ser cuidado ao longo do tempo.

## Perguntas para reflexão

- Em um sistema de atendimento, que partes pertencem ao hardware, ao software e ao trabalho humano?
- Por que uma definição curta de hardware e software não basta para analisar uma falha real?
- Que papéis humanos participam de um sistema de folha de pagamento além do usuário que abre uma tela?
- Como uma regra de negócio mal compreendida pode gerar erro mesmo quando o software executa sem falha aparente?
- Que dados uma venda no comércio precisa registrar para que estoque, cobrança e relatório façam sentido?
- Por que servidores, backups, logs e monitoramento importam em sistemas corporativos?
- Em que situações um relatório tecnicamente correto pode não apoiar uma decisão?
- Como esta aula prepara a distinção futura entre dados, informação e conhecimento?

## Síntese da aula

Hardware, software e pessoas são componentes centrais de sistemas computacionais e sistemas de informação. Hardware fornece a base material: processamento, memória, armazenamento, entrada, saída e comunicação. Software organiza instruções, regras, estruturas e comportamentos esperados. Pessoas dão finalidade ao sistema, definem necessidades, operam rotinas, registram dados, interpretam resultados, tratam exceções, prestam suporte, mantêm infraestrutura e tomam decisões.

A ideia principal é que nenhum desses elementos resolve sozinho um problema organizacional. Hardware sem software é capacidade sem comportamento definido. Software sem hardware não executa. Tecnologia sem pessoas, processos e dados bem compreendidos produz sistemas frágeis, difíceis de usar, difíceis de manter ou incapazes de gerar informação útil.

Esta aula também reforçou a noção de sistema estudada anteriormente. Em sistemas reais, partes se relacionam: dados entram, softwares aplicam regras, hardwares executam e armazenam, pessoas conferem e decidem, processos orientam etapas e a organização lida com consequências. A próxima aula aprofundará o elemento que circula por essa relação: dados, informação e conhecimento.

## Mini glossário da aula

**Hardware**: conjunto de componentes físicos usados para entrada, processamento, armazenamento, comunicação e saída de dados.

**Software**: conjunto organizado de instruções, regras e componentes lógicos que orientam recursos computacionais a executar tarefas.

**CPU**: unidade central de processamento, responsável por executar instruções e coordenar operações básicas durante a execução.

**Memória**: recurso usado para manter dados e instruções acessíveis enquanto uma execução está acontecendo.

**Armazenamento**: recurso usado para preservar dados, arquivos, programas e resultados para uso posterior.

**Dispositivo de entrada**: componente ou meio pelo qual dados e comandos chegam ao sistema, como teclado, leitor, sensor ou arquivo recebido.

**Dispositivo de saída**: componente ou meio pelo qual resultados são apresentados ou enviados, como tela, impressora, arquivo, mensagem ou relatório.

**Servidor**: equipamento ou ambiente preparado para fornecer recursos, dados ou serviços a usuários, aplicações ou outros sistemas.

**Terminal**: meio de acesso usado para interagir com um sistema, enviando entradas e recebendo saídas.

**Sistema operacional**: software que gerencia recursos computacionais e cria condições para execução de programas.

**Aplicativo**: software voltado a uma finalidade de uso percebida por usuários ou áreas de trabalho.

**Programa**: conjunto organizado de instruções criado para orientar algum processamento.

**Usuário**: pessoa que utiliza um sistema para registrar dados, consultar informação ou executar uma tarefa.

**Operador**: pessoa ou equipe que conduz rotinas, acompanha execuções e segue procedimentos de operação.

**Desenvolvedor**: profissional que constrói, altera ou mantém componentes de software conforme regras, dados e necessidades definidas.

**Analista**: profissional que interpreta necessidades, regras, processos e impactos para orientar solução de negócio ou solução técnica.

**Infraestrutura**: conjunto de recursos técnicos que sustenta sistemas, como servidores, rede, armazenamento, permissões e ambientes.

**Operação**: execução organizada das atividades necessárias para manter sistemas e processos funcionando no uso real.

**Manutenção**: atividade de corrigir, adaptar, melhorar ou preservar sistemas ao longo do tempo.

**Suporte**: atividade de atendimento, orientação, registro de incidentes e encaminhamento de problemas relacionados a sistemas.

**Dado**: valor registrado, recebido ou armazenado que representa algum fato, evento, característica ou estado.

**Processo**: sequência organizada de atividades executadas para produzir um resultado.

**Regra de negócio**: condição, cálculo, restrição ou decisão que expressa uma necessidade da organização.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir explicar hardware sem limitar a resposta a "parte física" e software sem limitar a resposta a "parte lógica". Deve diferenciar hardware, software, sistema e ferramenta, mostrando que cada termo descreve uma função diferente dentro de uma solução.

Também deve explicar por que pessoas fazem parte dos sistemas de informação, identificando papéis como usuário, operador, analista, desenvolvedor, administrador, gestor, auditor, suporte e operação. O aluno deve compreender a dependência entre hardware e software, além de conectar hardware, software, pessoas, dados e processos em exemplos corporativos simples.

Por fim, deve conseguir explicar por que sistemas corporativos exigem infraestrutura, operação, monitoramento, logs, backups, segurança, manutenção e suporte. O domínio esperado inclui perceber que Mainframe e COBOL serão estudados futuramente dentro dessa relação entre plataforma, software, dados, regras de negócio, processos e pessoas.
