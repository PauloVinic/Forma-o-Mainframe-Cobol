# Aula 09 — Compilação, interpretação e execução

## Objetivo da aula

O objetivo desta aula é explicar, em nível conceitual, como um código-fonte pode deixar de ser apenas uma representação textual de um programa e passar a produzir comportamento em um ambiente computacional. Ao final, o aluno deve conseguir diferenciar escrever código-fonte, preparar um programa para execução, interpretar instruções, executar um programa e observar resultados.

A aula também deve formar uma distinção importante para todo o restante da formação: código-fonte, executável, script, bytecode, ambiente de execução e processo em execução não são nomes diferentes para a mesma coisa. Eles indicam momentos, formas ou componentes diferentes no caminho entre instruções escritas por pessoas e comportamento efetivamente realizado por computadores.

O foco permanece introdutório. Não será ensinado nenhum comando, nenhuma ferramenta, nenhuma linguagem específica e nenhum procedimento prático de compilação. O propósito é construir vocabulário para que, nas próximas etapas, o aluno compreenda arquivos, ambientes, erros, linguagens, COBOL, JCL e Mainframe sem imaginar que "rodar um programa" é uma ação única e simples.

## O problema que esta aula resolve

Muitos iniciantes confundem escrever código-fonte com executar um programa. A pessoa vê um texto estruturado em uma linguagem de programação e imagina que aquele texto, por si só, já está fazendo algo no computador. Também é comum usar a palavra "rodar" para tudo: abrir uma ferramenta, traduzir código, iniciar execução, processar dados, gerar saída e conferir resultado. Essa palavra pode ser útil em conversa informal, mas esconde etapas diferentes.

Essa confusão atrapalha porque problemas podem surgir em momentos distintos. Um código pode estar mal escrito e nem ser aceito por uma ferramenta. Pode ser aceito e traduzido, mas falhar ao iniciar por falta de recurso. Pode executar durante algum tempo e parar ao encontrar um dado inesperado. Pode executar até o fim e produzir um relatório incorreto porque a regra de negócio foi mal representada. Dizer apenas "deu erro" não explica em que camada o problema apareceu.

Esta aula resolve essa lacuna separando texto, preparação, execução e resultado. O aluno precisa entender que existe um caminho entre o código-fonte escrito por pessoas e o comportamento observado em um sistema. Esse caminho pode envolver compilação, interpretação, ambiente de execução, arquivos, permissões, versões, dados, parâmetros e validação de saídas.

## Introdução

As aulas anteriores construíram a base necessária para chegar a este tema. Tecnologia da informação foi apresentada como uso organizado de tecnologia para lidar com dados, informação, processos e decisões. Sistemas foram estudados como conjuntos de componentes relacionados. Hardware, software e pessoas foram analisados como partes de sistemas computacionais. Dados, informação e conhecimento mostraram a importância do contexto. Processamento foi explicado como transformação orientada por regras. O modelo entrada, processamento e saída ajudou a enxergar fluxos. Programa foi estudado como conjunto organizado de instruções. Código-fonte foi apresentado como representação textual formal de um programa.

Agora surge a pergunta que a Aula 08 preparou: se código-fonte é texto formal, como esse texto passa a produzir comportamento? Um arquivo de código pode estar salvo em uma pasta, pode ser lido por um desenvolvedor, pode ser revisado por uma equipe e pode estar guardado por anos sem executar nada. Para que produza efeito, precisa ser tratado por algum mecanismo e colocado em funcionamento em algum ambiente.

Essa passagem entre representação e comportamento é essencial para computação. O computador não executa intenção humana diretamente, e também não executa qualquer texto técnico apenas porque parece organizado. Linguagens, ferramentas e ambientes existem para transformar, analisar, conduzir ou executar instruções de forma controlada. Entender essa passagem evita várias confusões futuras.

## Código-fonte não é execução

Código-fonte é uma representação formal de um programa, mas não é automaticamente execução. Ele pode estar em um arquivo parado no armazenamento, sem consumir CPU, sem ocupar memória de execução, sem ler entradas e sem produzir saídas. Nessa condição, ele existe como texto estruturado, disponível para leitura, edição, análise ou preparação.

Um arquivo de código-fonte pode ser aberto por uma pessoa para estudo. Pode ser analisado por uma ferramenta para encontrar problemas de escrita. Pode ser traduzido para outra forma. Pode ser interpretado por um mecanismo que conduz suas instruções. Pode participar da geração de um artefato intermediário ou executável. Cada uma dessas situações é diferente de dizer que o programa está efetivamente em execução.

Existir como texto significa estar registrado em uma forma persistente, geralmente em arquivo. Estar em execução significa que o comportamento representado por esse texto está sendo conduzido por um ambiente computacional, usando recursos e tratando dados. Essa diferença será importante para entender arquivos, ambientes, processos, jobs, logs e erros.

## O que significa executar um programa

Executar um programa significa colocar seu comportamento em funcionamento em um ambiente computacional. Durante a execução, instruções são efetivamente realizadas, dados são acessados, recursos são consumidos e efeitos podem ser produzidos. Esses efeitos podem ser visíveis, como uma mensagem na tela, ou menos visíveis, como gravação de arquivo, atualização de registro, envio de mensagem a outro sistema ou geração de evidência.

Uma execução pode usar CPU, memória, armazenamento, arquivos, rede, banco de dados, entrada de usuário, parâmetros, permissões, bibliotecas, configurações e recursos do sistema operacional. A Aula 03 já mostrou que software não executa no vazio: ele depende de hardware e ambiente. Aqui, essa ideia ganha forma mais precisa. Um programa escrito ou armazenado não está automaticamente ativo; ele precisa ser iniciado e conduzido sob certas condições.

Não é necessário aprofundar sistemas operacionais neste momento. Essa será uma fase futura. Por enquanto, basta compreender que execução é atividade em andamento. Ela tem começo, consome recursos, pode produzir saídas, pode falhar, pode terminar e pode deixar registros do que aconteceu.

## Do código ao comportamento

Entre o código-fonte e o comportamento observado existe um caminho. Uma pessoa escreve uma representação formal usando uma linguagem de programação. Uma ferramenta, mecanismo ou ambiente analisa, traduz, prepara ou interpreta essa representação. Depois, durante a execução, o computador realiza operações sobre dados e recursos, produzindo resultados conforme as instruções e condições disponíveis.

Esse caminho pode assumir formas diferentes. Em algumas tecnologias, o código-fonte passa por compilação antes de ser executado. Em outras, um interpretador conduz as instruções no momento da execução. Em outras, o código é transformado em uma forma intermediária que será executada por uma máquina virtual ou por um runtime. O detalhe técnico varia, mas a ideia central permanece: o texto escrito por pessoas precisa ser tratado por mecanismos próprios para produzir comportamento computacional.

Essa visão também ajuda a separar responsabilidades. O código-fonte expressa regras e instruções. As ferramentas verificam e preparam ou conduzem essas instruções. O ambiente oferece recursos e condições. Os dados alimentam a execução. O resultado precisa ser analisado conforme a finalidade do sistema.

## O que é compilação

Compilação é, nesta aula, o processo de analisar e transformar uma representação de programa em outra representação. O resultado pode ser código de máquina, assembly, código objeto, bytecode, outra representação intermediária, outra linguagem ou artefato que ainda precisará ser combinado e carregado. Portanto, compilação não é sinônimo de gerar diretamente um arquivo executável nativo; é uma família de transformações usada em pipelines diferentes.

Durante a compilação, uma ferramenta chamada compilador pode realizar análise léxica, análise sintática, verificações semânticas, análise de tipos, transformações, otimizações e geração de outra representação. Nem todo compilador realiza as mesmas verificações e nem toda linguagem possui o mesmo sistema de tipos. Problemas de sintaxe, nomes não resolvidos, declarações ausentes, incompatibilidades de tipos, dependências ou ligação entre partes podem ser detectados em etapas diferentes, conforme linguagem e ferramenta. Compilação pode falhar; quando é bem-sucedida, demonstra somente que a ferramenta aceitou e transformou o artefato segundo as condições que verificou.

Compilação bem-sucedida não garante que o programa esteja correto em termos de regra de negócio. Ela indica que o código atendeu a certas exigências formais e pôde ser preparado. Um cálculo de desconto com fórmula errada pode compilar. Uma validação cadastral que aceita dado indevido pode compilar. Um relatório que soma campo errado pode compilar. A ferramenta não sabe automaticamente qual era a intenção da organização.

## O que é interpretação

Interpretação é execução mediada por programa ou ambiente que lê, analisa e realiza operações descritas por outra representação. Um interpretador pode trabalhar diretamente com código-fonte, com uma árvore ou estrutura interna, com bytecode ou com outra representação intermediária. A imagem de que ele executa “linha por linha” pode ajudar no início, mas é insuficiente: linhas são forma de apresentação para pessoas, e implementações reais podem analisar blocos, manter estruturas internas e compilar trechos durante a própria execução.

Comparar interpretação com compilação exige cuidado. Para iniciantes, é útil imaginar compilação como uma preparação anterior e interpretação como uma condução mais próxima do momento da execução. Mas essa distinção não deve virar regra rígida. Tecnologias reais podem misturar etapas, preparar partes antecipadamente, traduzir trechos sob demanda ou usar formas intermediárias.

O ponto comum é mais importante que a diferença: tanto compilação quanto interpretação existem para permitir que instruções expressas em linguagem de programação produzam comportamento computacional. Em ambos os casos, o código-fonte não é executado como uma frase em português. Ele é tratado por mecanismos que conhecem regras formais da linguagem e do ambiente.

## Compilação e interpretação não são inimigas

É comum ouvir que algumas linguagens são compiladas e outras são interpretadas. Essa classificação ajuda no começo, mas pode criar uma visão simplista. No mundo real, muitas tecnologias usam modelos mistos. Um código pode ser transformado em uma forma intermediária, depois executado por uma máquina virtual. Um ambiente pode interpretar instruções, mas também otimizar partes durante a execução. Uma linguagem pode ter várias implementações com estratégias diferentes.

Por isso, compilação e interpretação não devem ser vistas como inimigas nem como categorias morais. Uma não é automaticamente "séria" e a outra "fraca". Elas são formas diferentes, e às vezes combinadas, de levar instruções até o comportamento executado.

O aluno não precisa dominar esses detalhes agora. O cuidado didático é apenas impedir uma conclusão rígida: "compilado vira programa de verdade; interpretado é apenas texto". Essa frase é falsa e atrapalha o estudo. O que importa é entender que cada tecnologia define um caminho entre fonte, preparação, ambiente e execução.

## Executável, script, bytecode e ambiente de execução

Executável é uma forma preparada de um programa que pode ser colocada em execução por um ambiente compatível. Ele não é o código-fonte original, embora possa ter sido produzido a partir dele. Um executável depende de condições: sistema, permissões, recursos, bibliotecas, dados e contexto adequado.

Script é um texto de instruções normalmente conduzido por um interpretador ou ambiente capaz de lê-lo e executá-lo de forma mediada. O termo aparece muito em automação, tarefas operacionais e linguagens em que o próprio arquivo textual pode ser usado diretamente por um mecanismo de execução. Isso não significa que script seja improviso ou menos importante. Um script pode sustentar tarefas críticas se estiver inserido em processo controlado.

Bytecode é nome usado por algumas tecnologias para uma representação intermediária projetada para execução por máquina abstrata, interpretador ou runtime específico. Não existe um bytecode universal: formatos e objetivos variam. Bytecode não é sinônimo de toda representação intermediária e não é necessariamente código de máquina da CPU física; pode ser interpretado, verificado, transformado ou compilado novamente durante a execução.

Máquina concreta é o hardware ou arquitetura física que executa instruções da CPU. Máquina abstrata é modelo de execução definido por regras e instruções próprias. Neste contexto, máquina virtual de linguagem implementa uma máquina abstrata sobre outra plataforma. Virtualização completa de sistema operacional é outro uso do termo “máquina virtual” e será estudada futuramente; não deve ser confundida com a máquina virtual de uma linguagem.

Runtime é conjunto de mecanismos, bibliotecas, serviços e condições que apoiam uma tecnologia durante a execução. Conforme o ecossistema, pode incluir gerenciamento de memória, tratamento de exceções, carregamento de módulos, bibliotecas básicas, interface com sistema operacional, coleta de lixo, execução de bytecode ou compilação just-in-time. Nem todo runtime inclui todos esses elementos. Runtime não é sinônimo de sistema operacional, embora use seus serviços; também não é idêntico a máquina virtual ou ambiente de execução, embora possa fazer parte deles.

Esses termos aparecem no estudo de programação porque mostram que não existe uma única maneira de sair do código-fonte até a execução. Alguns caminhos geram executáveis. Outros conduzem scripts. Outros usam bytecode e máquinas virtuais. Todos dependem de ambiente.

## Representações intermediárias e pipelines possíveis

Uma representação intermediária existe quando uma ferramenta separa a forma em que o programa foi escrito da forma em que será finalmente executado. Essa separação pode facilitar análise, otimização, portabilidade e geração para arquiteturas diferentes. Ela não é obrigatória em toda tecnologia. O LLVM, por exemplo, documenta uma representação intermediária usada em análise e transformações; outras tecnologias adotam formatos e objetivos distintos.

Não há uma sequência universal de etapas. Um pipeline possível é: código-fonte → compilação → código objeto → ligação entre partes e bibliotecas → executável → carregamento → execução. Outro é: código-fonte → bytecode → runtime ou máquina virtual → execução, com possível compilação just-in-time de trechos durante o funcionamento. Alguns scripts são entregues diretamente a um interpretador. Os exemplos mostram modelos, não receitas que toda linguagem deve seguir.

**Compilação antecipada** (ahead-of-time, ou AOT) é estratégia em que transformação relevante ocorre antes da execução principal. **Compilação just-in-time** (JIT) é estratégia em que determinados trechos podem ser transformados durante ou próximo da execução. Uma implementação pode combinar as duas. Nenhuma estratégia, isoladamente, prova qualidade, segurança, correção ou desempenho em todas as situações.

## Carregamento, processo e execução

Além de compilar ou interpretar, alguns caminhos incluem montagem, ligação, carregamento e inicialização. Montagem costuma transformar assembly em forma mais próxima de código de máquina; ligação combina componentes e resolve referências entre eles; carregamento disponibiliza artefatos e recursos para que possam começar a executar. Nem todos os ambientes expõem essas etapas com os mesmos nomes ou separações.

A Aula 07 distinguiu programa armazenado de processo em execução. Um artefato armazenado pode ser fonte, script, bytecode, código objeto ou executável; nenhum deles está ativo apenas por existir. Quando um ambiente inicia uma execução, recursos e estado são associados a ela. Processo é a abstração de sistema operacional usada, em nível inicial, para representar essa execução ativa. O mesmo programa pode originar múltiplos processos ou execuções com entradas, versões e consequências diferentes.

## O que uma etapa bem-sucedida demonstra

Salvar um arquivo demonstra apenas que ele foi preservado. Análise sintática bem-sucedida não demonstra que a regra tem sentido. Compilação bem-sucedida não demonstra que a regra de negócio está correta. Ligação bem-sucedida não demonstra que o ambiente correto estará disponível. Iniciar execução não demonstra término correto; terminar sem falha aparente não demonstra resultado correto; resultado correto em um caso não prova correção geral.

Essa sequência prepara a próxima aula. Ela permite separar artefato, transformação, execução e resultado antes de investigar por que algo deu errado. Em um processamento de folha, por exemplo, o código pode compilar e gerar artefato; o processo pode iniciar com arquivo disponível; ainda assim, uma tabela de desconto desatualizada pode produzir valores incorretos. A causa pode estar em dado, requisito, configuração ou implementação, e não na etapa que apenas mostrou sucesso técnico.

## Programa armazenado e programa em execução

A Aula 07 introduziu a diferença entre programa armazenado e programa em execução. Agora essa diferença precisa ficar mais clara. Um programa armazenado pode existir em arquivo, em forma de código-fonte, executável, script ou artefato intermediário. Ele está preservado em algum lugar, mas não está necessariamente ativo.

Quando o programa é executado, torna-se uma atividade em andamento no ambiente computacional. Ele pode ocupar memória, receber parâmetros, abrir arquivos, consultar dados, produzir saídas e terminar com sucesso ou falha. O mesmo programa armazenado pode ser executado muitas vezes, em momentos diferentes, com entradas diferentes, por usuários diferentes ou em ambientes diferentes.

Essa distinção será importante para entender processos, jobs, rotinas, execução batch e ambientes corporativos. Um job futuro não será apenas "um programa guardado"; será uma execução organizada dentro de um ambiente, com entradas, saídas, dependências, evidências e resultado operacional.

## O papel do ambiente

Execução não ocorre no vazio. Um programa depende de ambiente: sistema operacional, permissões, variáveis, arquivos disponíveis, bibliotecas, configurações, bancos de dados, rede, horário, usuário, caminho de execução, recursos de hardware e versões de componentes. Quando uma dessas condições muda, o comportamento pode mudar ou a execução pode falhar.

O mesmo programa pode funcionar em um ambiente e falhar em outro. Em um lugar, o arquivo esperado existe; em outro, não. Em um ambiente, a permissão permite gravação; em outro, bloqueia. Em um ambiente, a configuração aponta para dados de teste; em outro, aponta para dados reais. Em um ambiente, a versão de uma biblioteca é compatível; em outro, não.

Essa ideia prepara a Aula 11, que tratará ambientes computacionais com mais cuidado. Por enquanto, o essencial é perceber que execução depende de condições externas ao código-fonte. Analisar um problema exige perguntar não apenas "o código está certo?", mas também "em que ambiente ele foi executado?".

## Entrada, processamento e saída na execução

Executar um programa normalmente significa materializar o modelo entrada, processamento e saída estudado na Aula 06. Durante a execução, o programa recebe ou acessa entradas, aplica instruções e regras, produz dados intermediários e gera saídas. A execução é o momento em que a descrição formal do comportamento passa a atuar sobre dados concretos.

As entradas podem vir de usuário, arquivo, banco de dados, mensagem de outro sistema, parâmetro, configuração ou dados já armazenados. O processamento pode validar, calcular, classificar, comparar, consultar, atualizar ou preparar respostas. As saídas podem ser telas, arquivos, registros, mensagens, relatórios, logs, atualizações ou evidências.

Essa conexão é importante porque evita tratar execução como um evento abstrato. Quando alguém diz que um programa executou, a pergunta seguinte deve ser: executou com quais entradas, usando quais regras, em qual ambiente e produzindo quais saídas?

## Erros antes e durante a execução

Erros podem aparecer em momentos diferentes. Podem surgir ao escrever o código, quando a pessoa usa uma forma incompatível com a linguagem. Podem surgir ao traduzir ou analisar o código, quando uma ferramenta tenta preparar o programa e encontra problema. Podem surgir ao iniciar a execução, se o ambiente não possui recurso, permissão ou dependência necessária.

Também podem aparecer durante a execução, quando o programa encontra uma condição inesperada: arquivo ausente, dado fora do esperado, recurso indisponível, permissão negada, falha de comunicação ou situação não tratada. E podem ser percebidos depois da execução, quando alguém analisa a saída e descobre que o resultado está incorreto, incompleto ou inadequado.

Esta aula não substitui a Aula 12, que estudará categorias de erro com mais cuidado. O objetivo agora é preparar uma ideia: "deu erro" não é uma categoria suficiente. É preciso observar em que momento o problema apareceu e que camada está envolvida.

## Erro de sintaxe, erro de tradução, erro de execução e erro lógico

Erro de sintaxe ocorre quando a escrita não respeita a forma exigida por uma linguagem ou ferramenta. É um problema de estrutura formal. A ferramenta não consegue reconhecer corretamente a instrução, a organização ou a expressão usada. Em nível inicial, pode ser entendido como uma falha na forma de escrever.

Erro de tradução ou preparação ocorre quando a ferramenta não consegue transformar, preparar ou aceitar o código para a próxima etapa. Pode estar ligado a problemas detectados no processo de compilação, análise, ligação entre partes ou geração de artefato. O detalhe técnico varia por tecnologia; a ideia central é que o problema aparece antes da execução efetiva.

Erro de execução ocorre quando o programa já está em funcionamento e encontra uma condição que impede ou compromete a continuidade. Erro lógico é diferente: o programa pode estar escrito em forma válida, pode ter sido preparado, pode executar até o fim e ainda produzir resultado errado porque a regra representada está incorreta, incompleta ou mal aplicada. Um programa pode estar formalmente aceitável e operacionalmente perigoso.

## Compilar não significa estar certo

Compilação bem-sucedida significa que o código atendeu a certas regras formais e pôde ser transformado ou preparado. Isso é importante, mas não basta para dizer que o programa está correto. A ferramenta verifica aquilo que ela consegue verificar no nível da linguagem e da preparação. Ela não conhece automaticamente o contrato, a política de desconto, a legislação, a regra comercial ou o acordo operacional da organização.

Um cálculo de desconto pode compilar mesmo usando percentual errado. Uma data de vencimento pode ser calculada com regra incompleta, ignorando feriados ou exceções do contrato. Uma validação cadastral pode aceitar dado indevido porque a regra de duplicidade foi mal pensada. Um relatório pode somar o campo errado e ainda ser gerado sem falha técnica. Um processamento pode ignorar exceção importante e tratar todos os registros como se fossem casos comuns.

Por isso, sistemas reais precisam de revisão, teste, conferência, validação de regra, comparação com resultado esperado e participação de pessoas que entendem o processo. Compilar é uma etapa de preparação; não é prova de aderência ao negócio.

## Executar não significa resolver o problema

Um programa pode executar sem travar e ainda não resolver o problema. Ele pode produzir resultado incorreto, incompleto, inútil ou perigoso. Pode gerar um arquivo aceito tecnicamente, mas com registros errados. Pode exibir uma mensagem, mas não orientar a ação necessária. Pode atualizar dados, mas usar período incorreto. Pode terminar com aparente sucesso e deixar uma divergência para outra área descobrir depois.

Em sistemas corporativos, resultado precisa ser validado contra regras, expectativas, controles, auditoria e consequências reais. Não basta perguntar se "rodou". É preciso perguntar se executou no ambiente certo, com versão certa, entradas certas, regras certas, configurações certas e saídas conferidas.

Essa distinção é uma das mais importantes da formação. Computadores podem executar instruções com grande velocidade. Se a instrução representa mal o problema, a velocidade apenas espalha o erro mais rapidamente.

## Compilação, interpretação e execução em sistemas corporativos

Em um banco, um programa que participa de validação de transações precisa estar na versão correta, executar no ambiente autorizado, receber dados confiáveis de conta e cliente, aplicar regras de limite e registrar evidências. Não basta existir código para validar transações; é preciso garantir que a preparação e a execução aconteçam sob controle, porque o resultado afeta dinheiro, confiança e auditoria.

No governo, uma rotina que calcula ou classifica benefícios precisa usar regras vigentes, dados de cidadãos, documentos e períodos corretos. Se uma versão antiga for executada em produção, cidadãos podem receber decisão errada. Se a execução terminar sem falha técnica, mas aplicar critério desatualizado, o problema aparecerá na consequência social e administrativa.

Em uma seguradora, programas que analisam apólice, cobertura, franquia e documentação precisam ser executados com dados corretos e regras compatíveis com o contrato. Uma preparação correta não garante que a regra de cobertura esteja representada corretamente. A conferência de saídas e evidências é essencial para justificar pagamento, recusa ou pendência.

No comércio, uma rotina de venda, estoque ou faturamento precisa aplicar preço, desconto, regra fiscal e disponibilidade. Um programa pode executar sem travar e ainda baixar estoque errado se a entrada veio duplicada ou se a configuração apontou para local incorreto. A operação precisa controlar saídas para que faturamento, entrega e estoque permaneçam coerentes.

Na folha de pagamento, compilação, interpretação ou execução de rotinas de cálculo precisam ser controladas porque pequenas diferenças de regra podem afetar muitas pessoas. Versão, período de referência, dados de eventos, parâmetros e relatórios de conferência importam tanto quanto o código. Uma execução aparentemente normal pode produzir valores errados se o conjunto de entradas ou regras estiver inadequado.

Em telecom, rotinas de faturamento podem processar consumo, franquia, plano, descontos e ajustes. Se a execução usa dados incompletos, a fatura pode sair errada. Em cobrança, programas podem classificar atraso, calcular juros e gerar avisos; se o ambiente usa política antiga ou arquivo incorreto, o cliente pode receber cobrança indevida. Em contabilidade, processos de fechamento precisam preservar evidências porque valores consolidados dependem de origem, versão e período.

Esses exemplos mostram que não basta ter código. Sistemas corporativos precisam preparar, executar no ambiente correto, conferir entradas, controlar saídas, registrar evidências e preservar capacidade de explicar o resultado.

## Ambientes de desenvolvimento, homologação e produção

Ambiente de desenvolvimento é usado para criar e alterar programas ou componentes. É onde mudanças são esperadas e onde o risco sobre operações reais deve ser menor. Ambiente de teste é usado para verificar comportamento em cenários planejados, com dados e condições voltados a descobrir problemas antes de afetar usuários finais.

Ambiente de homologação aproxima a validação do uso real. Pode envolver áreas de negócio, conferência de regras, comparação com expectativas e aceitação de uma mudança antes de liberação. Ambiente de produção é onde o sistema sustenta operações reais, com dados reais, usuários reais e consequências reais.

Código normalmente não deve ir direto do desenvolvimento para produção porque mudanças precisam ser verificadas. Uma alteração pode compilar, executar em teste simples e ainda falhar em cenário real. Separar ambientes reduz risco, ajuda a controlar versões e permite validar comportamento antes de afetar processos importantes. Esta aula apenas introduz essa separação; a Aula 11 aprofundará ambientes computacionais.

## Controle de versão e rastreabilidade em nível inicial

Organizações precisam saber qual versão de um programa foi usada, quando foi alterada, por quem, com qual objetivo e qual impacto teve. Versão é a identificação de um estado específico de um programa, arquivo, configuração ou componente. Quando versões não são controladas, fica difícil explicar por que um resultado mudou.

Rastreabilidade é a capacidade de acompanhar origem, alteração, execução e resultado. Em sistemas corporativos, pode ser necessário demonstrar que determinada rotina foi executada com certa versão, em certo ambiente, em certo horário, com certos dados e produzindo certas saídas. Isso ajuda suporte, auditoria, investigação, correção e continuidade operacional.

Esta aula não ensina Git, ferramentas de versionamento ou processos de governança. O ponto é conceitual: execução responsável exige memória sobre o que foi executado. Sem controle de versão e rastreabilidade, a organização pode até produzir resultados, mas terá dificuldade para explicar e corrigir problemas.

## Conexão futura com COBOL e Mainframe

Futuramente, o aluno estudará programas COBOL que precisam ser compilados ou preparados para execução em ambientes controlados. Também estudará Mainframe como ambiente corporativo em que programas, arquivos, jobs, controles, evidências e operação aparecem de forma organizada. A compreensão desta aula será pré-requisito para não confundir fonte, preparação, execução e resultado.

Em ambientes Mainframe, a execução de programas costuma estar relacionada a rotinas, arquivos de entrada e saída, parâmetros, ambientes, códigos de retorno, evidências e acompanhamento operacional. Nesta aula, esses termos aparecem apenas como conexão futura. Não é o momento de ensinar COBOL, JCL, comandos, compilação COBOL ou z/OS tecnicamente.

O ponto é formar maturidade: antes de estudar uma tecnologia específica, o aluno precisa entender que programas corporativos não são apenas textos ou telas. Eles são preparados, executados, controlados e analisados dentro de sistemas que lidam com dados importantes e consequências reais.

## Confusões comuns de iniciantes

Uma confusão comum é achar que escrever código é o mesmo que executar. Escrever produz uma representação formal. Executar coloca comportamento em funcionamento. Entre essas duas coisas pode haver análise, tradução, interpretação, preparação, carregamento de ambiente e uso de recursos.

Outra confusão é achar que compilação garante correção. Compilação verifica aspectos formais e prepara o programa. Ela não garante que a regra de negócio foi compreendida, que a fórmula está certa, que o relatório responde à pergunta correta ou que exceções foram tratadas.

Também é comum acreditar que, se executou sem erro visível, então está certo. Um programa pode terminar sem travar e ainda produzir cobrança indevida, relatório distorcido, cadastro inconsistente ou pagamento incorreto. Resultado precisa ser conferido contra expectativa e contexto.

Há quem pense que erro é sempre erro de sintaxe. Sintaxe é apenas uma categoria. Problemas podem aparecer na tradução, no ambiente, na execução, nos dados, na configuração, na regra ou na interpretação da saída.

Outra confusão é imaginar que todo código vira executável da mesma forma. Tecnologias podem usar executáveis, scripts, bytecode, máquinas virtuais, interpretadores e runtimes. O caminho depende da linguagem, da ferramenta e do ambiente.

Também aparece a ideia de que interpretado significa menos sério. Isso é uma simplificação. Sistemas importantes podem usar mecanismos interpretados ou mistos. Seriedade depende de controle, clareza, teste, ambiente, operação e adequação ao problema.

Muitos iniciantes ignoram o ambiente de execução. Eles olham apenas para o código e esquecem permissões, arquivos, configurações, versões, dados disponíveis e dependências. O mesmo código pode se comportar de modo diferente quando essas condições mudam.

Ignorar entradas e configurações é outra falha. Uma execução depende do que recebe e do que encontra. Entrada errada, parâmetro errado ou configuração incorreta pode produzir saída ruim mesmo quando o programa foi preparado corretamente.

Há ainda a confusão de ignorar versão. Se duas versões diferentes existem, dizer "o programa rodou" é insuficiente. É preciso saber qual versão rodou. Por fim, muitos não diferenciam programa armazenado de programa em execução. O arquivo guardado é uma possibilidade; a execução é a atividade real acontecendo.

## Perguntas para reflexão

- Por que um arquivo de código-fonte salvo em uma pasta não está automaticamente executando?
- O que muda quando um programa deixa de estar armazenado e passa a estar em execução?
- Que tipo de problema a compilação consegue detectar e que tipo de problema ela não consegue garantir?
- Como um programa pode executar sem travar e ainda produzir resultado incorreto?
- Por que ambiente, entrada, configuração e versão precisam ser considerados ao analisar uma execução?
- Em que situações uma saída técnica pode existir, mas não resolver a necessidade do negócio?
- Por que sistemas corporativos precisam preservar evidências de execução?
- Como esta aula ajuda a preparar o estudo futuro de arquivos, ambientes, erros, COBOL e Mainframe?

## Síntese da aula

Código-fonte não é execução. Ele é uma representação textual formal de um programa. Para que produza comportamento, precisa ser analisado, traduzido, interpretado, preparado ou conduzido por mecanismos apropriados, dentro de um ambiente computacional. Esse ambiente oferece recursos, permissões, configurações, arquivos, dados e componentes necessários para a execução.

A aula diferenciou compilação, interpretação e execução em nível conceitual. Compilação pode preparar ou traduzir código-fonte para outra forma. Interpretação conduz instruções por meio de um mecanismo mediador. Execução é o momento em que o comportamento acontece, consumindo recursos e produzindo efeitos. Também vimos que modelos mistos existem, com bytecode, máquinas virtuais, runtimes e diferentes formas de preparação.

Um dos pontos centrais é que compilar não significa estar correto, e executar sem travar não significa resolver o problema. Sistemas corporativos exigem controle de versão, ambiente, entradas, saídas, evidências e validação de resultados. A próxima aula estudará arquivos, pastas, formatos e extensões, aprofundando a ideia de que código-fonte, executáveis, scripts, configurações, entradas, saídas e resultados normalmente existem como arquivos organizados em algum armazenamento.

## Mini glossário da aula

**Compilação**: processo de tradução ou transformação de código-fonte para uma forma preparada para execução ou uso por outro ambiente.

**Compilador**: ferramenta que analisa código-fonte e tenta transformá-lo em uma forma preparada, apontando problemas quando não consegue.

**Interpretação**: condução de instruções por um mecanismo que lê e executa ou orienta a execução de código de forma mediada.

**Interpretador**: mecanismo capaz de ler instruções em determinada linguagem ou forma reconhecida e conduzir sua execução.

**Execução**: momento em que o comportamento de um programa efetivamente acontece, usando recursos e processando dados.

**Executável**: forma preparada de um programa que pode ser colocada em execução por ambiente compatível.

**Script**: texto de instruções conduzido por interpretador ou ambiente adequado, frequentemente usado para automação ou tarefas orientadas por texto.

**Bytecode**: forma intermediária gerada por algumas tecnologias entre o código-fonte e a execução final.

**Máquina virtual**: mecanismo que oferece uma camada de execução para certos programas ou formatos intermediários.

**Runtime**: conjunto de componentes necessários para que um programa execute em determinada tecnologia.

**Ambiente de execução**: conjunto de condições, recursos, permissões, configurações e componentes disponíveis durante a execução.

**Programa armazenado**: programa preservado em arquivo ou artefato, sem necessariamente estar ativo.

**Programa em execução**: programa cujo comportamento está em andamento em um ambiente computacional.

**Processo**: instância ativa de um programa em execução, com recursos e contexto associados.

**Erro de sintaxe**: erro na forma de escrita de uma instrução ou estrutura em relação às regras da linguagem.

**Erro de tradução**: erro percebido durante preparação, compilação ou transformação do código para outra forma.

**Erro de execução**: erro que aparece enquanto o programa está em funcionamento.

**Erro lógico**: erro em que o programa pode executar, mas representa regra ou raciocínio incorreto.

**Desenvolvimento**: ambiente ou etapa em que programas são criados e alterados.

**Teste**: ambiente ou etapa usada para verificar comportamento antes de uso real.

**Homologação**: validação mais próxima do uso real, frequentemente com conferência da área responsável.

**Produção**: ambiente em que sistemas sustentam operações reais.

**Versão**: identificação de um estado específico de um programa, arquivo, configuração ou componente.

**Rastreabilidade**: capacidade de acompanhar alterações, versões, execuções, entradas, saídas e responsáveis.

## Critérios de domínio

Depois de estudar esta aula, o aluno deve conseguir explicar por que código-fonte não é o mesmo que execução. Deve diferenciar um arquivo de código armazenado de um programa em funcionamento, reconhecendo que execução envolve recursos, ambiente, dados e efeitos.

O aluno deve diferenciar compilação, interpretação e execução em nível conceitual. Também deve explicar o papel de compilador, interpretador, máquina virtual, runtime e ambiente de execução sem transformar esses conceitos em prática de ferramenta.

Também é esperado que o aluno compreenda que compilar não significa estar correto e que executar sem travar não significa resolver o problema. Deve reconhecer que erro pode aparecer antes da execução, durante a execução ou depois, quando o resultado é analisado.

O aluno deve diferenciar erro de sintaxe, erro de tradução, erro de execução e erro lógico em nível inicial. Deve explicar por que entrada, dados, regras, configuração, versão e ambiente influenciam o comportamento observado.

Por fim, deve conectar o tema com programas, sistemas corporativos, COBOL e Mainframe futuramente. O domínio esperado é perceber que sistemas reais precisam controlar preparação, execução, versão, evidências, entradas e saídas antes de avançar para arquivos, ambientes computacionais e categorias de erro.

## Referências e leituras para aprofundamento

- Oracle. *The Java Virtual Machine Specification*.
- Python Software Foundation. *Python Language Reference — Execution model*.
- LLVM Project. *LLVM Language Reference Manual*.
- ACM, IEEE Computer Society e AAAI. *Computer Science Curricula 2023*.
