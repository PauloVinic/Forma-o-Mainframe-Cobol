# Aula 07 — O que é um programa

## Objetivo da aula

O objetivo desta aula é construir uma compreensão precisa, mas acessível, do que é um programa e de como ele se relaciona com necessidade, requisito, especificação, algoritmo, código-fonte, software, sistema e processo em execução. Ao final, o aluno deve saber que esses termos se conectam, porém descrevem níveis ou perspectivas diferentes de um mesmo trabalho técnico.

Esta aula não ensina sintaxe nem pede escrita de código. Ela prepara o aluno para estudar código-fonte, compilação, interpretação, execução, arquivos, ambientes e erros. Antes de perguntar como escrever uma instrução, é necessário entender o que se espera de um sistema, qual método pode resolver uma parte do problema e o que muda quando uma descrição passa a ser executada em um ambiente real.

## O problema que esta aula resolve

É comum dizer que “o sistema precisa de um programa”, que “o algoritmo está errado” ou que “a tela não funciona” como se programa, sistema, algoritmo e interface fossem sinônimos. Esse modo de falar é compreensível na conversa cotidiana, mas deixa a análise técnica imprecisa. Quando um pagamento sai errado, é diferente descobrir que o requisito era ambíguo, que a especificação não tratava uma exceção, que o algoritmo escolheu regra inadequada, que o programa implementou o algoritmo incorretamente ou que o processo em execução usou arquivo errado.

A confusão também produz expectativa irreal sobre programação. Uma necessidade de negócio não se transforma diretamente em programa. Entre “precisamos calcular corretamente uma folha de pagamento” e uma execução real existem regras, requisitos, decisões de projeto, descrições de comportamento, algoritmos, código, testes, arquivos, ambientes e pessoas responsáveis por conferir o resultado.

Esta aula organiza essas palavras sem transformá-las em curso completo de engenharia de requisitos, algoritmos ou sistemas operacionais. A meta é dar ao iniciante uma linguagem de análise: saber perguntar o que a organização precisa, o que o sistema deve fazer, como isso foi especificado, que método foi escolhido, o que o programa efetivamente implementa e o que ocorreu quando ele foi executado.

## Introdução: o programa dentro de uma cadeia de decisões

Na Aula 02, sistema foi apresentado como conjunto de componentes relacionados. Nas Aulas 05 e 06, processamento foi descrito como transformação de entradas em saídas segundo regras. Agora o foco é uma parte importante dessa transformação: o programa. Um programa pode receber dados, comparar condições, calcular, validar, classificar, consultar, atualizar, produzir arquivo ou chamar outro componente. Mesmo assim, ele não explica sozinho o funcionamento de um sistema inteiro.

Considere uma folha de pagamento, que será o caso progressivo desta aula. A organização tem necessidade de pagar pessoas corretamente e cumprir obrigações. Essa necessidade não é um programa. Ela leva a objetivos, regras e requisitos: considerar eventos do período, aplicar descontos autorizados, preservar histórico e produzir saídas para banco, contabilidade e trabalhadores. A partir daí podem ser criadas especificações, escolhidos algoritmos e implementados programas. Quando um desses programas passa a funcionar em determinado ambiente, surge uma execução concreta, com dados, recursos e riscos próprios.

Separar essas camadas não é burocracia de vocabulário. É uma maneira de localizar problemas e responsabilidades. Se uma regra trabalhista mudou, talvez seja necessário rever requisito e especificação antes de alterar código. Se dois programas têm a mesma especificação, podem usar algoritmos ou estruturas diferentes. Se o programa está correto no arquivo armazenado, mas falha em produção, a investigação inclui o processo ativo e seu ambiente, não apenas a lógica escrita.

## O problema das palavras próximas

Os termos sistema, software, aplicativo, ferramenta, programa, algoritmo, código-fonte, processo, serviço e tela podem aparecer no mesmo cenário, mas não apontam para a mesma coisa. Uma tela é uma interface por meio da qual uma pessoa fornece entrada ou recebe saída. Um serviço pode ser componente que atende solicitações de outros componentes. Uma ferramenta é recurso usado para uma atividade. Um aplicativo costuma ser software percebido pelo usuário por sua finalidade. Um sistema inclui componentes técnicos e não técnicos organizados em torno de um propósito.

Programa e algoritmo também não são equivalentes. Um algoritmo é uma forma de descrever método ou estratégia para resolver uma classe de problemas. Um programa é uma descrição organizada, em forma que um ambiente computacional pode tratar, de instruções e estruturas que participam de um comportamento. O programa pode implementar algoritmos, mas também lida com entrada, saída, interação, tratamento de falhas, configuração e integração — elementos que não precisam ser todos descritos como algoritmos.

As fronteiras variam conforme o contexto. Uma equipe pode chamar de “programa” todo um executável distribuído; outra pode usar a palavra para cada módulo; em sistemas operacionais, processo tem sentido técnico ligado à execução; em engenharia de software, software pode incluir documentos e dados associados. O curso adotará definições operacionais consistentes, sem negar que outras áreas usem termos de maneira legítima e diferente.

## Necessidade, objetivo e requisito

Uma **necessidade** é um problema, oportunidade ou obrigação que motiva mudança ou operação. “A organização precisa calcular pagamentos do período” expressa necessidade. Um **objetivo** explicita resultado desejado, como pagar até determinada data com rastreabilidade. Esses enunciados orientam o trabalho, mas ainda não dizem com precisão como o sistema deve se comportar.

Um **requisito** descreve algo que um sistema, componente ou processo deve fazer, ou uma condição que deve respeitar. Pode dizer que o sistema deve calcular descontos conforme regra vigente, impedir pagamento duplicado, manter histórico de alteração ou gerar arquivo em formato acordado. Requisitos podem ser funcionais, quando descrevem capacidades ou comportamentos, e não funcionais, quando tratam propriedades ou restrições como segurança, desempenho, disponibilidade ou auditoria. Essa distinção será aprofundada em engenharia de software; aqui ela apenas evita confundir uma necessidade ampla com instruções de programa.

Uma **regra de negócio** expressa política, condição, cálculo, limite ou decisão ligada à atividade da organização. “Horas extras acima de certo limite exigem aprovação” pode ser regra de negócio. Ela pode originar requisitos e ser implementada por programas, mas não é automaticamente código. A regra precisa ter vigência, responsáveis, exceções e interpretação suficientemente claras para ser aplicada sem criar resultados arbitrários.

No caso da folha, “pagar corretamente” é necessidade. “Calcular salário líquido usando eventos aprovados no período” pode ser requisito. “Desconto de determinado benefício segue tabela vigente” é regra de negócio. Antes de implementar, ainda é necessário esclarecer quais eventos contam, como são tratados casos excepcionais, qual data define o período e que saídas comprovam o resultado.

## Especificação: comportamento esperado antes da implementação

Uma **especificação** descreve de maneira mais precisa comportamento, propriedades, entradas, saídas, restrições ou regras esperadas de um sistema ou componente. Pode ser texto estruturado, tabela de decisão, modelo, diagrama, contrato de interface, exemplos de casos ou notação formal. Pode existir antes de qualquer programa e pode ser independente da linguagem ou plataforma escolhida.

Por exemplo, uma especificação de cálculo de folha pode declarar entradas necessárias, condições de aceitação, ordem de aplicação de descontos, arredondamentos, saídas esperadas e tratamento de eventos inconsistentes. Ela não precisa dizer se a solução será COBOL, outra linguagem, uma regra configurada em ferramenta ou uma combinação de componentes. Seu papel é tornar expectativas examináveis e reduzir ambiguidades antes ou durante a implementação.

Algumas especificações podem ser formais, executáveis ou usadas para gerar parte de código. Isso não elimina a distinção conceitual. Mesmo quando uma ferramenta transforma modelo em artefato executável, ainda é útil separar “o que se espera” de “como determinado programa concreto realiza isso”. Uma especificação pode estar incompleta; um programa pode divergir dela; e dois programas podem implementar a mesma especificação de maneiras diferentes.

## Algoritmo: método, não sinônimo de programa

Um **algoritmo** é um método ou estratégia claramente definida para resolver uma classe de problemas. Uma definição técnica frequentemente enfatiza processo de cálculo especificado e resultado prescrito quando as regras são seguidas. Nesta fase, basta perceber que algoritmo descreve uma maneira de transformar entrada em resultado; não depende, em princípio, de linguagem de programação, hardware ou arquivo específico.

No caso da folha, um algoritmo pode descrever como percorrer eventos de um trabalhador, separar proventos e descontos, aplicar prioridades e calcular totais. A descrição pode estar em linguagem natural cuidadosa, pseudocódigo, fluxograma, tabela ou linguagem de programação. A implementação transforma uma escolha de algoritmo em elementos concretos de um programa, com tipos de dados, arquivos, módulos, bibliotecas, interfaces e tratamento de exceções.

Um programa pode conter vários algoritmos. Pode haver algoritmo de cálculo, outro de ordenação de registros e outro de detecção de duplicidade. Nem toda parte de um programa é melhor entendida como algoritmo: abrir conexão, registrar log, ler parâmetro, exibir mensagem ou coordenar componentes pode seguir protocolos e convenções que vão além de uma estratégia de resolução isolada.

O mesmo algoritmo pode aparecer em programas diferentes e programas diferentes podem atender a mesma necessidade com algoritmos distintos. Um sistema pode calcular totalizações lendo registros em sequência ou consultando dados agrupados por outro componente; as duas alternativas podem obedecer à mesma regra de negócio e ter consequências diferentes de desempenho, manutenção ou rastreabilidade. Análise formal de correção e eficiência será estudada adiante; por enquanto, o ponto é não chamar toda sequência de código de “o algoritmo” sem observar o problema que ela tenta resolver.

## Definição operacional de programa

Para esta formação, **programa** é uma descrição organizada de instruções, dados estruturados e mecanismos de controle, expressa em forma que pode ser traduzida, interpretada ou executada por ambiente computacional para participar de comportamentos definidos. A definição é operacional: ajuda a distinguir programa de necessidade, requisito e especificação, mas não pretende esgotar usos da palavra em todas as disciplinas.

“Organizada” indica que não é coleção aleatória de frases. Há estruturas que indicam ações, condições, repetição, dados, relações e ordem. “Em forma que pode ser tratada por ambiente” lembra que uma intenção humana vaga não basta: o ambiente precisa reconhecer a representação de acordo com regras da linguagem ou mecanismo usado. “Participar de comportamentos” evita sugerir que um arquivo isolado resolve por si só uma atividade organizacional; o efeito depende de execução, entradas, recursos, integrações e pessoas.

Programa não é a própria necessidade. Também não é automaticamente a especificação do comportamento. Ele é uma implementação concreta que procura realizar uma parte da especificação. Pode estar formalmente válido e ainda produzir resultado diferente do esperado porque requisito foi mal entendido, especificação era incompleta, algoritmo foi inadequado, regra mudou ou implementação contém defeito. Essa separação será essencial quando a formação estudar erros, testes e manutenção.

## Programa, dados, regras e processamento

Programas participam do processamento ao manipular representações de dados segundo instruções, regras e condições. Na folha de pagamento, o programa pode receber cadastro, eventos aprovados, tabelas vigentes, parâmetros de período e autorizações. Ele pode validar entradas, executar cálculos, registrar ocorrências e produzir demonstrativo, arquivo bancário ou relatório de conferência.

Entretanto, o programa não “descobre” por conta própria a regra correta. Pessoas e organizações definem políticas, requisitos e critérios. Se a regra está ambígua, se a tabela está desatualizada ou se uma exceção não foi especificada, o programa pode executar de modo previsível e ainda gerar consequência inadequada. Essa é uma razão para tratar necessidade, requisito, especificação, algoritmo e implementação como camadas relacionadas.

Também é importante separar comportamento esperado e comportamento observado. O comportamento esperado é descrito por requisitos e especificações: o que deveria ocorrer sob determinadas condições. O comportamento observado é o que de fato ocorreu em uma execução, com dados, versão, ambiente e recursos concretos. Comparar os dois ajuda a detectar defeitos, dados problemáticos, configurações inadequadas e falhas de operação.

Há uma consequência prática dessa distinção: um programa não transforma uma regra em verdade apenas porque a executa repetidamente. Suponha que uma tabela de desconto seja interpretada como percentual mensal quando o documento que a originou pretendia percentual anual. O programa pode aplicar a fórmula de maneira consistente a milhares de registros. O problema não estará necessariamente na escrita de cada instrução; pode estar na compreensão do requisito, na especificação da unidade, na tabela recebida ou na ausência de caso de teste que exponha a diferença.

Por isso, entradas e saídas precisam ser vistas como parte de um contrato de comportamento, ainda que o termo “contrato” seja aprofundado só mais adiante. Para calcular uma folha, não basta receber qualquer conjunto de valores. É preciso saber que período os eventos representam, quais códigos são aceitos, em que unidade os valores estão, que versão de tabela deve ser usada e o que o programa deve fazer quando encontra ausência ou contradição. Do lado da saída, não basta gerar um arquivo: é preciso saber se o destinatário espera determinado formato, se os totais conferem, se há registros rejeitados e que evidências permitem explicar o resultado.

Essa visão aproxima programação de responsabilidade. O programa é capaz de automatizar parte de uma atividade definida, mas não elimina a necessidade de pessoas interpretarem regras, aprovarem exceções, verificarem resultados e melhorarem o processo. Em sistemas corporativos, automatizar uma regra ambígua pode apenas tornar uma decisão inadequada mais rápida e mais difícil de perceber.

## Um caso progressivo: da folha ao programa em execução

Vale reorganizar o caso da folha em camadas, sem fingir que a realidade cabe em uma única sequência simples. A primeira camada é a necessidade: trabalhadores precisam receber valores corretos e a organização precisa cumprir obrigações, manter histórico e explicar seus cálculos. A necessidade define o problema geral, mas ainda permite muitas soluções e não informa diretamente uma máquina.

Na segunda camada aparecem requisitos. O sistema deve considerar eventos aprovados do período, impedir duplicidade de pagamento, aplicar tabelas vigentes, registrar exceções e gerar saídas para pessoas, banco e contabilidade. Alguns requisitos descrevem funções; outros estabelecem restrições, como proteção de dados pessoais, prazo de fechamento e rastreabilidade. Um requisito bem escrito reduz ambiguidades, mas pode continuar exigindo decisões de detalhamento.

Na terceira camada, a especificação torna certas decisões observáveis. Ela pode dizer que cada trabalhador terá um identificador, que eventos sem aprovação serão rejeitados ou sinalizados, que determinados descontos serão aplicados depois de determinadas parcelas e que valores devem obedecer a regra definida de arredondamento. Também pode apresentar exemplos: para entradas A, B e C, espera-se a saída D; para evento inconsistente, espera-se rejeição e registro de motivo. Esses exemplos ajudam a testar entendimento, mas não são ainda a implementação.

Na quarta camada, alguém escolhe algoritmos e estruturas de processamento. Um método pode percorrer eventos agrupados por trabalhador, separar categorias, acumular valores e aplicar regras em ordem determinada. Outro pode organizar os mesmos dados de maneira diferente, desde que preserve requisitos e resultados esperados. A escolha pode afetar desempenho, memória, facilidade de teste e clareza de manutenção. Esta aula não compara complexidade formal, mas já mostra que “há um cálculo” não determina automaticamente “há um único algoritmo”.

Na quinta camada surge o programa concreto. Ele organiza módulos, instruções, estruturas de dados e chamadas a componentes para realizar a implementação escolhida. Pode incluir partes de cálculo, leitura de arquivo, validação, emissão de mensagens e gravação de resultados. Pode usar bibliotecas ou serviços fornecidos por outros componentes. O programa não precisa conter todas as regras como texto fixo; algumas podem estar em tabelas, configurações ou serviços externos. Mesmo assim, a responsabilidade de entender como a regra chega ao comportamento continua existindo.

Na sexta camada, o código-fonte representa grande parte dessa implementação em linguagem de programação. Ele pode estar dividido em módulos e arquivos, e pode ser acompanhado de configurações, recursos e instruções de construção. A Aula 08 examinará por que essa representação precisa ser legível para pessoas e tratável por ferramentas. Por enquanto, a distinção basta: fonte é maneira de expressar e manter programa; não é sinônimo de toda a necessidade organizacional nem de execução em curso.

Por fim, quando a organização inicia o processamento mensal, uma forma preparada do programa é colocada para executar. O processo ativo recebe dados concretos, usa permissões e recursos do ambiente, lê determinada versão de tabela e produz saídas. O comportamento observado pode coincidir com a especificação, revelar dado inválido, expor defeito ou mostrar que uma regra precisa ser revista. O resultado encerra uma execução, não encerra a responsabilidade de conferir, explicar e aprender com ela.

## Limites da automação e da implementação

Programas são poderosos porque tornam certas operações repetíveis. Repetição, porém, não é sinônimo de correção nem de compreensão. Um programa pode aplicar uma regra de forma idêntica em todos os casos e ainda não lidar com exceção legítima. Pode processar entrada completa segundo seu formato e ainda receber valor que não representa a situação real. Pode produzir saída no prazo e ainda não fornecer informação suficiente para quem precisa tomar decisão.

Também não é correto imaginar que toda necessidade organizacional deve virar programa. Algumas decisões exigem julgamento humano, autorização, interpretação de documentos, negociação ou responsabilidade que não pode ser delegada integralmente a regras automatizadas. Sistemas podem apoiar essas atividades registrando informações, apresentando opções, aplicando controles ou encaminhando casos, sem substituir a decisão humana. A fronteira entre o que automatizar e o que revisar depende de risco, custo, regras, dados disponíveis e objetivos da organização.

Em manutenção, reconhecer esse limite evita alterações apressadas. Se alguém encontra condição aparentemente errada em um programa, ainda precisa perguntar: qual requisito ela implementa? Há exceção documentada? A tabela externa mudou? O comportamento observado é falha ou resultado esperado pouco compreendido? Alterar instrução sem investigar essas perguntas pode remover proteção importante ou criar divergência em outro processo.

## Programas como artefatos que evoluem

Programas não permanecem congelados depois de criados. Requisitos mudam, regras de negócio são atualizadas, dados ganham novos formatos, ambientes recebem versões diferentes e problemas observados exigem manutenção. Uma mudança pequena em uma instrução pode alterar comportamento de muitos registros; uma mudança de especificação pode exigir revisão de testes, tabelas, documentação e procedimentos operacionais.

Essa evolução reforça a diferença entre programa e sistema. Um programa pode mudar sem que toda a finalidade do sistema mude; uma nova regra de negócio pode exigir alterações em vários programas e atividades manuais; uma correção de ambiente pode resolver comportamento observado sem modificar o código-fonte. Rastrear versões, entradas, saídas e decisões torna possível entender o que mudou e por quê.

Na formação futura, versionamento, testes, manutenção e engenharia de software darão instrumentos técnicos para lidar com essa evolução. Nesta fase, o aluno deve guardar a ideia principal: programa é artefato concreto dentro de uma rede de decisões e componentes. Para analisá-lo com maturidade, é preciso perguntar tanto o que ele executa quanto o que deveria executar, sob quais condições e com quais consequências.

## Programa e código-fonte

Código-fonte será estudado com detalhe na próxima aula. Por enquanto, considere-o uma representação de programas em linguagem de programação, geralmente textual, legível por pessoas e tratável por ferramentas. O código-fonte não é sempre idêntico ao programa em todos os contextos. Um programa pode estar distribuído por vários arquivos, incluir código gerado, depender de bibliotecas e recursos, ser configurado por outros artefatos ou ser transformado em forma diferente antes de executar.

Em conversa cotidiana, é aceitável apontar para um arquivo-fonte e chamá-lo de programa. Para análise técnica inicial, convém perguntar: aquele arquivo contém parte do programa? É uma representação editável? Há outros módulos ou recursos? Qual artefato será efetivamente executado? Essa precisão prepara a diferença entre fonte, compilação, interpretação, executável e runtime que aparecerá na Aula 09.

## Programa, software, aplicação, ferramenta e sistema

**Software** é termo mais amplo que programa. Em várias definições de engenharia de software, pode abranger programas e também dados associados, configurações, documentação, recursos ou procedimentos necessários para uso e manutenção. A extensão exata varia com a fonte e o contexto. Para esta fase, basta usar software para conjunto de componentes lógicos destinados a oferecer comportamentos ou serviços, reconhecendo que um programa individual pode ser apenas uma parte dele.

Uma **aplicação** costuma ser software voltado a finalidade de uso percebida por usuários ou outras aplicações. Uma **ferramenta** é recurso usado para executar atividade, como editor ou gerador de relatório. Uma **tela** é interface: pode coletar entrada e apresentar saída, mas não é todo o programa nem todo o sistema. Pode haver programas sem tela, como rotinas batch, serviços e integrações; uma tela também pode acionar vários programas.

Um **sistema** é mais amplo ainda. Na Aula 02, foi descrito como conjunto de componentes relacionados com um propósito. Um sistema de folha pode envolver programas de cálculo, telas de cadastro, bancos de dados, arquivos, integrações bancárias, regras, responsáveis, procedimentos de conferência, permissões, infraestrutura e atendimento. O programa de cálculo é importante, mas não substitui dados corretos, regra vigente, ambiente autorizado ou operação responsável.

## Programa armazenado e processo em execução

Um programa preservado em armazenamento não está necessariamente fazendo algo. Pode ser arquivo-fonte, artefato preparado para execução, módulo, script ou outro componente guardado. A execução começa quando um ambiente computacional carrega ou conduz uma forma do programa, disponibiliza recursos e passa a realizar operações sobre dados e entradas.

**Processo** é uma abstração usada por sistemas operacionais para representar uma execução ativa de programa. Como modelo introdutório, um processo possui estado e recursos associados, por exemplo memória, identificador, permissões, arquivos abertos e informações sobre o ponto de execução. A mesma definição de programa pode originar várias execuções em momentos, usuários ou dados diferentes; por isso, programa e processo não são a mesma coisa.

Essa explicação será refinada em sistemas operacionais. Algumas plataformas usam modelos diferentes de isolamento, execução e serviço; processos podem criar threads e interagir com outros processos. Para esta aula, a distinção essencial é simples: o programa é uma descrição ou artefato disponível; o processo é uma execução concreta acompanhada pelo ambiente.

No caso da folha, o programa pode permanecer armazenado até o fechamento mensal. Quando a rotina é iniciada, surge execução com versão escolhida, dados de determinado período, parâmetros, arquivos de entrada e recursos do ambiente. Se ela for executada novamente para outro período ou por motivo de reprocessamento, a definição do programa pode ser a mesma, mas o processo e suas consequências serão outros.

## Programas invisíveis, serviços e integração

Nem todo programa aparece na tela de um usuário. Há rotinas que validam registros, geram arquivos, registram eventos, atualizam saldos, enviam mensagens, atendem solicitações de outros componentes ou executam em horário agendado. Em sistemas corporativos, o usuário pode perceber apenas comprovante ou relatório; o comportamento pode envolver muitos programas e serviços em cadeia.

Essa observação reforça a diferença entre programa e sistema. Uma falha em pagamento pode estar no programa de cálculo, em serviço que fornece tabela, no arquivo que traz eventos, na configuração do ambiente, na regra de negócio ou no procedimento que iniciou a execução. A análise responsável não escolhe culpado antes de distinguir essas camadas.

## Limites e variações terminológicas

As definições desta aula são instrumentos de estudo. Em programação, “programa” pode significar código ou aplicação completa. Em sistemas operacionais, o foco costuma ser a relação entre programa e processo. Em engenharia de software, requisitos, especificações e implementações recebem atenção separada. Em documentação de produtos, software pode incluir componentes que não aparecem ao usuário. Essas variações não significam que qualquer uso seja igualmente preciso em qualquer situação; significam que o contexto precisa ser declarado.

O curso adotará a convenção apresentada aqui para manter continuidade: necessidade e requisito expressam problema e obrigação; especificação descreve comportamento esperado; algoritmo descreve método; programa implementa parte dessa descrição em forma tratável por ambiente; código-fonte é uma representação, geralmente textual; software e sistema são conjuntos mais amplos; processo representa execução ativa. Quando uma aula futura precisar de nuance adicional, ela deverá declarar a ampliação em vez de contradizer silenciosamente essa base.

## Relação com aulas anteriores e posteriores

As aulas anteriores prepararam esta distinção. Dados representam entradas e estados; processamento transforma entradas segundo regras; entrada e saída ajudam a observar o que um programa recebe e produz. Não é necessário repetir esses modelos aqui: o novo ponto é separar a regra esperada da implementação concreta que a executa.

A Aula 08 aprofundará código-fonte como forma de representar programas. A Aula 09 explicará como diferentes tecnologias traduzem, interpretam ou executam essas representações. A Aula 10 mostrará arquivos como meios de preservar fonte, configurações, entradas e saídas. A Aula 11 tratará de ambientes e dependências. A Aula 12 usará a diferença entre comportamento esperado e observado para analisar erros, defeitos, falhas e operação.

## Conexão futura com Mainframe e COBOL

Em sistemas Mainframe e COBOL, uma necessidade corporativa pode atravessar regras de negócio, especificações, programas, arquivos, jobs, bancos de dados, controles de execução e conferência operacional. Um programa COBOL não é sinônimo de todo o processo de negócio nem de uma instrução de JCL que o executa. Cada elemento tem função própria e uma alteração precisa ser avaliada no nível correto.

Por exemplo, uma mudança em regra de cálculo pode exigir atualização de requisito e especificação antes de alterar o programa. A execução em batch pode criar processos que usam arquivos e parâmetros concretos. Um retorno aparentemente bem-sucedido não prova que a especificação foi atendida; resultados precisam ser comparados com dados, regras, relatórios e evidências. Essa visão prepara manutenção responsável sem antecipar prática de COBOL ou JCL.

## Confusões comuns de iniciantes

Uma confusão comum é chamar necessidade de programa. “Precisamos pagar funcionários corretamente” descreve objetivo, não instruções executáveis. Outra é chamar qualquer sequência de passos de algoritmo e supor que algoritmo e programa são iguais. Um algoritmo pode ser independente de linguagem; programa inclui decisões de implementação e pode conter elementos que não são um algoritmo isolado.

Também é comum tratar código-fonte como o programa inteiro. Código-fonte é representação importante, geralmente textual, mas programas podem envolver vários arquivos, artefatos e recursos. Software é mais amplo que programa, e sistema é mais amplo que software porque pode incluir pessoas, dados, processos e infraestrutura.

Por fim, muitos confundem programa armazenado com processo em execução. Um arquivo não está ativo apenas por existir. E um programa formalmente aceito por uma ferramenta pode ainda divergir do comportamento esperado por causa de especificação, dados, ambiente, regra ou implementação. Essa distinção evita concluir que “rodou” significa necessariamente “resolveu o problema”.

## Perguntas para reflexão

- Em uma folha de pagamento, qual diferença existe entre a necessidade de pagar corretamente e o programa que participa do cálculo?
- Como um requisito pode estar correto e uma especificação ainda deixar uma exceção sem resposta?
- Por que dois programas podem atender à mesma necessidade usando algoritmos diferentes?
- Em que sentido um programa pode conter mais de um algoritmo?
- Por que código-fonte não é obrigatoriamente todo o programa em um sistema real?
- Que componentes, além de programas, fazem parte de um sistema de folha?
- O que muda quando um programa armazenado gera duas execuções com dados de períodos diferentes?
- Como comportamento esperado e comportamento observado ajudam a investigar um pagamento incorreto?

## Síntese da aula

Programa é uma descrição organizada, em forma tratável por ambiente computacional, de instruções e estruturas que participam de comportamentos definidos. Não é necessidade, requisito, regra de negócio, especificação, algoritmo, código-fonte, software, sistema ou processo, embora se relacione com todos eles.

Necessidade e objetivo explicam por que algo importa. Requisito descreve obrigação ou condição. Especificação torna comportamento esperado mais preciso. Algoritmo descreve método para resolver problema. Programa é implementação concreta; código-fonte é uma de suas representações usuais. Software pode reunir programas e componentes associados; sistema abrange ainda pessoas, processos, dados e infraestrutura. Processo é abstração de execução ativa.

Essa separação ajuda a investigar diferenças entre o que deveria ocorrer e o que de fato ocorreu. Um programa pode estar sintaticamente válido, executar até o fim e ainda implementar regra inadequada ou usar contexto errado. A próxima aula aprofundará como código-fonte representa programas para pessoas e ferramentas.

## Mini glossário da aula

**Necessidade**: problema, oportunidade ou obrigação que motiva uma atividade ou mudança.

**Requisito**: capacidade que sistema ou componente deve fornecer, ou condição que deve respeitar.

**Regra de negócio**: política, cálculo, limite ou decisão ligada à atividade da organização.

**Especificação**: descrição de comportamento, propriedades, entradas, saídas ou restrições esperadas; pode ser independente da implementação.

**Algoritmo**: método ou estratégia claramente definida para resolver uma classe de problemas.

**Implementação**: realização concreta de uma especificação, algoritmo ou decisão de projeto em componentes executáveis ou utilizáveis.

**Programa**: descrição organizada, em forma tratável por ambiente computacional, de instruções e estruturas que participam de comportamentos definidos.

**Código-fonte**: representação de programa em linguagem de programação, geralmente textual, tratável por ferramentas e legível por pessoas.

**Software**: conjunto mais amplo de programas e componentes associados; a abrangência exata varia conforme a definição adotada.

**Sistema**: conjunto de componentes relacionados, técnicos e não técnicos, organizado para um propósito.

**Aplicação**: software voltado a uma finalidade de uso percebida por usuário ou outro sistema.

**Processo**: abstração de sistema operacional para uma execução ativa de programa, com estado e recursos associados.

**Execução**: atividade em que ambiente computacional conduz uma forma do programa sobre recursos, dados e entradas concretos.

**Comportamento esperado**: resultado ou propriedade descrita por requisito ou especificação.

**Comportamento observado**: resultado efetivamente verificado em uma execução concreta.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir distinguir necessidade, requisito, regra de negócio, especificação, algoritmo, programa, código-fonte, software, sistema, processo e execução em caso simples. Deve explicar que uma especificação pode existir antes da implementação e que algoritmo não é sinônimo de programa.

Deve reconhecer que um programa pode conter vários algoritmos, que programas distintos podem atender à mesma necessidade e que código-fonte é representação geralmente textual, não necessariamente o programa inteiro. Também deve diferenciar programa armazenado de processo em execução como modelo inicial de sistemas operacionais.

O aluno deve analisar o caso de folha de pagamento, apontando necessidade, requisitos, regras, especificação, algoritmo, programa, processo e sistema mais amplo. Deve explicar por que comportamento esperado pode diferir do observado e por que uma execução sem interrupção não prova, por si só, que a necessidade foi atendida corretamente.

## Referências e leituras para aprofundamento

- ISO/IEC/IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*.
- NIST. *Computer Security Resource Center Glossary: Algorithm*.
- ARPACI-DUSSEAU, Remzi H.; ARPACI-DUSSEAU, Andrea C. *Operating Systems: Three Easy Pieces*, capítulo sobre processos.
- ACM, IEEE Computer Society e AAAI. *Computer Science Curricula 2023*, áreas de Algorithmic Foundations, Foundations of Programming Languages e Software Development Fundamentals.
