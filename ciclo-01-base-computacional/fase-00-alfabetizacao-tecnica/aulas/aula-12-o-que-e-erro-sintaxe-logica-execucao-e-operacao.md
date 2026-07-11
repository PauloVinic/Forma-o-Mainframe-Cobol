# Aula 12 — O que é erro: sintaxe, lógica, execução e operação

## Objetivo da aula

O objetivo desta aula é construir uma compreensão inicial, mas rigorosa, sobre erros em tecnologia e sistemas. Ao final, o aluno deve conseguir explicar por que a frase “deu erro” é tecnicamente insuficiente, diferenciar erro de sintaxe, erro lógico, erro de execução e erro operacional, reconhecer erro de ambiente, erro de dado e erro de regra de negócio, e analisar problemas considerando entrada, processamento, saída, arquivos, ambientes, permissões, configurações, regras e operação.

Esta aula encerra o conjunto conceitual das 12 aulas da Fase 0. Ela não ensina programação, COBOL, JCL, comandos ou prática de ferramenta. Seu papel é preparar o aluno para pensar melhor quando algo não ocorre como esperado. Antes de escrever código, instalar ferramentas ou operar sistemas críticos, é necessário saber classificar problemas, buscar evidências e evitar conclusões apressadas.

## O problema que esta aula resolve

Muitos iniciantes tratam qualquer problema como “deu erro”. A tela não abriu, o relatório saiu diferente, o arquivo não foi encontrado, o cadastro foi rejeitado, a cobrança ficou errada, o programa parou, o resultado não bateu: tudo vira a mesma frase. O problema é que essa frase descreve uma percepção, mas não explica causa, momento, camada, impacto ou condição.

Quando um profissional escuta que “deu erro”, precisa investigar melhor. O problema ocorreu antes da execução, durante a execução ou depois dela? A entrada estava correta? O processamento aplicou a regra certa? A saída foi gerada no formato esperado? O ambiente era o correto? O arquivo estava no caminho certo? O usuário tinha permissão? A configuração apontava para o lugar adequado? A regra de negócio estava clara? Havia logs ou evidências?

Sem essas perguntas, a análise fica frágil. O aluno pode culpar o código quando o problema estava nos dados, culpar o usuário quando a interface induziu ao erro, culpar o ambiente quando a regra estava mal definida ou aceitar uma saída incorreta apenas porque o sistema não parou. Esta aula organiza o vocabulário inicial para evitar esse tipo de simplificação.

## Introdução

As aulas anteriores construíram uma sequência. Tecnologia da informação foi apresentada como relação entre pessoas, processos, dados e tecnologia. Sistema foi estudado como conjunto de partes relacionadas, com entradas, processamento, saídas, fronteiras e ambiente. Hardware, software e pessoas mostraram que computação envolve componentes físicos, componentes lógicos e ação humana.

Depois, dados, informação e conhecimento mostraram que registros precisam de contexto. Processamento foi entendido como transformação orientada por regras. Entrada, processamento e saída deram uma forma para enxergar fluxos. Programa e código-fonte mostraram que comportamento pode ser descrito por instruções. Compilação, interpretação e execução explicaram que escrever, preparar e executar não são a mesma coisa. Arquivos e pastas mostraram onde dados, instruções, entradas, saídas e evidências podem ficar. Ambientes computacionais mostraram que nada roda isolado das condições ao redor.

Agora, o aluno precisa entender como problemas aparecem. Um erro pode surgir na escrita de uma instrução, na lógica de uma regra, durante a execução, na operação real, nos dados, no ambiente, na configuração, na permissão, em arquivos ou em integrações. Aprender a nomear esses tipos de problema é parte da alfabetização técnica.

## “Deu erro” não é diagnóstico

Dizer apenas “deu erro” raramente ajuda a resolver um problema. Essa frase pode ser o começo de uma investigação, mas não o diagnóstico. Ela não informa onde o problema ocorreu, que entrada foi usada, qual resultado era esperado, qual resultado foi obtido, em que ambiente aconteceu, quem executou, qual arquivo foi processado, qual regra deveria valer ou que evidência existe.

Um diagnóstico técnico precisa aproximar o problema de sua causa provável. Se um relatório saiu com total errado, a causa pode estar no cálculo, no filtro, nos dados de entrada, na regra de negócio, na versão do programa, no ambiente, no arquivo usado, na data de referência ou na interpretação do usuário. A frase “deu erro” não diferencia nada disso.

Classificar o tipo de erro é parte do raciocínio técnico. Não significa encontrar a causa imediatamente, mas organizar a busca. Um erro de sintaxe pede uma investigação diferente de um erro lógico. Um erro de execução pede atenção a condições de runtime, recursos, arquivos e permissões. Um erro operacional pede olhar para processo, sequência, conferência e contexto real de uso.

## O que é erro em sentido amplo

Em sentido amplo, erro é uma diferença entre o que era esperado e o que ocorreu, ou uma violação de regra, expectativa, condição, formato, comportamento ou resultado. Essa ideia vale fora da programação. Se uma entrega deveria chegar a um endereço e vai para outro, há erro no processo. Se uma planilha soma a coluna errada, há erro no resultado. Se uma pessoa aprova uma solicitação sem a documentação exigida, há erro em relação à regra.

Em processos manuais, erros podem surgir por informação incompleta, interpretação errada, procedimento confuso, falta de conferência ou regra mal comunicada. Em processos administrativos, podem aparecer como cadastro duplicado, documento vencido, valor lançado no centro de custo errado ou prazo calculado de forma incorreta. Em sistemas computacionais, erros podem envolver instruções, dados, arquivos, permissões, ambiente, integração, processamento e saída.

O ponto comum é a divergência entre expectativa e ocorrência. A expectativa pode vir de uma regra formal, de uma necessidade do negócio, de um formato aceito, de um contrato, de uma configuração ou de uma condição técnica. Entender a origem da expectativa ajuda a entender o erro.

## Termos próximos e convenção operacional da aula

Na prática cotidiana, “erro” pode significar engano humano, defeito no código, dado incorreto, mensagem apresentada, interrupção, resultado errado ou incidente de produção. Fontes de teste e engenharia de software também variam em seus termos. Para evitar que uma palavra ampla esconda a investigação, esta aula adota uma convenção operacional inspirada em vocabulários de teste, sem apresentá-la como terminologia universal.

**Engano humano** é ação, interpretação ou decisão humana inadequada que pode introduzir um problema. **Defeito** — também chamado de falta ou fault em algumas fontes — é problema presente em requisito, projeto, código, configuração, dado, procedimento ou outro artefato. **Falha** é comportamento observado diferente do esperado durante uso ou execução. **Incidente** é evento operacional que interrompe, degrada ou ameaça um serviço, processo ou usuário. **Sintoma** é evidência observada; **causa** é condição ou conjunto de condições que contribuiu para o problema.

Um modelo didático útil é: engano, condição ou decisão inadequada → possível introdução de defeito → ativação sob determinadas condições → falha observável → possível incidente e impacto. O modelo não descreve todos os casos. Um defeito pode nunca ser ativado; uma falha pode não produzir incidente relevante; um incidente pode resultar da combinação de ambiente, processo, dado e decisão; e não existe sempre um único culpado ou uma única “causa raiz”.

Resultado incorreto pode ser mais perigoso que uma parada explícita, pois parece normal até alguém conferir. Mensagem de erro pode ser sintoma de causa mais profunda. E comportamento inesperado pode revelar defeito, regra desconhecida, expectativa equivocada ou configuração diferente. A utilidade da terminologia está em tornar perguntas mais precisas, não em forçar todo problema a uma etiqueta única.

## Erro de sintaxe

Erro de sintaxe é problema na forma de escrita de uma instrução, comando, expressão ou estrutura, segundo as regras de uma linguagem ou formato. Toda linguagem formal tem regras. A Aula 08 mostrou que código-fonte não é intenção solta: ele precisa obedecer a uma forma que ferramentas possam analisar. A Aula 09 mostrou que compilação, interpretação e execução dependem de etapas que precisam compreender essa forma.

Um exemplo conceitual fora do código ajuda. Em português, uma frase com palavras fora de ordem pode dificultar a compreensão. Em um formulário, escrever uma data em formato não aceito pode fazer o sistema rejeitar a entrada. Em uma linguagem formal, esquecer um elemento obrigatório, usar um símbolo fora de lugar ou montar uma estrutura inválida impede que a ferramenta aceite aquilo como instrução válida.

Erro de sintaxe costuma aparecer antes da execução completa, porque a ferramenta não consegue compreender ou aceitar a estrutura. Ele não diz necessariamente que a ideia de negócio está errada; diz que a forma escrita não respeita as regras esperadas. Corrigir sintaxe é fazer a estrutura ser compreendida, mas isso não garante que o raciocínio esteja correto.

## Defeito lógico e falha lógica observada

“Erro lógico” é expressão comum, mas mistura níveis. Pode haver raciocínio inadequado, regra mal compreendida, algoritmo incorreto, implementação incorreta ou falha observada no resultado. Nesta aula, é mais preciso dizer que existe **defeito lógico** quando requisito, especificação, algoritmo ou implementação expressa regra inadequada; a saída incorreta é a possível falha observada. A escrita formal pode estar correta e o sistema pode executar normalmente mesmo assim.

Se um desconto deve ser calculado sobre o valor líquido, mas é calculado sobre o valor bruto, há erro lógico. Se uma regra de idade é invertida e aceita quem deveria ser recusado, há erro lógico. Se a data de vencimento é calculada somando dias corridos quando a regra exige dias úteis, o resultado pode parecer tecnicamente válido, mas estar errado para o negócio.

Outros exemplos aparecem em relatórios que somam campo indevido, validações que aceitam situação que deveria rejeitar, tarifas que aplicam percentual errado ou filtros que deixam de considerar uma condição importante. O perigo do erro lógico é que o sistema pode executar sem mensagens de falha. A saída existe, o arquivo é gerado, a tela aparece, mas o resultado está incorreto.

## Falhas detectadas durante a execução

“Erro de execução” é útil como descrição do momento em que algo se manifesta, mas não identifica causa única. Durante execução, programa, rotina ou sistema usam arquivos, dados, memória, permissões, configurações, dependências e recursos. Uma falha nesse momento pode decorrer de defeito de código, entrada inesperada, dado inválido, recurso indisponível, integração, configuração, ambiente, condição concorrente ou combinação desses fatores.

Arquivo ausente, permissão negada, divisão por zero, dado incompatível, conexão interrompida, falta de memória, dependência ausente ou caminho inválido são hipóteses de investigação, não causas equivalentes. A Aula 09 preparou a diferença entre artefato, processo e execução; a Aula 10 mostrou o papel dos arquivos; a Aula 11 explicou que o ambiente influencia o comportamento.

Esse tipo de erro mostra que um programa não vive isolado. Mesmo que a sintaxe esteja correta e a lógica pareça adequada, a execução pode encontrar uma condição que impede o funcionamento. Investigar erro de execução exige observar momento, ambiente, entrada, recurso acessado, mensagem, log e contexto.

## Erro operacional

Erro operacional é problema relacionado à execução de uma rotina, procedimento, processo ou uso de sistema no contexto real da operação. Pode envolver execução em horário errado, uso de arquivo errado, escolha de ambiente errado, sequência incorreta de passos, falha de conferência, comunicação incompleta, liberação indevida, operação duplicada ou ausência de evidência.

Esse tipo de erro não significa simplesmente “culpa da pessoa”. Muitas vezes ele revela falha de processo, treinamento insuficiente, ferramenta confusa, documentação incompleta, controle frágil ou desenho de sistema que permite uma ação indevida. Uma pessoa pode executar a rotina errada porque os nomes são ambíguos, porque não havia bloqueio, porque a instrução estava desatualizada ou porque a interface não deixava claro o ambiente.

Em sistemas corporativos, erro operacional precisa ser tratado com seriedade porque acontece no fluxo real de trabalho. A correção pode envolver melhoria de processo, validação, autorização, registro, treinamento, mensagem mais clara ou restrição técnica. Culpar rapidamente alguém não resolve a causa.

## Erro de ambiente

Erro de ambiente é problema causado pelas condições onde o sistema roda ou é usado. Ele pode ocorrer por configuração incorreta, versão errada, banco indisponível, arquivo em caminho diferente, permissão insuficiente, dependência ausente, serviço externo fora do ar, dados de teste usados como se fossem produção ou execução no ambiente errado.

A Aula 11 mostrou que ambiente não é apenas máquina. Ele inclui sistema operacional, arquivos, usuários, permissões, configurações, rede, dados, versões, bibliotecas, banco de dados e integrações. Se uma dessas condições não corresponde ao esperado, o sistema pode falhar ou produzir resultado inadequado.

Um erro de ambiente explica situações como “funcionou em teste, mas falhou em produção”. Essa frase não encerra a análise; ela abre uma comparação entre ambientes. O que mudou? Dados? Caminho? Permissão? Configuração? Versão? Serviço externo? Banco? Sem essa comparação, a investigação fica incompleta.

## Erro de dado

Erro de dado é problema causado por dado incorreto, incompleto, duplicado, inconsistente, ambíguo, desatualizado, fora de formato ou sem contexto. A Aula 04 mostrou que dado precisa de significado, qualidade e contexto para virar informação útil. Um sistema pode aplicar regras corretamente sobre dados ruins e produzir resultados ruins.

Se um cliente está cadastrado com documento incorreto, uma validação pode rejeitar a operação. Se um produto aparece duplicado, o estoque pode ser calculado de forma errada. Se uma data está em formato inesperado, o processamento pode falhar. Se uma tabela de preços está desatualizada, a cobrança pode sair incorreta mesmo que o programa esteja tecnicamente funcionando.

Erros de dado são especialmente importantes porque muitas vezes parecem erro do sistema. Às vezes o sistema apenas revela a inconsistência que já estava no registro. Em outras situações, o próprio sistema permitiu entrada ruim por falta de validação. Por isso, análise madura observa tanto o dado quanto o processo que permitiu sua criação.

## Erro de regra de negócio

Erro de regra de negócio é problema na compreensão, documentação, implementação ou aplicação de uma regra organizacional. A regra pode estar mal definida, incompleta, contraditória, desatualizada ou diferente da prática real. Nesse caso, o sistema pode estar seguindo uma regra, mas a regra não representa corretamente o que deveria acontecer.

Em um banco, o cálculo de juros pode usar base incorreta. Em um benefício público, a elegibilidade pode ser interpretada sem considerar exceções. Em uma seguradora, a regra de cobertura pode estar desatualizada. Em comércio, a política de desconto pode não tratar promoção acumulada. Em crédito, um limite pode ser aplicado antes da atualização cadastral. Em cobrança, a geração de títulos pode ignorar uma condição de suspensão.

Esse tipo de erro mostra que tecnologia não é separada do negócio. Um programa pode executar bem uma regra ruim. Por isso, entender erro exige conversar com processo, regra, documentação, dados e pessoas responsáveis.

## O erro pode estar em várias camadas

Um problema aparente pode ter causa no código, no dado, no ambiente, na regra, no processo, na permissão, no arquivo, na integração, na configuração ou na operação. Uma análise madura evita conclusões rápidas porque a primeira manifestação nem sempre revela a causa.

Imagine um relatório de vendas com total incorreto. A causa pode ser lógica: o relatório somou campo errado. Pode ser dado: algumas vendas foram cadastradas em duplicidade. Pode ser ambiente: o relatório rodou em base de teste. Pode ser arquivo: a rotina leu uma entrada antiga. Pode ser configuração: o período de referência estava errado. Pode ser permissão: parte dos dados não estava acessível ao usuário. Pode ser regra: a definição de “venda válida” mudou. Pode ser operação: a rotina foi executada antes do fechamento.

O mesmo sintoma, total incorreto, pode ter causas diferentes. Investigar é separar camadas, coletar evidências e comparar o esperado com o ocorrido.

## Classificação por dimensões, não por etiqueta única

Em vez de escolher uma categoria exclusiva, é mais útil descrever um problema por dimensões. A primeira é a **origem possível**: requisito, regra de negócio, projeto, algoritmo, código, dado, configuração, integração, ambiente, procedimento, ação humana, documentação ou infraestrutura. A segunda é o **momento de detecção**: escrita, análise, compilação, ligação, inicialização, execução, validação de saída, operação ou auditoria.

Também importa registrar a **manifestação**: rejeição, mensagem, resultado incorreto, interrupção, lentidão, indisponibilidade, perda, duplicidade, inconsistência ou comportamento intermitente. E o **impacto**: nenhum impacto percebido, impacto local, operacional, financeiro, regulatório, de segurança, reputacional ou humano. As listas são exemplos iniciais, não taxonomia fechada.

Assim, um arquivo de folha processado duas vezes pode ter origem operacional e de controle, ser detectado na conferência de saída, manifestar duplicidade e causar impacto financeiro. A mesma ocorrência pode envolver configuração inadequada, interface confusa ou regra de prevenção ausente. Classificar por dimensões preserva complexidade suficiente para investigar sem impedir ação.

## Entrada, processamento, saída e erro

A Aula 06 apresentou o modelo entrada, processamento e saída. Erros podem aparecer em qualquer parte desse fluxo. Na entrada, pode haver dado inválido, formato incorreto, arquivo errado, informação incompleta ou valor fora das regras. Se a entrada é ruim, o processamento pode falhar ou produzir saída ruim.

Durante o processamento, a regra pode estar errada, a sequência pode ser inadequada, a condição pode estar invertida, o cálculo pode usar base incorreta ou uma exceção pode não ter sido tratada. Na saída, o resultado pode ser gerado em formato incorreto, enviado para destino errado, apresentado de forma ambígua ou interpretado de maneira equivocada.

Essa visão ajuda a localizar o problema. Antes de dizer que o sistema “errou”, é preciso perguntar: a entrada era válida? O processamento aplicou a regra certa? A saída corresponde ao esperado? O erro está no dado que entrou, na transformação feita ou no resultado produzido?

## Arquivos e erros

A Aula 10 mostrou que arquivos têm nome, conteúdo, formato, extensão, caminho, versão e contexto. Cada um desses elementos pode participar de erro. Um arquivo ausente pode impedir processamento. Nome errado pode fazer uma rotina não reconhecer a entrada. Versão antiga pode produzir resultado desatualizado. Formato incorreto pode causar rejeição. Conteúdo inválido pode passar pela abertura, mas falhar nas regras.

Também há risco quando arquivo de teste é usado em produção, arquivo duplicado é processado duas vezes, permissão de leitura é negada, saída é sobrescrita, arquivo está incompleto ou material é enviado para destino errado. Em sistemas corporativos, isso pode afetar cobrança, folha, estoque, contabilidade, auditoria e atendimento.

Arquivos frequentemente servem como entrada, saída e evidência. Por isso, investigar erro envolvendo arquivos exige verificar se o arquivo certo foi usado, em qual versão, em qual ambiente, com qual conteúdo, por quem, quando e para qual processamento.

## Ambiente e erros

A Aula 11 mostrou que muitos erros só aparecem em determinado ambiente. Um programa pode funcionar no ambiente local e falhar em produção porque os dados são diferentes, as permissões são mais restritas, os caminhos mudaram, a configuração aponta para outro serviço, a versão é diferente ou uma dependência externa está indisponível.

A frase “funcionou no meu ambiente” não encerra a investigação. Ela indica que, em um conjunto de condições, o comportamento foi observado. O ambiente real pode ter outras condições. Em sistemas corporativos, produção tem dados reais, usuários reais, integrações reais, controles mais rígidos e consequências reais.

Comparar ambientes é parte da análise. É preciso observar versão do programa, versão de configuração, banco acessado, arquivos disponíveis, permissões, horários, serviços externos, volume de dados e logs. Sem isso, o erro pode ser corrigido no lugar errado.

## Mensagens de erro

Mensagens de erro têm papel importante porque podem indicar causa, local, tipo de problema ou sintoma. Uma boa mensagem ajuda a entender se o arquivo não foi encontrado, se a permissão foi negada, se o formato é inválido, se a conexão falhou ou se uma regra rejeitou a entrada.

Mas mensagens não devem ser interpretadas isoladamente. Às vezes a mensagem mostra apenas a consequência final. Um sistema pode informar que não conseguiu gerar relatório, mas a causa real pode ser falta de permissão, dados inconsistentes, configuração errada ou serviço indisponível. A mensagem é uma pista, não necessariamente a explicação completa.

Ler mensagens com atenção é um hábito técnico. Ignorá-las atrasa a análise. Copiá-las sem entender também não basta. O profissional precisa relacionar mensagem, momento, ambiente, entrada, logs e comportamento observado.

## Logs, evidências e rastreabilidade

Sistemas corporativos precisam registrar eventos, execuções, falhas, horários, usuários, entradas, saídas, retornos e decisões relevantes. Logs e evidências ajudam a reconstruir o que ocorreu. Eles indicam etapas realizadas, mensagens emitidas, registros rejeitados, arquivos usados, retornos recebidos e condições encontradas.

Rastreabilidade é a capacidade de acompanhar o histórico de um processamento, dado ou evento. Sem rastreabilidade, uma equipe pode saber apenas que houve problema, mas não conseguir demonstrar quando aconteceu, quem executou, que versão estava ativa, que entrada foi usada ou qual saída foi gerada.

Não é necessário aprofundar observabilidade agora. O ponto essencial é que investigação e auditoria dependem de registros. Em sistemas críticos, corrigir o problema é importante, mas entender e comprovar o que aconteceu também é parte da responsabilidade.

## Como investigar um erro conceitualmente

Investigar erro começa por comparar expectativa e ocorrência. O que era esperado? O que ocorreu? Quando ocorreu? Em qual ambiente? Com quais dados? Qual entrada foi usada? Qual regra deveria ser aplicada? Qual saída foi gerada? O problema é reproduzível? Há logs ou evidências? O erro ocorreu antes, durante ou depois da execução? A causa provável está no código, no dado, na configuração, no ambiente, na regra, no processo ou na operação?

Essas perguntas não são uma receita mecânica, mas um roteiro de raciocínio. Primeiro, é preciso descrever o problema com precisão. Depois, localizar o momento do fluxo. Em seguida, comparar condições: ambiente, dados, arquivos, versões e permissões. Também é necessário observar se o problema acontece sempre ou apenas em situação específica.

Uma investigação bem conduzida evita corrigir sintoma sem entender causa. Se uma rotina falha porque o arquivo está ausente, criar manualmente um arquivo qualquer pode esconder o problema real: talvez a etapa anterior não tenha gerado a entrada, talvez o caminho esteja errado, talvez a permissão tenha mudado. Diagnóstico exige contexto.

## Erros em sistemas corporativos

Em um banco, um erro lógico no cálculo de juros pode cobrar valor indevido. A causa pode estar na regra, na data de referência ou na base de cálculo. O impacto pode ser financeiro, regulatório e reputacional. A investigação precisa revisar regra aplicada, dados de contrato, versão do programa, logs e amostras de cálculo.

No governo, um erro de dado pode negar benefício a uma pessoa elegível. A causa pode ser cadastro incompleto, integração falha ou regra desatualizada. O impacto pode ser humano, jurídico e operacional. É necessário investigar origem do dado, validações, histórico, ambiente e evidências de processamento.

Em uma seguradora, um erro de regra de negócio pode recusar sinistro que deveria seguir para análise. A causa pode ser interpretação incorreta de cobertura ou exceção não documentada. No comércio, um erro de ambiente pode apontar para tabela de preços antiga e gerar venda com valor errado. Em folha de pagamento, arquivo de banco em versão incorreta pode atrasar salários.

Em telecom, erro de execução em rotina de faturamento pode interromper processamento de consumo. Em cobrança e cartões, arquivo duplicado pode gerar tentativa repetida de liquidação. Em contabilidade, relatório com filtro errado pode comprometer fechamento. Em atendimento ao cliente, permissão inadequada pode impedir consulta necessária ou expor dado indevido. Em todos os casos, é preciso identificar tipo de erro, causa provável, impacto e evidência disponível.

## Impacto real dos erros

Erros em sistemas corporativos podem gerar consequências financeiras, operacionais, jurídicas, regulatórias, reputacionais e humanas. Um pagamento errado afeta pessoas e caixa. Uma cobrança indevida pode gerar reclamações, estornos e perda de confiança. Um benefício negado indevidamente pode prejudicar alguém. Uma informação vazada pode violar segurança e privacidade.

Relatório incorreto pode orientar decisão ruim. Saldo inconsistente pode comprometer atendimento e conciliação. Operação duplicada pode movimentar valor duas vezes. Atraso em fechamento pode afetar contabilidade, prazos e obrigações. Falha de auditoria pode impedir comprovação de uma ação.

Por isso, erro não é apenas incômodo técnico. Em sistemas reais, erro tem contexto e consequência. A gravidade depende do processo afetado, do dado envolvido, da quantidade de pessoas impactadas, da possibilidade de correção e da capacidade de demonstrar o que aconteceu.

## Erro não é sempre culpa do usuário

Culpar o usuário rapidamente é uma postura fraca tecnicamente. Às vezes a pessoa executou uma ação indevida, mas é preciso perguntar por que essa ação foi possível ou provável. A interface estava clara? O processo era compreensível? A regra foi explicada? Havia validação? A mensagem orientava corretamente? O sistema bloqueava operação perigosa?

Erro pode ser consequência de interface ruim, processo confuso, treinamento insuficiente, documentação desatualizada, mensagem ambígua ou sistema que permite escolha inadequada sem confirmação. Quando a análise para na frase “foi erro do usuário”, a organização perde chance de melhorar ferramenta, regra, treinamento e controle.

Isso não elimina responsabilidade humana. Significa apenas que responsabilidade técnica exige investigar o sistema de trabalho como um todo: pessoas, processo, ferramenta, ambiente e informação.

## Erro não é sempre culpa do programador

Também é incorreto presumir que todo erro vem do código. Um programa pode estar tecnicamente correto e falhar por ambiente, dado, configuração, operação, integração, dependência externa, regra ambígua ou processo incorreto. Se o banco está indisponível, se o arquivo enviado está vazio, se a regra mudou sem comunicação ou se a operação executou rotina fora de sequência, o código pode ser apenas uma parte do cenário.

Isso não significa proteger código de análise. Código deve ser investigado quando faz parte da hipótese. Mas uma análise madura distribui perguntas pelas camadas corretas. Procurar defeito apenas no código pode desperdiçar tempo e deixar a causa real ativa.

O profissional precisa combinar humildade e método. O problema pode estar no que foi programado, no que foi pedido, no que foi configurado, no que foi informado, no que foi operado ou no que estava disponível no ambiente.

## Tratamento de erro em nível conceitual

Sistemas precisam prever situações anormais. Tratamento de erro, em nível conceitual, é a forma como um sistema evita que uma condição problemática gere dano maior. Isso pode envolver validar entrada, rejeitar dados inválidos, registrar falhas, impedir operação insegura, avisar o usuário, permitir reprocessamento, preservar evidências e interromper uma rotina quando continuar seria perigoso.

Um sistema que recebe arquivo em formato errado pode rejeitá-lo e informar o motivo. Uma rotina que encontra registro inválido pode separá-lo em arquivo de rejeição. Uma tela pode impedir envio de cadastro incompleto. Um processamento pode registrar log antes de parar. Uma operação crítica pode exigir confirmação ou autorização.

Não é necessário aprender programação de tratamento de erro agora. O essencial é entender que sistemas responsáveis não fingem que situações anormais nunca acontecerão. Eles precisam reconhecer, limitar impacto, registrar e permitir investigação.

## Conexão futura com Mainframe e COBOL

Em ambientes Mainframe e COBOL, erros podem aparecer em compilação, execução de programas, processamento batch, leitura de arquivos, validação de registros, retorno de execução, permissões, datasets, JCL, integração com bancos e operação. A base desta aula ajudará o aluno a não tratar todos esses problemas como uma única categoria.

Futuramente, aparecerão códigos de retorno, abends, logs, arquivos rejeitados, relatórios de erro, rotinas de reprocessamento e controles de produção. Esses temas serão estudados tecnicamente no momento adequado. Agora, basta entender que sistemas corporativos precisam indicar, registrar, classificar e tratar problemas com cuidado.

Esta aula não ensina COBOL, JCL, abend, return code, z/OS ou comandos. Ela prepara a leitura conceitual para quando esses termos surgirem dentro de ambientes controlados, processamento batch e sistemas críticos.

## Confusões comuns de iniciantes

Uma confusão comum é achar que todo erro é igual. Essa visão impede distinguir sintaxe, lógica, execução, ambiente, dado, regra e operação. Sem classificação, a pessoa tenta resolver problemas diferentes com a mesma abordagem.

Outra confusão é achar que erro é sempre culpa do código. Código pode ser a causa, mas dados ruins, ambiente errado, permissão insuficiente, regra ambígua ou operação inadequada também podem produzir problemas. O oposto também é frágil: culpar sempre o usuário ignora falhas de interface, processo, validação, documentação e controle.

Muitos iniciantes acham que, se compilou, está certo. Compilar ou ser aceito por uma ferramenta indica que a forma foi compreendida, não que a regra está correta. Também acham que, se executou, resolveu. Um sistema pode executar sem parar e ainda gerar resultado errado.

Mensagens de erro também são mal interpretadas. Às vezes indicam causa com clareza; às vezes mostram apenas sintoma. Ignorar ambiente, dados, regra de negócio, arquivos, permissões e operação faz a investigação ficar estreita. Corrigir sintoma sem causa pode fazer o problema voltar.

Por fim, não registrar evidências enfraquece qualquer análise. Sem logs, horários, entradas, saídas, versões e contexto, a investigação depende de memória e impressão. Diferenciar erro lógico de erro de execução, por exemplo, exige observar se a regra estava errada ou se a execução encontrou uma condição que impediu o comportamento esperado.

## Perguntas para reflexão

- Por que a frase “deu erro” não é suficiente para orientar uma investigação técnica?
- Em que situação um sistema pode executar normalmente e ainda produzir resultado errado?
- Como você diferenciaria erro de sintaxe, erro lógico, erro de execução e erro operacional?
- Que perguntas ajudam a descobrir se um problema está na entrada, no processamento ou na saída?
- Como arquivos, versões e caminhos podem participar de um erro?
- Por que ambiente deve ser investigado quando algo funciona em um lugar e falha em outro?
- Que riscos surgem ao culpar automaticamente o usuário ou o programador?
- Que evidências seriam úteis para reconstruir um erro em sistema corporativo?

## Síntese da aula

“Erro” é palavra ampla e, sozinha, não é diagnóstico. A convenção operacional desta aula distingue engano humano, defeito em artefato ou condição, falha observada e incidente operacional. Sintoma não é necessariamente causa. Defeito lógico pode estar em requisito, especificação, algoritmo ou implementação; uma falha durante execução descreve momento de manifestação, não causa única.

Dados, ambiente, configuração, regra e operação são dimensões possíveis de origem e contexto, não etiquetas mutuamente exclusivas. Um sistema pode estar tecnicamente funcionando e ainda produzir resultado errado. A análise deve observar entrada, processamento, saída, arquivos, permissões, versões, operação, mensagens, logs e evidências; formular hipóteses; comparar esperado e observado; conter impacto; corrigir, validar e prevenir recorrência.

Esta aula encerra as 12 aulas conceituais planejadas da Fase 0 — Alfabetização Técnica. A próxima etapa do projeto não deve ser pular imediatamente para a Fase 1. Antes disso, a próxima etapa deve ser a Consolidação da Fase 0 — revisão geral, estudo dirigido, exercícios teóricos, avaliação e checklist final, para verificar se o vocabulário básico realmente foi assimilado.

## Mini glossário da aula

- Erro: palavra ampla; nesta aula, usar com qualificador ou preferir engano, defeito, falha ou incidente conforme a dimensão analisada.
- Engano humano: ação, interpretação ou decisão inadequada que pode introduzir problema.
- Defeito: problema presente em requisito, projeto, código, configuração, dado, procedimento ou outro artefato; algumas fontes usam falta ou fault.
- Falha: comportamento observado diferente do esperado durante uso ou execução.
- Incidente: evento operacional que interrompe, degrada ou ameaça serviço, processo ou usuário.
- Comportamento inesperado: ação ou resposta que surpreende em relação à expectativa de uso ou regra.
- Resultado incorreto: saída errada, mesmo que o sistema tenha executado sem parar.
- Erro de sintaxe: problema na forma de escrita segundo regras de uma linguagem ou formato.
- Defeito lógico: inadequação em requisito, regra, algoritmo ou implementação que pode levar a resultado incorreto.
- Falha durante execução: manifestação detectada enquanto programa, rotina ou sistema executa; não indica causa única.
- Erro operacional: problema ligado ao uso real, sequência, procedimento, rotina, conferência ou operação.
- Erro de ambiente: problema causado por configurações, permissões, versões, recursos ou condições do ambiente.
- Erro de dado: problema causado por dado incorreto, incompleto, duplicado, inconsistente ou fora de contexto.
- Erro de regra de negócio: problema na compreensão, documentação, implementação ou aplicação de regra organizacional.
- Mensagem de erro: comunicação emitida por sistema ou ferramenta para indicar problema, causa provável ou sintoma.
- Log: registro de eventos, mensagens, horários, etapas e falhas.
- Evidência: informação preservada que ajuda a comprovar o que ocorreu.
- Rastreabilidade: capacidade de acompanhar origem, execução, alteração, resultado e histórico de um processo.
- Diagnóstico: análise que busca identificar tipo, causa e contexto de um problema.
- Causa: condição que originou ou contribuiu para o problema.
- Fator contribuinte: condição que, em combinação com outras, favorece a ocorrência ou o impacto.
- Sintoma: manifestação percebida do problema.
- Reprodução: capacidade de fazer o problema ocorrer novamente sob condições conhecidas.
- Validação: verificação de entrada, regra, condição ou resultado contra critérios esperados.
- Tratamento de erro: forma como um sistema reconhece, limita, registra ou responde a situações anormais.
- Contenção: ação para limitar impacto imediato.
- Correção: alteração para remover ou reduzir causa conhecida.
- Prevenção: medida para reduzir probabilidade ou impacto de recorrência.
- Impacto operacional: efeito de um problema sobre rotina, atendimento, prazo, processamento ou continuidade.
- Reprocessamento: nova execução de uma rotina ou etapa para corrigir, completar ou refazer resultado sob controle.

## Critérios de domínio

Ao final desta aula, o aluno deve ser capaz de explicar por que “deu erro” não é diagnóstico suficiente; diferenciar erro de sintaxe, erro lógico, erro de execução e erro operacional; reconhecer erro de ambiente, erro de dado e erro de regra de negócio; entender que compilar não garante correção; entender que executar sem falhar não garante resultado correto; analisar um problema considerando entrada, processamento, saída, ambiente, arquivo, dado, regra e operação; explicar por que logs, evidências e rastreabilidade importam; evitar culpar automaticamente usuário ou programador; reconhecer impacto real de erros em sistemas corporativos; e conectar o tema com Mainframe, COBOL, batch, produção e sistemas críticos futuramente.

## Referências e leituras para aprofundamento

- ISO/IEC/IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*.
- International Software Testing Qualifications Board. *ISTQB Glossary*.
- Python Software Foundation. *Python Language Reference — Execution model*.
