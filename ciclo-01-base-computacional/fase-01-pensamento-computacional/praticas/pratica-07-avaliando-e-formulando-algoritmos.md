# Prática 07 — Avaliar, formular e explicar um algoritmo

## Objetivo e modalidades

Avaliar descrições candidatas e formular algoritmo independente de linguagem para validação estrutural de uma transação individual, explicando contrato, efetividade, precisão, término, correção intuitiva, pressupostos e limites.

Na trilha essencial, conclua os onze blocos em 3h15–4h. O aprofundamento acrescenta contrato alternativo, não determinismo, heurística, entrada fora do domínio, segunda representação e transferência; não é requisito para avançar.

O caso não detecta fraude, decide bloqueio, prevê risco, escolhe intervenção ou substitui autoridade humana. Cada execução trata uma transação, sem repetição.

## Bloco 1 — Avaliar descrições candidatas

Avalie sete candidatas:

- **C1 — intenção vaga:** “analise cuidadosamente e faça o melhor”.
- **C2 — processo organizacional:** receber, pedir parecer, aguardar aprovação e negociar quando necessário.
- **C3 — forma sem contrato:** pseudocódigo recebe “dados”, manda “resolver” e produz “ok”.
- **C4 — procedimento sem saída:** verifica identificador, moeda e autorização, mas não declara resultado.
- **C5 — espera indefinida:** aguarda confirmação externa até que ela chegue.
- **C6 — heurística:** encaminha para atenção os registros que “parecem incomuns”, sem garantir classificação correta.
- **C7 — quase adequada:** recebe um registro individual admitido, verifica campos e autorização em quantidade fixa, produz categoria e motivo, mas confunde autorização ausente com desconhecida.

| Candidato | Classe | Entrada | Saída | Efetivo? | Termina? | Veredito |
|---|---|---|---|---|---|---|
| C1 |  |  |  |  |  |  |
| C2 |  |  |  |  |  |  |
| C3 |  |  |  |  |  |  |
| C4 |  |  |  |  |  |  |
| C5 |  |  |  |  |  |  |
| C6 |  |  |  |  |  |  |
| C7 |  |  |  |  |  |  |

Justifique cada célula. Processo útil não vira algoritmo por ser detalhado; pseudocódigo não fornece contrato; heurística pode ser executada algoritmicamente, mas sua garantia é limitada. Em C7, identifique o que pode ser preservado e o que precisa ser revisto.

Para cada veredito, cite ao menos dois critérios entre classe, entrada, saída, efetividade, precisão e término. “Não gostei” ou “parece algoritmo” não são justificativas. Quando a informação for insuficiente, escreva “não demonstrado” em vez de preencher por suposição.

## Bloco 2 — Classe e instâncias

Use a classe: **classificar estruturalmente uma transação individual para análise posterior, segundo campos obrigatórios e estado da autorização, produzindo categoria e motivo**.

Defina duas instâncias pertencentes:

| Instância | Identificador | Valor/moeda | Contas | Campos | Autorização |
|---|---|---|---|---|---|
| I1 | presente | 250,00 BRL | presentes | completos | confirmada |
| I2 | presente | 80,00 BRL | presentes | completos | desconhecida |

Proponha um caso fora da classe e explique o motivo. Um conjunto de várias transações está fora porque a unidade é um registro por execução. Uma imagem ilegível também pode estar fora do domínio, mas registre se isso é fronteira legítima ou lacuna diante do objetivo.

Não defina classe como “casos aprovados pelo algoritmo”. A classe precisa existir independentemente da solução.

## Bloco 3 — Contrato

Entrada hipotética:

- identificador;
- valor e moeda;
- conta de origem e destino;
- autorização confirmada, ausente ou desconhecida;
- campos obrigatórios completos ou incompletos.

Saídas permitidas:

- estruturalmente apta para análise posterior;
- pendente de informação;
- estruturalmente inválida para o recorte;
- sempre com motivo.

| Elemento | Declaração |
|---|---|
| classe |  |
| entrada |  |
| domínio |  |
| pré-condições |  |
| saídas |  |
| pós-condições |  |
| dependências externas |  |
| limites |  |

Desconhecido deve permanecer diferente de ausente. Valor monetário exige moeda declarada. Defina quais campos são obrigatórios. Fraude, aprovação financeira, bloqueio, segurança e autorização definitiva ficam fora.

Revise a pré-condição: ela descreve entrada admissível ou elimina silenciosamente o caso mais difícil? Revise a pós-condição: ela relaciona entrada e saída ou apenas repete “funciona”?

Faça uma leitura nos dois sentidos. Do contrato para o procedimento, localize onde cada saída e limite será atendido. Do procedimento para o contrato, identifique qualquer dado ou regra usada sem origem. Registre dependência não fornecida em vez de inventá-la.

## Bloco 4 — Procedimento em linguagem estruturada

Escreva passos para uma transação, com quantidade fixa de verificações. Não use “para cada”, “enquanto”, coleção, contador ou acumulador.

Cada ação deve identificar objeto, operação, resultado observável e referência ao contrato. Uma estrutura possível, que deve ser completada sem inventar regras:

1. receber uma transação admissível;
2. verificar se os campos obrigatórios estão completos e interpretáveis;
3. se houver campo incompleto, produzir a categoria estrutural correspondente e motivo;
4. caso contrário, identificar o estado declarado da autorização;
5. preservar a diferença entre ausente e desconhecida;
6. produzir uma das saídas permitidas e motivo;
7. encerrar o recorte.

Não transforme “autorização ausente” em fraude ou bloqueio. Se o contrato não determinar qual categoria estrutural corresponde a uma condição, registre a lacuna antes de escrever o passo.

## Bloco 5 — Pseudocódigo

Converta o procedimento para pseudocódigo independente de linguagem, com convenções locais em português. O texto deve declarar início e fim do recorte, receber uma transação e produzir categoria e motivo.

Não imite sintaxe real. Não use repetição. Não inclua “resolver”, “validar adequadamente” ou “decidir o melhor”. Mantenha desconhecido explícito.

Audite a conversão:

| Elemento do contrato | Passo estruturado | Pseudocódigo | Situação |
|---|---|---|---|
| entrada |  |  |  |
| campos obrigatórios |  |  |  |
| autorização desconhecida |  |  |  |
| saída e motivo |  |  |  |
| limite decisório |  |  |  |

Pseudocódigo é representação do algoritmo candidato. A forma correta não prova que o conteúdo satisfaz o contrato.

Compare ainda os nomes empregados. “Ausente”, “desconhecida” e “incompleta” não podem virar um único rótulo por economia. Se a notação não tiver maneira clara de preservar a diferença, revise a convenção antes do conteúdo.

## Bloco 6 — Efetividade e precisão

Para cada passo, pergunte se o executor sabe o que consultar, se o resultado é observável, se o termo está definido, se há julgamento oculto, dependência externa ou resultado anterior necessário.

| Passo | Operação efetiva? | Ambiguidade | Dependência | Revisão |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

“Campos completos” só é preciso se os campos obrigatórios estiverem listados. “Moeda válida” depende de domínio admitido. “Consultar autorização” não é efetivo se exige serviço externo sem contrato; usar o estado já recebido é operação distinta.

Classifique dependências como entrada, definição do contrato, resultado anterior ou serviço externo. Não esconda uma dependência mudando o verbo.

## Bloco 7 — Término

Produza argumento de 120–200 palavras. Ele deve mencionar:

- uma transação por execução;
- quantidade fixa de verificações;
- ausência de repetição ou espera indefinida;
- operações externas somente sob contrato;
- caminho até cada saída;
- todas as entradas admissíveis.

Não aceite “termina porque tem FIM”, “porque é curto” ou “porque terminou nos exemplos”. Se seu procedimento espera nova informação, revise-o para produzir pendência; a obtenção posterior pertence a outro processo.

Separe descrição finita e execução finita. O pseudocódigo caber numa página não impede espera sem limite.

Depois do primeiro argumento, procure um caminho que não tenha sido mencionado. Se encontrar condição sem saída ou operação externa sem limite, o argumento revelou uma revisão necessária; não acrescente a palavra FIM como correção.

## Bloco 8 — Correção intuitiva

Relacione grupos de entrada às saídas, sem construir tabela de decisão completa:

| Condição relevante | Saída esperada | Por que satisfaz a pós-condição |
|---|---|---|
| campo obrigatório incompleto |  |  |
| autorização desconhecida |  |  |
| autorização ausente |  |  |
| dados completos e autorização confirmada |  |  |

Explique por que cada grupo chega à categoria e ao motivo compatíveis. Preserve os limites: “apta para análise posterior” não é aprovação; “inválida no recorte” não é fraude.

Isso é argumento intuitivo, não prova formal. Os grupos ajudam a examinar cobertura conceitual, mas exemplos não substituem o argumento sobre toda entrada admissível.

Confirme também que a saída contém motivo. Um procedimento que escolhe categoria correta e perde a justificativa viola a pós-condição adotada. Se dois grupos chegam à mesma categoria por motivos diferentes, preserve a diferença quando ela for necessária à análise posterior.

## Bloco 9 — Casos de exame

| Caso | Campos | Valor/moeda | Autorização | Pertence ao domínio? |
|---|---|---|---|---|
| T1 | completos | 250,00 BRL | confirmada |  |
| T2 | conta destino ausente | 90,00 BRL | confirmada |  |
| T3 | completos | 300,00 BRL | desconhecida |  |
| T4 | completos | 100 sem moeda | ausente |  |

Registre saída, motivo, lacuna e efeito sobre o algoritmo. Não faça rastreamento passo a passo de estados.

T4 exige decisão de contrato: valor sem moeda é entrada admitida que produz pendência ou viola pré-condição? Justifique sem excluir silenciosamente. Os casos examinam o procedimento; não provam correção.

Não altere o algoritmo entre T1 e T4. Registre primeiro os efeitos da versão vigente. Caso uma lacuna apareça, leve-a ao Bloco 10 e preserve a evidência que motivou a mudança.

## Bloco 10 — Contraexemplo e revisão

Introduza T5: todos os campos estão presentes, mas o valor é textual e não interpretável. Um algoritmo que verifica apenas presença pode produzir “apta”, contrariando a pós-condição estrutural.

| Item | Registro |
|---|---|
| versão inicial |  |
| contraexemplo | T5 |
| diagnóstico |  |
| contrato revisto |  |
| passo revisto |  |
| pseudocódigo revisto |  |
| impacto e limite |  |

Preserve as duas versões. Distinga campo presente de campo interpretável. Se alterar domínio, explique por que a mudança corresponde ao problema e como entradas rejeitadas serão reconhecidas.

Uma revisão localizada é preferível a reescrever sem diagnóstico. O contraexemplo pode revelar saída ausente, ambiguidade, pré-condição excessiva, dependência oculta, não término ou pós-condição incompleta.

## Bloco 11 — Relação com o P3

Transfira o método, não as regras de transação, para o estoque:

| Elemento | Preparação de uma ocorrência não atendida |
|---|---|
| classe |  |
| entrada |  |
| saída |  |
| pré-condição |  |
| pós-condição |  |
| limite |  |
| caso para Aula 08 |  |

Preserve histórico desconhecido, ausência de causalidade e autoridade decisória. O algoritmo inicial prepara uma ocorrência para análise; não escolhe intervenção.

Escolha um caso admissível para rastrear na Aula 08, mas não registre estados intermediários agora.

Declare quais elementos do método foram transferidos: classe, contrato, efetividade, término, correção intuitiva e limites. Não transfira categorias de transação para estoque apenas porque a estrutura da atividade é semelhante.

## Entrega, solução comentada e autocorreção

Entregue avaliação dos sete candidatos, classe e instâncias, contrato, procedimento, pseudocódigo, análise de efetividade, argumentos de término e correção intuitiva, quatro casos, revisão, ligação com P3 e autoavaliação.

### Solução comentada — consulte somente depois da tentativa

Não existe redação única. C1 é intenção; C2 é processo aberto; C3 tem forma sem contrato; C4 não produz saída; C5 não garante término; C6 é heurística vaga; C7 é quase adequada, mas perde diferença semântica essencial.

Contrato parcial possível: domínio de um registro individual legível com vocabulário declarado; saída estrutural com motivo; limite sem decisão financeira. Campos incompletos podem produzir “inválida no recorte”; autorização desconhecida, “pendente”; dados completos e confirmação, “apta para análise posterior”. A autorização ausente exige formulação coerente com a fonte e não autoriza inferir fraude.

Um passo exemplar é “verificar se identificador, valor, moeda e contas estão presentes e interpretáveis conforme definições do contrato”. “Verificar se está tudo certo” permanece vago.

O término decorre de uma unidade por execução, verificações fixas e caminhos que produzem saída sem esperar. T5 mostra que presença não implica interpretabilidade; revise definição e passo. Alternativas são aceitas se preservarem contrato, desconhecidos e limites.

Uma solução não deve preencher lacunas com políticas novas. Se o contrato não disser como tratar autorização ausente, a resposta adequada pode ser registrar pendência na versão inicial e formular pergunta, não criar rejeição automática. Se a equipe decidir depois uma regra estrutural autorizada, identifique a nova fonte e a nova versão.

Nos casos de exame, T1 pode sustentar “apta para análise posterior” sem significar aprovação. T2 evidencia incompletude. T3 preserva desconhecido. T4 e T5 examinam a diferença entre presença, moeda declarada e interpretabilidade. Esses resultados ajudam a revisar, mas não constituem prova.

Para o P3, uma resposta adequada leva o formato do contrato ao estoque e mantém o conteúdo do domínio anterior: uma ocorrência, histórico conhecido ou desconhecido, evidência, saída de preparação e limite decisório. Não copie categorias financeiras.

No aprofundamento, um contrato alternativo pode admitir entrada inicialmente fora do domínio e produzir saída explícita. Compare a ampliação por adequação, não por quantidade. Uma heurística pode ser representada por passos efetivos, mas seu contrato deve declarar que não garante a conclusão ampla. Um procedimento contínuo pode ser útil sem satisfazer o recorte terminante desta aula.

### Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| classe/instância | confunde caso e conjunto | distingue | cobre domínio |
| entrada/domínio | usa conhecimento oculto | declara | trata inválidos |
| saída | vaga ou decisória | observável | contém motivo |
| pré/pós-condição | vira passo | declara propriedade | relaciona entrada e saída |
| contrato | incompleto | verificável | orienta passos |
| efetividade | exige adivinhação | operação realizável | dependências visíveis |
| precisão | termos vagos | definições locais | interpretação estável |
| ordem | arbitrária | dependência indicada | compatível com contrato |
| término | cita FIM | argumenta | cobre domínio |
| correção | cita exemplos | relaciona grupos | preserva limites |
| representação | confunde com algoritmo | distingue | conversão coerente |
| contraexemplo | ignora | diagnostica | revisa contrato e passos |
| independência | imita linguagem | pseudocódigo local | sem implementação |
| pressupostos/limites | ocultos | declarados | não automatiza autoridade |

O essencial termina quando nenhum critério está em “precisa de revisão”.

## Carga

- Avaliação de candidatos e classe: 35–45 min.
- Contrato e procedimento: 50–65 min.
- Pseudocódigo e efetividade: 45–55 min.
- Término e correção intuitiva: 35–45 min.
- Casos, revisão, P3 e autoavaliação: 30–50 min.
- Prática essencial: 3h15–4h.
- Aula, exercícios, prática e revisão: aproximadamente 7h50–10h.
- Aprofundamento opcional: 3h–5h adicionais.
- Percurso completo opcional: 11h30–15h.
