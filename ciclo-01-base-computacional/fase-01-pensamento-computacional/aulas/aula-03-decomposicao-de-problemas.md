# Aula 03 — Decomposição de problemas

## Metadados

- **Ciclo:** 1 — Base Computacional
- **Fase:** 1 — Pensamento Computacional
- **Subtítulo da fase:** De problemas informais a soluções estruturadas
- **Posição:** terceira de 14 aulas
- **Competência central:** C03 — decompor e recompor problemas preservando relações relevantes
- **Nível trabalhado:** Nível 2, Nível 3 e início do Nível 4 em caso simples
- **Pré-requisitos:** Aulas 01 e 02; noções de sistema, componente, fronteira, entrada, saída, processamento e interface da Fase 0
- **Prática associada:** `../praticas/pratica-03-decompondo-problemas.md`
- **Projeto integrado:** conclusão do marco P1 com a decomposição do problema de estoque

## Introdução e definição

### Objetivo da aula

Ao concluir esta aula, você deverá conseguir dividir um problema formulado em partes administráveis segundo um critério declarado, reconhecer relações e dependências entre essas partes, avaliar granularidade, cobertura, sobreposição e lacunas e, por fim, recompor o conjunto para verificar se o problema original continua atendido.

O resultado esperado não é uma lista longa nem um desenho sofisticado. É uma decomposição justificável: outra pessoa deve conseguir identificar qual era o todo, para que ele foi dividido, por que cada parte existe, o que atravessa as fronteiras entre partes e como verificar o conjunto novamente.

### O problema que esta aula resolve

Uma formulação pode estar correta e ainda ser grande demais para orientar análise e ação. “Reduzir atendimentos incompletos sem aumentar perdas nem custo” reúne contagem, disponibilidade, regras, decisões, registros e operação. Tratar tudo de uma vez favorece omissões, responsabilidades confusas, regras incompatíveis, duplicidade, intervenção prematura e dificuldade de verificar ou explicar resultados.

Decompor concentra atenção, distribui investigação e localiza dependências. Também pode omitir partes, duplicar responsabilidades, favorecer decisões locais e apagar relações. A divisão só ajuda quando preserva o problema de origem.

### Ponte com a Aula 02 e com a Fase 0

A Aula 02 estabeleceu o problema como objeto delimitado e revisável de análise, que pode envolver diferença, obstáculo, risco, incerteza, decisão, necessidade ou oportunidade. Objetivo, estados, escopo, fronteira, restrições, critérios e questões abertas formam o **todo de partida**. Se ele estiver vago, a decomposição apenas distribuirá a vagueza.

Da Fase 0, recuperamos a noção de sistema como conjunto de componentes relacionados que opera com algum propósito. Recuperamos também que uma interface é uma relação ou um ponto de interação pelo qual algo relevante atravessa a fronteira entre partes, e não apenas uma tela. Essas ideias ajudam a reconhecer que dividir não significa isolar completamente. Entradas, saídas, informação, materiais, decisões, regras e mudanças de estado podem atravessar a fronteira escolhida.

Esta retomada é funcional. Não estamos projetando software, definindo componentes técnicos nem escrevendo programas. “Processo”, nesta aula, designa principalmente uma atividade organizacional ou transformação do domínio; não é a instância ativa de um programa estudada na Fase 0. Uma função do problema também não é, por si só, uma unidade de software.

### Caso de abertura — quando seis itens ainda não explicam o problema

Considere a formulação construída na Aula 02:

> Nos três produtos e dois centros incluídos, 192 de 2.400 linhas não foram atendidas integralmente na primeira separação em 28 dias: 6% no CD Norte e 10,8% no Sul. Pretende-se reduzir a ocorrência de modo sustentado, protegendo perdas, custo, divergências e outros produtos. A taxa inferior a 3% por centro em três ciclos é meta candidata. Permanecem abertos comparabilidade da contagem, qualidade dos registros, impacto, relações causais, linhas de base das proteções e autoridade sobre a meta. Estoque adicional, redistribuição, correção de registros e previsão são alternativas não avaliadas.

Há vários focos possíveis: observar demanda, verificar posição, acompanhar entradas, tratar separação, registrar ocorrências, avaliar resposta e controlar efeitos. Uma equipe, porém, escreve apenas “compras, depósito, sistema, pessoas, transporte, clientes”. Essa enumeração mistura áreas, meios e interessados, não declara critério, cobertura ou relações. A presença de “sistema” tampouco demonstra causa.

A pergunta correta não é “quantos itens foram escritos?”, e sim: **esta divisão ajuda a responder ao propósito declarado e permite reconstruir o todo sem inventar certeza?**

### Definição operacional de decomposição

Nesta fase, adotaremos a seguinte definição operacional:

> **Decomposição de problemas é a divisão intencional de um todo formulado em partes administráveis, segundo um critério declarado, preservando as relações, dependências, restrições, responsabilidades, interfaces e propriedades necessárias para que o todo possa ser recomposto e avaliado.**

Cada termo da definição tem função:

- **intencional:** a divisão serve a uma pergunta ou decisão; não é fragmentação por hábito;
- **todo formulado:** existe uma referência comum contra a qual cobertura e resultado serão verificados;
- **critério declarado:** sabemos se dividimos por funções, informações e objetos do domínio, etapas ou outro princípio;
- **partes administráveis:** cada parte permite investigação ou decisão mais focada;
- **preservação:** relações e restrições não somem apenas porque traçamos fronteiras;
- **recomposição:** voltamos a perguntar se o conjunto ainda responde ao problema original.

Essa é uma convenção pedagógica útil, não uma definição universal nem uma receita infalível. Problemas diferentes admitem decomposições diferentes; a mesma decomposição pode ser útil para uma finalidade e inadequada para outra. A atividade é iterativa: compreender uma parte pode levar à revisão da fronteira, do nível de detalhe ou até da formulação do todo.

Decompor também não equivale a implementar. Uma boa decomposição pode orientar investigação feita por pessoas, comparação de alternativas, coleta de evidências ou organização de uma decisão. Nenhuma parte precisa virar programa, tela ou arquivo.

### Todo, parte e termos próximos

Precisão de vocabulário evita que palavras parecidas ocultem decisões diferentes.

| Termo | Uso nesta aula | Pergunta de controle |
|---|---|---|
| **Todo** | problema formulado que será dividido e depois reavaliado | Que resultado comum não pode ser perdido? |
| **Parte** | recorte identificável obtido segundo o critério escolhido | Que parcela do todo este recorte cobre? |
| **Subproblema** | questão menor cuja resolução contribui para o problema maior | Há algo local a compreender ou resolver, sem esquecer o todo? |
| **Função** | contribuição ou transformação necessária ao resultado | O que precisa ser realizado? |
| **Tarefa** | ação delimitada executada em um contexto | Quem ou o que faz qual ação? |
| **Etapa** | período ou posição reconhecível no percurso do caso | Em que momento do percurso estamos? |
| **Componente** | elemento identificável de um sistema ou solução | De qual sistema e segundo qual fronteira ele é componente? |
| **Responsabilidade** | obrigação de cuidar de um resultado, decisão ou informação | Quem responde por quê, com qual limite? |

Uma parte não é automaticamente um subproblema. “Documento da solicitação” pode ser um objeto do domínio, enquanto “reduzir documentos inválidos sem excluir solicitantes” pode ser um subproblema. Uma função não é automaticamente uma tarefa: “validar elegibilidade” expressa uma contribuição; “analista confere o comprovante” descreve uma ação mais localizada. Uma etapa não é necessariamente um componente permanente, e responsabilidade não é sinônimo de departamento.

Os rótulos devem ser acompanhados de uma frase de escopo. “Validação” é ambíguo; “verificar se os documentos mínimos estão presentes sem decidir a elegibilidade” torna a fronteira observável. O objetivo não é decorar categorias, mas impedir que palavras genéricas substituam o raciocínio.

## Critérios e formas de decomposição

### Decomposição não é enumeração, classificação ou desenho de solução

Atividades próximas podem apoiar a análise, mas não devem ser confundidas.

| Atividade | O que faz | Por que não basta como decomposição |
|---|---|---|
| **Enumeração** | reúne itens lembrados | pode não ter critério, cobertura nem relações |
| **Classificação** | agrupa itens por semelhança | organiza ocorrências, mas não necessariamente divide o problema |
| **Sequenciamento** | ordena ações ou eventos | ordem temporal não mostra todas as dependências e responsabilidades |
| **Divisão de trabalho** | atribui atividades a pessoas ou equipes | a estrutura organizacional pode duplicar ou omitir partes do problema |
| **Desenho de solução** | propõe como intervir | pode fechar alternativas antes de compreender o todo e as partes |
| **Arquitetura técnica** | organiza elementos de uma solução construída | pertence a decisões posteriores e não é consequência automática desta análise |

Imagine a lista “cadastro, prioridade alta, prioridade média, pagamento, reclamação”. Ela mistura uma possível função, classes, uma etapa e uma ocorrência. Separar os itens em colunas melhora a classificação, mas ainda precisamos declarar o todo, escolher um critério principal, explicitar o escopo das partes e registrar suas dependências.

Também é possível ter uma sequência sem decomposição adequada: “receber, executar a atividade de análise, registrar uma conclusão” informa três momentos, porém não revela quais informações orientam a atividade, que ato autoriza o registro do resultado, o que ocorre diante de pendência nem como uma restrição de privacidade atravessa as etapas. E é possível decompor sem ordenar: uma visão por informações e objetos do domínio pode considerar solicitação, documento, registro da decisão e comunicação emitida sem afirmar uma ordem única.

### Critério e propósito orientam a divisão

O critério responde **segundo que aspecto o todo será dividido**. O propósito responde **para que essa visão será usada agora**. Ambos devem aparecer antes das partes.

Se o propósito é descobrir responsabilidades ausentes, uma decomposição funcional pode ser produtiva. Inconsistências de significado favorecem informações e objetos do domínio; espera e retorno favorecem etapas e eventos. Outros propósitos podem justificar localidades, responsabilidades, categorias de regras ou tipos de exceção. Nenhum critério é superior em abstrato.

Um critério principal dá coerência ao primeiro nível. Misturas são possíveis quando justificadas, mas devem ser visíveis. “Receber solicitação”, “documento”, “equipe regional” e “após cinco dias” pertencem a critérios diferentes. Colocá-los como partes equivalentes dificulta comparar cobertura e dependências. Uma saída é escolher funções no primeiro nível e, dentro de uma função específica, usar objetos ou etapas em um segundo nível.

O artigo histórico de David Parnas sobre critérios de decomposição mostra uma lição que permanece útil fora do projeto de software: dividir segundo passos de processamento não é a única escolha, e princípios diferentes expõem preocupações diferentes. Nesta aula, usamos somente essa lição sobre a importância do critério; as conclusões de projeto de módulos ficam para uma etapa posterior da formação.

### Decomposição funcional

A decomposição funcional pergunta: **quais contribuições ou transformações precisam existir para que o resultado do todo seja alcançado?** Seus rótulos costumam combinar verbo e objeto, como “receber solicitação”, “verificar completude”, “decidir elegibilidade”, “comunicar decisão” e “tratar contestação”.

Funções devem expressar resultados do domínio, não nomes vagos de áreas. “Financeiro” pode ser uma unidade organizacional; “autorizar pagamento conforme decisão válida” expressa a função relevante. A pessoa ou equipe responsável pode ser registrada separadamente. Essa separação permite perceber que uma função atravessa duas equipes ou que uma equipe executa várias funções.

Uma boa decomposição funcional ajuda a verificar responsabilidades, entradas e resultados parciais. Ela não determina ordem completa, causalidade ou partes técnicas. Funções amplas, duplicadas ou vagas podem esconder informações; copiar a solução ou os departamentos atuais cristaliza seus defeitos. “Ler o campo” e “clicar em confirmar” podem ser detalhes prematuros.

Teste funcional inicial: se uma parte desaparecer, qual contribuição necessária deixa de ocorrer? Se nada relevante mudar, o rótulo pode ser detalhe, meio ou duplicação. Se o efeito sobre o todo não puder ser explicado, o escopo da função ainda está vago.

### Decomposição por informações e objetos do domínio

Esta decomposição pergunta: **sobre quais informações e objetos do domínio precisamos raciocinar separadamente?** Antes de formar as partes, distinga categorias que podem aparecer juntas no caso:

| Categoria | Uso nesta aula | Exemplo no benefício |
|---|---|---|
| **objeto do domínio** | algo cuja identidade ou condição importa ao problema | pessoa solicitante, solicitação, documento, contestação |
| **dado** | valor ou símbolo cuja interpretação depende de contexto | `20/06` ou “recebido”, ainda ambíguos sem referência |
| **informação** | representação com significado sobre um objeto ou ocorrência | condição documental, estado da solicitação, prazo registrado |
| **registro** | evidência ou armazenamento de informação | pendência registrada, registro da análise, decisão registrada |
| **atividade** | transformação realizada no domínio | analisar elegibilidade, decidir, emitir comunicação |
| **resultado** | efeito ou produto de uma atividade | conclusão da análise, decisão autorizada, comunicação emitida |

Um **documento** é um artefato delimitado que contém informação registrada; sua identidade e condição podem torná-lo também objeto do domínio no recorte. “Análise” e “decisão”, sem qualificação, podem nomear atividade, resultado ou registro. Por isso, escreva **atividade de análise**, **conclusão ou registro da análise**, **ato de decidir** e **resultado ou registro da decisão**, conforme o significado pretendido.

O objetivo aqui não é construir um modelo técnico de dados. Não definiremos campos, chaves, tabelas, formatos de armazenamento nem estruturas de software. A pergunta é analítica: de que objeto se fala, que informação o representa, qual registro a evidencia, quem a usa, quando muda, que regra a restringe e que inconsistência afetaria outras partes?

Esse critério é útil quando uma mesma informação ou seu registro percorre várias funções, ou quando nomes iguais escondem significados distintos. “Data da solicitação”, “data de recebimento completo” e “data do registro da decisão” não são intercambiáveis. A divisão por informações e objetos pode revelar que uma métrica de prazo depende de qual marco foi registrado, sem concluir que o registro explica causalmente o atraso.

O risco é produzir um inventário de substantivos, copiar tabelas existentes, confundir registro com objeto do domínio, duplicar conceitos ou ignorar atividades e resultados. Fronteiras não são óbvias. Registre papel e interação: “documento apresentado — objeto cuja condição informada sustenta a verificação e pode motivar complementação” é melhor que “documentos”.

### Decomposição por etapas e eventos

A decomposição por etapas acompanha **períodos reconhecíveis do percurso**, enquanto eventos registram **ocorrências que iniciam, alteram ou encerram uma condição relevante**. No caso do benefício, etapas possíveis são entrada, preparação da atividade de análise, ato de decidir, emissão da comunicação e pós-decisão. Eventos possíveis incluem recebimento da solicitação, identificação de pendência, chegada de complemento, registro de decisão e apresentação de contestação.

Uma etapa pode durar e conter várias atividades. Um evento marca uma ocorrência; não precisa ter duração significativa. Essa diferença ajuda a evitar rótulos híbridos como “análise aprovada”, que podem confundir o período de analisar com o evento de registrar uma decisão.

Esta visão localiza esperas, retornos e mudanças de estado, mas não é algoritmo nem fluxo formal. Casos podem ocorrer em paralelo, repetir ou seguir condições. A descrição atual não é solução ideal; etapas podem esconder responsabilidades, ignorar estados ou relegar exceções a “outros”. Uma lista vertical não prova dependência entre itens.

O registro deve manter o nível organizacional do problema. Não se desenham símbolos de fluxograma, não se especifica pseudocódigo e não se decide como automatizar as etapas.

### Três decomposições do mesmo problema

Considere o problema “reduzir solicitações que permanecem sem ação após documentação completa, preservando correção, tratamento justo e direito de contestação”. Três critérios produzem três recortes legítimos:

| Critério | Pergunta e tipo de parte | Relação evidenciada | Vantagem | Risco | Uso provável |
|---|---|---|---|---|---|
| funções | o que precisa ocorrer? contribuições | entradas e resultados | localizar responsabilidades | verbos vagos | auditar capacidades ausentes |
| informações e objetos do domínio | sobre o que precisamos manter significado? objetos, informações e registros | produção, uso e mudança | localizar divergências | copiar estruturas existentes | investigar significados |
| etapas/eventos | em que momentos? períodos e ocorrências | precedência, espera e retorno | acompanhar percursos | presumir linearidade | localizar interrupções |

As decomposições não competem para revelar uma verdade única. Elas respondem a perguntas diferentes. Compará-las permite notar pontos cegos: uma função sem objeto necessário, um objeto sem responsável, uma etapa sem condição de saída ou um evento sem consequência conhecida.

Combinar visões não significa despejar todas as partes numa só lista. Mantenha cada critério legível e construa correspondências pontuais: a função “verificar completude” consulta a solicitação e os documentos durante a etapa de preparação; o evento “pendência identificada” altera a condição da solicitação e exige comunicação. Essa correspondência já prepara a recomposição.

## Estrutura das partes

### Hierarquia e níveis de decomposição

Uma parte pode ser dividida novamente, criando níveis. No primeiro nível funcional do benefício, “tratar pendência” é uma parte. Em um segundo nível, ela pode conter “registrar itens pendentes”, “informar a pessoa solicitante” e “receber complementação”. A hierarquia torna explícito que essas três contribuições pertencem àquela parte, e não diretamente ao todo no mesmo nível das demais funções.

Representação textual simples:

- todo: conduzir a solicitação até uma decisão válida e comunicada;
  - verificar suficiência documental;
  - tratar pendência;
    - registrar a pendência;
    - comunicar itens e prazo;
    - receber e associar complementação;
  - analisar elegibilidade;
  - produzir decisão autorizada;
  - comunicar decisão e direito de contestação.

Níveis não indicam importância, autoridade ou ordem temporal. Uma parte de segundo nível pode ser crítica; duas partes irmãs podem interagir; uma restrição pode atravessar toda a árvore. A estrutura apenas registra inclusão segundo uma escolha analítica.

Herbert Simon mostrou que muitos sistemas complexos podem ser examinados por hierarquias, sem apagar interações nem a escolha do nível. Isso não cria árvore natural, perfeita ou única: uma parte pode depender de várias outras, e um mapa de dependências complementa a árvore.

### Granularidade e critérios de parada

**Granularidade** é o grau de detalhe das partes. “Processar benefício” é grosseiro demais para distinguir verificação, decisão e comunicação. “Posicionar o cursor no primeiro caractere” é fino demais para a pergunta organizacional. O nível adequado é relativo ao propósito, à evidência disponível e à próxima decisão.

Considere parar de decompor quando a parte:

1. tem finalidade, fronteira, entradas e resultados compreensíveis;
2. pode ser investigada ou avaliada com evidência disponível ou obtenível;
3. possui relações relevantes identificáveis com outras partes;
4. permite atribuir responsabilidade analítica sem fingir isolamento;
5. possui nível adequado à decisão, ao público e à atividade atuais;
6. perderia significado ou introduziria detalhe prematuro se fosse dividida novamente.

Considere continuar quando o rótulo ainda reúne objetivos conflitantes, quando ninguém consegue explicar o resultado parcial, quando uma dependência importante fica escondida ou quando ocorrências diferentes são tratadas como uma coisa só. “Analisar e aprovar” pode exigir separação porque recomendar uma conclusão e autorizar uma decisão envolvem responsabilidades distintas. Em outro recorte, essa separação pode ser desnecessária.

Não pare apenas porque cada parte cabe a uma pessoa, dura um dia ou possui certo número de palavras. Esses limites podem servir ao planejamento do trabalho, mas não provam adequação analítica. Tampouco decomponha indefinidamente: mais partes aumentam o custo de manter consistência e de recompor.

Uma verificação prática é subir e descer um nível. Ao descer, cada parte filha explica uma contribuição da parte mãe? Ao subir, as partes irmãs permitem explicar o resultado da parte mãe? Se a resposta falhar, pode haver lacuna, mistura de critérios ou granularidade incompatível.

## Dependências e interfaces

### Relações, dependências e ordem

Uma **relação** conecta partes; uma **dependência** existe quando uma parte requer algo de outra sob alguma condição. **Precedência** indica antes/depois; **compartilhamento**, uso comum; **influência**, efeito possível ainda a investigar; **restrição transversal**, limite aplicado a várias partes. Elas não são sinônimos.

Algumas naturezas úteis são:

- **informação:** a atividade de análise precisa conhecer documentos recebidos e regras vigentes;
- **ordem:** o resultado de uma decisão individual só pode ser comunicado depois de autorizado;
- **recurso:** duas partes disputam a mesma equipe, sala ou janela operacional;
- **decisão:** o pagamento depende do registro de decisão válida, não apenas de recomendação;
- **regra:** atividade de análise e contestação precisam interpretar a mesma regra aplicável;
- **estado:** a retomada depende de a pendência ter mudado de aberta para atendida ou encerrada.

Essa lista não é taxonomia rígida. Uma dependência pode combinar naturezas: comunicação depende da decisão por informação e autorização. Registre **o que é requerido, por quem, em qual condição e com que consequência se faltar**.

Ordem e dependência não são sinônimos. Entrevistas de terça e quarta podem ser apenas agenda; análises paralelas podem depender da mesma regra. Dependência pode ser condicional, e um evento pode reabrir parte anterior. Teste: alterar a ordem muda necessariamente a validade? Retirar o item fornecido impede a contribuição?

Também não confunda dependência com causa. “A atividade de análise recebe o registro de documentos” não afirma que o registro causou um atraso. Setas entre partes precisam de rótulo; uma seta muda de significado quando representa “fornece informação”, “requer autorização”, “restringe” ou “ocorre antes”.

### Interfaces e mapa inicial de dependências

Nesta aula, **interface** é a relação ou o ponto de interação pelo qual informação, material, decisão, regra ou mudança de estado atravessa a fronteira entre partes. Uma tela é apenas uma possível manifestação futura; interface não significa necessariamente tela, API ou especificação técnica.

Para registrar uma interface inicial, pergunte:

- o que a parte recebe, de quem, em qual condição e com qual significado;
- o que produz, para quem e com qual significado;
- que erro, ausência ou ambiguidade pode atravessar a fronteira.

Exemplo: “verificação documental → atividade de análise: condição dos documentos e pendências encerradas; a atividade precisa distinguir ‘recebido’ de ‘legível e disponível’; se essa distinção faltar, casos podem ser analisados com base incompleta”. O registro é analítico. Não define formato, protocolo ou implementação.

Um mapa simples pode ser uma tabela:

| Origem → destino | Relação ou conteúdo | Condição | Consequência da ausência |
|---|---|---|---|
| atividade de análise → ato de decidir | conclusão e regras aplicadas | requer papel autorizado | não há decisão válida |
| registro da decisão → emissão da comunicação | resultado, fundamento e prazo | após autorização | interessado não conhece resultado ou direito |
| contestação → atividade de reanálise | alegação e eventual nova evidência | se contestação admissível | revisão pode usar base incompleta |

Esse mapa não é fluxo, algoritmo nem teoria de grafos. Retornos e circularidades precisam ser examinados; ausência de seta não prova independência; o mapa deve ser revisto na recomposição.

## Cobertura, sobreposição e lacunas

### Cobertura e matemática introdutória

Cobertura pergunta se as partes, tomadas em conjunto, alcançam os aspectos relevantes do todo **no escopo e para o propósito declarados**. Não promete cobrir toda a realidade. Se o recorte é a primeira decisão sobre três produtos em dois centros, transporte posterior e todos os demais produtos podem estar legitimamente fora, desde que a exclusão e os riscos de transferência permaneçam registrados.

Como formalização didática simplificada, use conjuntos; nem toda decomposição real cabe integralmente neles, e a notação não representa sozinha dependências, interfaces ou propriedades do todo. Seja `W` o conjunto dos aspectos relevantes **para o escopo, o propósito e um único critério declarados**, e sejam `P₁, P₂, ..., Pₙ` os escopos das partes, com `Pᵢ ⊆ W`. Se escopo, propósito ou critério mudarem, `W` precisa ser revisto em vez de receber partes de visões diferentes. Há cobertura quando:

`P₁ ∪ P₂ ∪ ... ∪ Pₙ = W`

O símbolo `⊆` significa “está contido em”; `∪` significa união, isto é, tudo o que aparece em pelo menos uma parte; `=` afirma que essa reunião corresponde ao conjunto de aspectos relevantes definido como `W`. A igualdade não é selo automático de qualidade nem prova que `W` foi bem definido: depende de termos claros, de um recorte justificável e de verificação contra o caso.

Exemplo funcional: se `W` inclui receber, verificar, decidir, comunicar e tratar contestação, uma divisão que omite comunicação não cobre `W`. Adicionar “outros” pode esconder a lacuna, não resolvê-la. A correção exige nomear a contribuição ausente ou justificar que ela está fora do escopo.

Não reúna na mesma igualdade partes funcionais, partes por informações e objetos do domínio e etapas como se fossem conjuntos equivalentes. Cada critério recorta o todo de forma diferente. A comparação entre critérios é argumentativa: verificamos o que cada visão torna visível e onde uma complementa a outra.

### Sobreposição, lacunas e elementos transversais

Duas partes distintas se sobrepõem quando seus escopos compartilham algum aspecto. Para `i ≠ j`, em notação:

`Pᵢ ∩ Pⱼ ≠ ∅`

`∩` significa interseção, o que é comum às partes; `≠` significa diferente; `∅` representa o conjunto vazio. Portanto, a expressão diz que existe ao menos um aspecto comum.

Uma **partição estrita** de `W` exige cobertura, partes não vazias e partes disjuntas duas a duas: para qualquer `i ≠ j`, `Pᵢ ∩ Pⱼ = ∅`. Essa estrutura é útil em classificações que exigem um único grupo por item. Decomposição e partição, portanto, não são sinônimos: decomposições sociotécnicas não precisam ser partições estritas. Privacidade pode restringir recebimento, atividade de análise, ato de decidir e emissão da comunicação; a regra vigente pode ser consultada na análise e na contestação. Esse alcance transversal é legítimo quando a responsabilidade e o efeito em cada parte estão claros.

Sobreposição torna-se **duplicidade problemática** quando duas partes executam ou decidem a mesma coisa sem coordenação, produzem versões incompatíveis ou deixam incerto quem responde pelo resultado. Se a atividade de análise e o ato de decidir alteram independentemente a interpretação da regra, há risco de conclusões divergentes. Se ambos precisam consultar a mesma regra controlada, há sobreposição legítima de dependência.

Uma **lacuna** é aspecto necessário do todo que nenhuma parte cobre, ou relação necessária que ninguém preserva. Às vezes todas as atividades aparentes estão listadas, mas ninguém é responsável por informar uma decisão; em outras, as partes existem, mas o significado de “documento recebido” muda ao atravessar a fronteira.

Audite: o que ficou sem parte? o que se repete e por quê? o que atravessa várias partes? Para cada elemento transversal, registre onde se aplica, quem responde e como será verificado. Lacuna pode revelar divisão incompleta, fronteira inadequada, pressuposto oculto ou problema mal formulado.

## Recomposição e validação

### Recomposição do todo

Recompor não é colar listas. É construir um argumento de que as contribuições parciais, suas interfaces e suas restrições podem sustentar novamente o objetivo global. A recomposição precisa responder:

1. todas as partes contribuem e, juntas, cobrem o todo declarado?
2. resultados parciais são compatíveis entre si?
3. dependências possuem origem, destino, condição e significado suficientes?
4. restrições e critérios de proteção continuam válidos através das fronteiras?
5. alguma propriedade do todo se perdeu ao otimizar uma parte?
6. questões abertas que afetam o conjunto permanecem visíveis?

No benefício, não basta verificar documentos, analisar e decidir localmente. O conjunto precisa preservar prazo total, aplicação coerente das regras, rastreabilidade, confidencialidade, acesso não digital e possibilidade de contestação. Uma conclusão tecnicamente correta que nunca é comunicada não recompõe o resultado “decisão válida e conhecida pelo interessado”.

A falha de recomposição traz informação. Pode revelar parte ausente, granularidade desigual, interface ambígua ou critério inadequado. Também pode indicar que o problema original ainda está mal formulado. Nesse caso, voltar à Aula 02 não é retrocesso: é revisão disciplinada do todo à luz do que as partes mostraram.

### Otimização local, propriedades do todo e iteração

**Otimização local** ocorre quando uma parte melhora sua própria medida e prejudica o resultado comum. Uma equipe pode reduzir o tempo de análise devolvendo imediatamente todo caso duvidoso. Sua fila diminui, mas o tempo total, a carga do atendimento e a desigualdade de acesso podem piorar. Uma parte pode cumprir sua meta e o problema permanecer.

Como nos sistemas da Fase 0, algumas propriedades dependem das relações: tempo total, consistência, confiança, rastreabilidade, capacidade, segurança e impacto. Elas não resultam da soma automática de métricas locais; cada resultado parcial precisa voltar a um critério global e a uma proteção.

O ciclo é: decompor, examinar, mapear relações, tentar recompor, localizar lacunas e sobreposições, revisar fronteira, critério ou granularidade e decompor novamente se necessário. Falhar na recomposição é evidência diagnóstica. Os processos de ciclo de vida organizados pela ISO/IEC/IEEE 15288:2023 admitem aplicação iterativa e concorrente ao sistema e recursiva aos seus elementos; Pólya associa decompor, recombinar e revisar. Nenhuma fonte transforma o ciclo em receita universal.

## Aplicação aos casos

### Caso progressivo — três decomposições do estoque

O **todo** não é “o estoque da empresa”. É o problema formulado sobre linhas não atendidas integralmente na primeira separação, nos três produtos, dois centros e 28 dias, com objetivo, proteções e incertezas já declarados. Usaremos três critérios sem alterar silenciosamente esse recorte.

**Visão funcional:**

| Parte | Contribuição para o todo | Dependência destacada |
|---|---|---|
| registrar demanda e atendimento | preservar o que foi pedido e o que foi atendido | requer critério comparável entre centros |
| manter posição de estoque | registrar saldos e movimentos pertinentes | depende de movimentos completos e significado comum |
| avaliar disponibilidade para separação | relacionar informações candidatas, mantendo a definição aberta | depende de posição, regras e condição física |
| separar e registrar resultado | atender a linha e registrar atendimento incompleto | fornece ocorrência para medição |
| tratar divergências | investigar diferenças entre registro e situação observada | requer histórico e evidência local |
| avaliar resposta | comparar alternativas sem assumir solução | depende de métricas globais e autoridade decisória |
| autorizar eventual resposta | registrar decisão legitimada | depende de avaliação e autoridade ainda aberta |
| acompanhar resultados e efeitos | comparar ciclos e critérios de proteção | depende de registros posteriores comparáveis |

**Visão por informações e objetos do domínio:** os objetos incluem pedido, linha, produto, centro, movimento de estoque identificado como objeto transacional e ocorrência registrada de atendimento incompleto; as informações e seus registros incluem posição registrada, quantidade física observada, condição de disponibilidade ainda aberta, registro da avaliação, decisão autorizativa registrada e indicadores posteriores. Regras e proteções são restrições transversais. A atividade de movimentar ou registrar estoque, a atividade de avaliar, o ato de autorizar e seus resultados não devem ser confundidos com os objetos examinados. Não se trata de esquema técnico. Posição registrada, quantidade física observada e disponibilidade não são equivalentes. Os 29 históricos incompletos limitam afirmações sobre movimentos; não provam causa para as 192 ocorrências.

**Visão por etapas e eventos:** evento de registro da demanda; preparação das informações; etapa de avaliação de disponibilidade; primeira separação; registro do resultado; eventual identificação de divergência; consolidação; atividade de avaliação da resposta; eventual registro da decisão autorizada; acompanhamento de ciclos e proteções. Nem todo caso tem divergência, verificações podem ser paralelas e o quadro não prescreve fluxo novo.

| Critério e pergunta | Relação principal | Vantagem e limite | Lacuna possível | Sobreposição possível |
|---|---|---|---|---|
| função — o que precisa ocorrer? | contribuições e resultados | mostra responsabilidades; deixa percursos menos visíveis | tratamento dos 29 históricos incompletos | atividade de avaliação e ato de autorização |
| informações e objetos — de que objeto e representação precisamos? | produção, mudança e uso | expõe divergências; deixa ordem em segundo plano | pessoa afetada | regra e indicador compartilhados |
| etapas — em que momentos? | precedência, retorno e espera | localiza interrupções; pode esconder funções | autoridade para reabrir a atividade de análise | verificações paralelas |

Mapa textual selecionado:

- demanda registrada → atividade de avaliação de disponibilidade: **fornece informação** sobre produto, centro e quantidade;
- movimentos → posição registrada: **atualizam estado** quando completos e interpretados pelo mesmo critério;
- posição e condição física → atividade de avaliação de disponibilidade: **fornecem informações candidatas**, cuja definição permanece aberta;
- atividade de avaliação de disponibilidade → separação: **informa** a condição considerada no momento;
- separação → atividade de medição: **produz registro** do atendimento da linha;
- divergências → atividade de avaliação da resposta: **fornecem evidência** com limites declarados;
- meta candidata → atividade de avaliação da resposta: **oferece referência provisória**, sujeita a validação;
- proteções → atividade de avaliação da resposta: **limitam respostas aceitáveis** quando legitimadas;
- atividade de avaliação da resposta → registro da eventual resposta autorizada: **requer autorização**, ainda não identificada;
- registro da eventual resposta → atividade de acompanhamento: **produz resultados** para comparar ciclos e efeitos;
- critérios do Norte ↔ critérios do Sul: **exigem definição e método compartilhados** para comparação; nenhuma dependência operacional ou transferência entre centros foi estabelecida.

Recomposição: as visões mostram contribuições, informações, objetos e momentos, mas só atendem ao todo se preservarem interessados, informações compartilhadas e seus critérios de interpretação, dependências entre centros, autoridade decisória e efeitos posteriores. Não estabelecem causalidade. Norte permanece em `84/1.400 = 6%`, Sul em `108/1.000 = 10,8%`, e o total em `192/2.400 = 8%`. A meta inferior a 3% por centro em três ciclos continua candidata; perdas, custo, divergências e transferência permanecem proteções; estoque adicional, redistribuição, correção de registros e previsão continuam alternativas não avaliadas.

Ao final do Projeto Parcial 1, o artefato contém: formulação do problema, interessados e afetados, restrições e proteções, três decomposições, mapa de dependências e questões abertas. A escolha e construção de modelos ficam para a Aula 04.

### Prática guiada interna — cobrança e atendimento

Compare duas propostas para esclarecer cobrança contestável. A: “cadastro, boleto, telefone, atraso, atendente, cliente irritado, pagamento, relatório”. B, funcional: registrar obrigação; emitir cobrança; receber informação de pagamento; conciliar; registrar e analisar contestação; comunicar conclusão.

Antes do comentário, anote: critério de cada proposta; cobertura; uma lacuna; uma dependência; uma sobreposição; e como recomporia o resultado. **Comentário:** A mistura objeto, canal, condição, papel e interessado, sem critério. B declara funções, mas pode precisar separar registro e atividade de análise da contestação. Proteger informações sensíveis atravessa todas; analisar depende da obrigação, da cobrança e das evidências de pagamento. “Atendente” é papel, não parte equivalente.

Se a pergunta mudar para localizar divergências de estado, os objetos obrigação, cobrança, pagamento e contestação ganham utilidade ao lado das informações e dos registros: cobrança emitida, pagamento informado, estado de conciliação e comunicação emitida. A visão funcional mostra contribuições; a de informações e objetos, significados. Fundir pagamento informado e conciliado pode ocultar uma divergência. Nenhuma visão explica causalmente o atraso nem escolhe automação.

## Atividades, síntese e domínio

### Confusões recorrentes

- **“Decompor é criar lista.”** Lista sem critério, relações e recomposição é enumeração.
- **“Partes devem ter o mesmo tamanho.”** Granularidade segue a decisão, não simetria visual.
- **“Cada parte pertence a uma pessoa.”** Responsabilidade de trabalho não define o recorte universal.
- **“Departamentos revelam a estrutura correta.”** O organograma pode duplicar ou ocultar funções.
- **“Etapas são sempre lineares.”** Há paralelismo, condição, repetição e retorno.
- **“Tabelas existentes revelam informações e objetos.”** Estruturas atuais podem preservar conceitos inadequados ou confundir objeto, informação e registro.
- **“Toda sobreposição é erro.”** Regras e proteções podem atravessar partes legitimamente.
- **“Partes não podem compartilhar regras.”** Compartilhamento coordenado difere de decisão duplicada.
- **“Resolver cada parte resolve o todo.”** Interfaces e propriedades globais ainda podem falhar.
- **“Mais detalhe é sempre melhor.”** Partes minúsculas elevam coordenação e podem perder propósito.
- **“A árvore elimina dependências.”** Relações cruzadas exigem mapa complementar.
- **“Interfaces são telas.”** Elas são relações ou pontos pelos quais informação, material, decisão, regra ou mudança de estado atravessa a fronteira entre partes.
- **“Funções já definem módulos.”** Funções do domínio não são unidades de software.
- **“Exceções cabem em ‘outros’.”** O rótulo costuma esconder cobertura e responsabilidade.
- **“Critério local substitui objetivo global.”** Toda medida parcial volta aos critérios do todo.
- **“A decomposição é neutra e única.”** Propósito, poder e fronteiras tornam a escolha situada e revisável.

### Exercícios — núcleo essencial

Resolva sem consultar uma resposta pronta. Nas questões abertas, declare o critério usado e sustente cada escolha com elementos do enunciado. O núcleo essencial produz a evidência esperada nesta aula; não comprova sozinho o domínio final de C03.

1. **Objetiva — definição.** Qual opção descreve adequadamente a decomposição de problemas nesta aula?
   - A) Dividir o todo formulado segundo um critério, tornar cada parte administrável e validar seus resultados separadamente contra metas locais.
   - B) Dividir o todo formulado segundo propósito e critério, preservar relações, dependências e restrições relevantes e testar, pela recomposição, se o objetivo global permanece atendido.
   - C) Partir de uma solução já escolhida, dividi-la segundo um critério, preservar relações entre seus elementos e verificar se essa solução pode ser reconstruída.
   - D) Dividir o problema formulado em partes administráveis, registrar responsáveis e interfaces e, depois de delimitá-las, tratar as partes como independentes.

2. **Objetiva — dependência e ordem.** Duas verificações foram agendadas para manhã e tarde; ambas consultam a mesma regra, mas nenhuma usa o resultado da outra. A leitura mais precisa é:
   - A) existe ordem de agenda e dependência compartilhada da regra, não necessariamente dependência entre as verificações;
   - B) a verificação da tarde depende da manhã porque ocorre depois;
   - C) não existe dependência, pois as verificações não trocam resultados diretamente;
   - D) a regra é externa às duas verificações e, por isso, não precisa aparecer no mapa de dependências.

3. **Objetiva — sobreposição.** Privacidade restringe recebimento, atividade de análise e emissão da comunicação. Qual registro distingue transversalidade legítima de duplicidade problemática?
   - A) Atribuir a privacidade exclusivamente a uma parte de governança; as demais apenas encaminham incidentes quando os detectam.
   - B) Registrar a privacidade somente no recebimento, pois a proteção aplicada na origem acompanha automaticamente todos os usos posteriores.
   - C) Tratá-la como restrição transversal, declarando seu efeito e a responsabilidade em cada parte afetada e coordenando a regra compartilhada.
   - D) Replicar a regra em cada parte e permitir que cada responsável a interprete localmente, dispensando coordenação entre as partes.

4. **Dissertativa — definição operacional.** Explique, com suas palavras, por que critério, preservação e recomposição são necessários. Dê um exemplo em que a ausência de um deles produz apenas fragmentação.

5. **Dissertativa — ordem e dependência.** Produza um exemplo de ordem sem dependência e outro de dependência sem ordem fixa. Para cada um, explique o teste usado.

6. **Dissertativa — recomposição.** Explique como uma melhoria local pode piorar o todo. Relacione uma métrica local, um critério global e uma proteção.

7. **Análise de caso — lista arbitrária.** Reescreva “cadastro, gerente, documento, três dias, análise, tela” como decomposição funcional coerente de uma solicitação. Registre o que foi removido, reposicionado ou renomeado.

8. **Análise de caso — dois critérios e cobertura.** Uma escola quer reduzir matrículas que exigem correção. Considere a visão funcional inicial “receber matrícula; verificar completude; registrar necessidade de correção; comunicar o que falta; encerrar o caso”. Revise-a se necessário e produza uma visão resumida por informações e objetos do domínio, com quatro a seis partes. Compare o que cada visão evidencia e indique uma lacuna ou limite de cobertura.

9. **Revisão.** Receba esta divisão: “entrada, análise, gerente, documento, saída”. Faça duas revisões entre critério, fronteira, granularidade ou dependência. Para cada mudança, declare a razão e o efeito sobre cobertura ou recomposição.

### Exercícios — aprofundamento

Os exercícios 10 a 16 são opcionais. Eles ampliam distinções, granularidade, formalização, transferência, mapa e integração do P1; não são pré-requisito para iniciar a Aula 04.

10. **Dissertativa — distinções.** Compare parte, subproblema, função, tarefa e etapa usando um único caso. Não use cinco exemplos desconectados.

11. **Dissertativa — hierarquia e parada.** Crie dois níveis funcionais para “tratar contestação” e justifique onde parou. Indique um detalhe que seria prematuro no propósito atual.

12. **Análise de caso — estoque.** Escolha uma função ampla do caso progressivo, decomponha-a em três a cinco partes e justifique a granularidade. Preserve os limites de evidência e não proponha solução.

13. **Análise matemática — cobertura e interseção.** Para `W = {receber, verificar, decidir, comunicar, contestar}`, considere `P₁ = {receber, verificar}`, `P₂ = {verificar, decidir}`, `P₃ = {comunicar}`. Calcule a união, identifique uma interseção não vazia, indique a lacuna e diga se há partição estrita. Proponha primeiro a menor correção explícita para restaurar cobertura, sem usar “outros”; depois, indique a mudança adicional necessária para obter partição estrita.

14. **Contraexemplo.** Construa um contraexemplo para a afirmação “se todas as tarefas foram atribuídas, o problema foi bem decomposto”. Mostre pelo menos uma dependência ou propriedade global perdida.

15. **Auditoria de mapa ampliado.** Considere as relações “recebimento → verificação documental: documentos”; “verificação → atividade de análise: antes”; “atividade de análise → ato de decidir: conclusão”; “decisão registrada → emissão da comunicação: resultado”; “comunicação emitida → contestação: prazo”; “contestação → reanálise: nova evidência”; “reanálise → nova decisão: retorno”; e “privacidade → todas as partes: aplica-se”. Identifique ao menos três rótulos insuficientes ou relações ambíguas. Reescreva-os com origem, destino, significado, condição e consequência da ausência; preserve o retorno e trate privacidade como restrição transversal, não como origem causal.

16. **Integração — Projeto Parcial 1.** Audite as três decomposições do estoque. Identifique uma lacuna possível, uma sobreposição legítima, um risco de duplicidade e uma questão aberta que pode alterar a estrutura. Conclua se o artefato está suficiente para avançar à Aula 04, sem criar o modelo.

Não há um gabarito completo nesta aula. Nas objetivas, procure a alternativa que preserva todos os elementos da definição, não palavras isoladas. Nas abertas, a correção deve observar coerência do critério, cobertura, dependências, granularidade, limites da evidência e recomposição. Decomposições diferentes podem ser adequadas quando justificadas pelo propósito.

### Recuperação ativa e reflexão

Sem reler, responda: por que o propósito orienta a decomposição? parte difere de subproblema como? função difere de etapa como? o que torna uma dependência relevante? por que ordem não a implica? o que é granularidade? quando parar? como detectar lacuna? quando sobreposição é legítima? o que é otimização local? como demonstrar recomposição? por que a divisão não é neutra? Depois, desenhe quatro partes e recomponha-as em um parágrafo.

Reflita: quem tem poder para definir partes e fronteiras? A divisão organizacional torna responsabilidades ou pessoas afetadas invisíveis? Métricas locais fragmentam o trabalho ou deslocam consequências? Registre uma alteração que faria após ouvir quem atravessa mais de uma parte.

### Síntese

Decompor é controlar complexidade por divisão orientada, não acumular itens. Funções, informações e objetos do domínio e etapas oferecem vistas diferentes. Hierarquia e granularidade organizam níveis; dependências e interfaces preservam conexões; cobertura, sobreposição e lacunas testam a estrutura. Recomposição mantém o todo reconhecível e protegido. A divisão revisável prepara a Aula 04 para escolher detalhes e perdas de cada abstração.

### Mini glossário

O mini glossário preserva 27 termos:

1. **Decomposição:** divisão orientada que preserva recomposição.
2. **Todo:** problema formulado de referência.
3. **Parte:** recorte produzido pelo critério.
4. **Subproblema:** questão menor ligada ao problema maior.
5. **Função do problema:** contribuição ou transformação necessária.
6. **Tarefa:** ação delimitada em um contexto.
7. **Etapa:** período reconhecível no percurso.
8. **Componente:** elemento identificável de sistema ou solução.
9. **Critério de decomposição:** princípio que distingue as partes.
10. **Decomposição funcional:** divisão por contribuições ou transformações.
11. **Decomposição por informações e objetos do domínio:** divisão pelo significado, identidade, condição e uso de informações, registros ou objetos relevantes.
12. **Decomposição por etapas:** divisão por momentos ou eventos.
13. **Hierarquia:** organização de partes em níveis.
14. **Nível:** posição de detalhe na hierarquia.
15. **Granularidade:** grau de detalhe das partes.
16. **Relação:** conexão relevante entre partes.
17. **Dependência:** relação em que uma parte requer algo de outra.
18. **Precedência:** relação de antes e depois.
19. **Interface:** relação ou ponto pelo qual algo relevante atravessa a fronteira entre partes.
20. **Cobertura:** alcance conjunto sobre o todo.
21. **Lacuna:** aspecto necessário não coberto.
22. **Sobreposição:** aspecto compartilhado por partes.
23. **Duplicidade:** repetição problemática sem coordenação.
24. **Elemento transversal:** condição aplicada a várias partes.
25. **Recomposição:** demonstração de que partes e relações sustentam o todo.
26. **Otimização local:** melhoria parcial que pode prejudicar o conjunto.
27. **Partição:** cobertura por partes sem sobreposição em sua forma estrita.

### Critérios de domínio da aula

**Nível 1 — reconhecimento:** localizar todo, partes e critério em exemplo fornecido.

**Nível 2 — explicação:** distinguir decomposição de lista, explicar dependência, granularidade, cobertura e recomposição.

**Nível 3 — aplicação guiada:** decompor por ao menos dois critérios; justificar parada; construir árvore ou quadro e mapa; identificar lacuna, duplicidade e sobreposição; demonstrar cobertura e recomposição.

**Início do Nível 4:** decompor caso simples autonomamente, comparar critérios e revisar após feedback. C03 não está dominada em problemas complexos; depende das Aulas 06, 11 e 14.

### Continuidade para a Aula 04

A Aula 04 perguntará quais detalhes precisam aparecer ou podem ser omitidos, para qual propósito, em qual nível e com quais perdas. Esta aula não antecipa entidade, atributo, teoria de modelos, representação formal, fluxograma, pseudocódigo ou partes de software. O núcleo essencial e a prática essencial fornecem a preparação necessária; exercícios e prática de aprofundamento permanecem opcionais.

## Referências, métricas e carga

### Referências centrais

- PÓLYA, George. *How to Solve It*. 2. ed. Princeton University Press, 1957. Apoia decompor, recombinar e revisar, não receita universal.
- KUMAR, Amruth N. et al. *Computer Science Curricula 2023*. ACM, IEEE Computer Society e AAAI, 2023. Sustenta progressão curricular. [Relatório oficial](https://ieeecs-media.computer.org/media/education/reports/CS2023.pdf).

### Aprofundamento bibliográfico

- SIMON, Herbert A. The Architecture of Complexity. *Proceedings of the American Philosophical Society*, v. 106, n. 6, p. 467–482, 1962. Apoia hierarquia e interações, não divisão natural única. [Registro estável](https://www.jstor.org/stable/985254).
- PARNAS, David L. On the Criteria To Be Used in Decomposing Systems into Modules. *Communications of the ACM*, v. 15, n. 12, p. 1053–1058, 1972. Usado apenas para critério e alternativas à sequência de processamento. [DOI](https://doi.org/10.1145/361598.361623).

### Terminologia e sistemas

- ISO; IEC; IEEE. *ISO/IEC/IEEE 24765:2017 — Systems and software engineering — Vocabulary*. Referência terminológica. [Registro oficial](https://www.iso.org/standard/71952.html).
- ISO; IEC; IEEE. *ISO/IEC/IEEE 15288:2023 — Systems and software engineering — System life cycle processes*. Apoia iteração e recursão, sem prescrever o método. [Registro oficial](https://www.iso.org/standard/81702.html).

### Métricas e carga sugerida

- **Extensão:** aproximadamente 7.600 palavras, 519 linhas, 10 seções H2 e 34 subseções H3.
- **Atividades e casos:** 16 exercícios — 9 no núcleo essencial e 7 no aprofundamento; 3 objetivos, 5 dissertativos e 8 de análise ou integração —; 3 casos desenvolvidos, além de casos curtos; 6 fontes.
- **Matemática:** subconjunto, união, interseção, vazio, cobertura, sobreposição, partição, percentuais e desigualdade.
- **Percurso essencial:** leitura, 1h45–2h15; recuperação, 25–35 min; núcleo essencial de exercícios, 1h40–2h10; prática essencial, 3h15–4h20; revisão final, 15–25 min; total, **7h20–9h45**.
- **Percurso completo opcional:** leitura e recuperação, 2h10–2h50; todos os exercícios, 3h20–4h30; prática com aprofundamento, 5h20–7h00; revisão ampliada, 30–45 min; total, **11h20–15h05**.
