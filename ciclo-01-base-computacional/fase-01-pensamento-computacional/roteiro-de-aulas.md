# Roteiro de Aulas — Fase 1

Este roteiro define 14 aulas futuras. Ele delimita finalidade, conceitos, prática, matemática e fronteira; não contém aulas integrais.

## Aula 01 — O que é pensamento computacional

**Finalidade:** apresentar pensamento computacional como família de práticas e perspectivas para formular problemas e soluções computáveis, relacionada à Ciência da Computação, mas não reduzida a programar.

**Desenvolvimento:** origem e difusão do termo; formulações de Jeannette Wing e debates posteriores; resolução de problemas, projeto de sistemas e compreensão de processos; alcance e limites; execução por pessoas ou máquinas; decomposição, abstração, padrões e algoritmos como dimensões relacionadas, não taxonomia universal; aplicações em sistemas corporativos.

**Prática prevista:** comparar descrições de uma tarefa que mostram ou não formulação, representação e verificação; analisar um fluxo corporativo sem propor código.

**Cuidado:** não prometer que qualquer raciocínio organizado é pensamento computacional nem apresentar “quatro pilares” como consenso único. Prepara a Aula 02 ao deslocar a atenção do rótulo para a formulação concreta de problemas.

## Aula 02 — O que é um problema

**Finalidade:** transformar situações vagas em problemas delimitados e verificáveis.

**Desenvolvimento:** situação, necessidade, problema, sintoma, causa e hipótese causal; objetivo; estado inicial e desejado; resultado esperado; interessado; escopo; restrição; recurso; entrada; saída; regra; condição; critério de sucesso; ambiguidade e problema mal definido. Retomada funcional de necessidade, requisito, regra de negócio e especificação da Fase 0.

**Matemática:** igualdade e desigualdade em critérios; intervalos e conjuntos simples de entradas admissíveis.

**Prática prevista:** reformular solicitações ambíguas de cadastro, cobrança e atendimento; separar fato, inferência, hipótese e decisão.

**Cuidado:** não confundir a solução solicitada pelo interessado com a definição do problema. Prepara decomposição ao estabelecer o todo que será dividido.

## Aula 03 — Decomposição de problemas

**Finalidade:** dividir complexidade preservando relações e possibilidade de recomposição.

**Desenvolvimento:** partes, responsabilidades, dependências, ordem e níveis; decomposição funcional, por dados e por etapas; critérios para parar de decompor; granularidade; interfaces iniciais; riscos de duplicidade, lacunas, partes incompatíveis e otimização local; recomposição e validação do todo.

**Prática prevista:** decompor um processo de concessão de benefício por três critérios e comparar consequências; criar mapa de dependências.

**Cuidado:** uma lista de tarefas não é automaticamente uma boa decomposição. Prepara abstração ao exigir escolha do que cada parte deve expor ou ocultar.

## Aula 04 — Abstração e modelos

**Finalidade:** selecionar detalhes relevantes para uma pergunta sem ensinar vagueza como simplificação.

**Desenvolvimento:** abstração; omissão controlada; modelo; representação; propósito; público; fronteira; nível de detalhe; entidade, atributo e relação em nível inicial; exemplos e contraexemplos; múltiplos modelos do mesmo sistema; perdas, vieses e riscos de abstração inadequada; relação com sistemas.

**Matemática:** conjuntos simples, pertencimento, relações e noção inicial de função entre entrada e saída quando pertinente.

**Prática prevista:** produzir modelos operacional e gerencial do mesmo processo de estoque, declarando omissões e limites.

**Cuidado:** modelo não é cópia integral da realidade nem verdade universal. Prepara padrões ao tornar comparáveis atributos selecionados.

## Aula 05 — Padrões e generalização

**Finalidade:** usar semelhanças e diferenças para reaproveitar raciocínio sem apagar exceções relevantes.

**Desenvolvimento:** atributo, semelhança, diferença, classificação, classe, regularidade, padrão, caso particular, regra, exceção, exemplo, contraexemplo, generalização e reutilização; padrões em dados e processos; generalização excessiva e correlação superficial.

**Matemática:** conjuntos, pertencimento, classificação, relações, igualdade e desigualdade.

**Prática prevista:** classificar transações e ocorrências de estoque, propor regra geral, procurar contraexemplo e restringir seu domínio.

**Cuidado:** repetição observada não garante lei nem causa. Prepara representações ao exigir que padrões e regras sejam comunicados sem ambiguidade.

## Aula 06 — Representação de problemas e soluções

**Finalidade:** selecionar a forma de representação conforme pergunta, público e necessidade de verificação.

**Desenvolvimento:** linguagem natural; listas estruturadas; tabelas; diagramas; fluxogramas; tabelas de decisão; modelos de estado; pseudocódigo; convenções; ambiguidade; consistência; rastreabilidade; conversão e combinação de representações; perdas de informação.

**Prática prevista:** representar o mesmo procedimento em texto estruturado, tabela e diagrama; converter entre duas formas e auditar divergências.

**Cuidado:** não transformar a aula em memorização de símbolos de fluxograma. Prepara algoritmo ao fornecer meios de registrar um procedimento já compreendido.

## Aula 07 — O que é um algoritmo

**Finalidade:** construir definição operacional precisa e distinguir algoritmo de entidades próximas.

**Desenvolvimento:** problema e classe de problemas; instância; entrada; saída; pré e pós-condição em nível introdutório; procedimento; passos efetivos; precisão; finitude; condição de término; determinismo e não determinismo introdutório; algoritmo, solução, representação, programa, implementação, heurística e processo organizacional.

**Matemática:** função como relação entrada–saída, sequência e contagem simples.

**Prática prevista:** avaliar descrições candidatas a algoritmo; formular procedimento de validação de transações e explicar por que termina e resolve a classe declarada.

**Cuidado:** “receita” é analogia limitada e algoritmo não precisa estar em código. Prepara sequência e estado ao perguntar o que muda a cada passo.

## Aula 08 — Sequência e estado

**Finalidade:** tornar observáveis ordem, dependência e mudança ao longo de uma execução.

**Desenvolvimento:** ordem; sequência; dependência; estado; transição; valor; atualização; variável como representação conceitual de valor mutável; memória conceitual; atribuição sem sintaxe de linguagem; rastreamento; tabela de execução; efeito de trocar passos; invariante inicial.

**Matemática:** sequências, igualdade antes/depois, intervalos e função de transição em nível intuitivo.

**Prática prevista:** rastrear saldo, estoque disponível e status; comparar duas ordens de atualização; identificar propriedade que deve permanecer verdadeira.

**Cuidado:** variável não é apenas “caixa” nem igualdade matemática é idêntica a atualização. Prepara decisões, que escolhem transições conforme condições.

## Aula 09 — Decisões e condições

**Finalidade:** representar escolhas completas e verificáveis com fundamentos lógicos graduais.

**Desenvolvimento:** condição; proposição; verdadeiro e falso; comparação; igualdade e desigualdade; negação, conjunção e disjunção; decisão simples e aninhada; alternativas; tabela de decisão; cobertura, exclusividade e completude; condições incompletas; precedência lógica inicial.

**Matemática:** lógica proposicional introdutória, tabelas pequenas de valores lógicos, intervalos e pertencimento.

**Prática prevista:** construir tabela de decisão para reposição e elegibilidade; converter para pseudocódigo; testar fronteiras e combinações.

**Cuidado:** linguagem natural pode ocultar precedência e condições sobrepostas. Prepara repetição, cuja continuidade também depende de condição.

## Aula 10 — Repetição e iteração

**Finalidade:** descrever processamento repetido com inicialização, progresso e término explícitos.

**Desenvolvimento:** repetição; iteração; coleção; condição de continuidade e de parada; repetição definida e condicionada; contador; acumulador; busca; processamento de coleção; progresso; laço infinito; erro por uma posição; rastreamento de iterações.

**Matemática:** contagem, sequência, intervalos, soma acumulada e limites simples.

**Prática prevista:** totalizar movimentos, buscar primeiro item elegível e processar coleção vazia, unitária e múltipla; registrar cada iteração.

**Cuidado:** repetir não garante progresso e a condição deve ser avaliada no estado correto. Prepara modularização ao revelar responsabilidades repetíveis.

## Aula 11 — Modularização e composição

**Finalidade:** organizar solução por responsabilidades e contratos compreensíveis.

**Desenvolvimento:** módulo; procedimento; função como conceitos; responsabilidade; parâmetro; entrada e saída; pré e pós-condição; contrato; coesão e acoplamento introdutórios; reutilização; composição; dependência; ordem de execução; estado compartilhado e efeitos em nível inicial.

**Prática prevista:** modularizar validação e reposição, escrever cartões de contrato e recompor o fluxo; identificar dependência oculta.

**Cuidado:** quantidade de módulos não mede qualidade e a aula não entra em arquitetura avançada. Prepara testes ao permitir verificar partes e integrações.

## Aula 12 — Correção, testes e depuração

**Finalidade:** transformar expectativas em evidência e investigar divergências sem adivinhação.

**Desenvolvimento:** comportamento esperado e observado; caso, entrada e oráculo de teste; caso normal, limite e inválido; teste positivo e negativo; cobertura como noção; rastreamento manual; hipótese; engano, defeito, falha e incidente; depuração; evidência; correção aparente; regressão introdutória. Conexão explícita com a Aula 12 da Fase 0.

**Prática prevista:** projetar testes, localizar defeitos em pseudocódigo e criar teste de regressão; separar sintoma de causa provável.

**Cuidado:** teste demonstra comportamento nos casos executados, não prova universal automaticamente. Prepara eficiência ao estabelecer que somente soluções adequadamente corretas devem ser comparadas pelo custo.

## Aula 13 — Eficiência e escolha de estratégias

**Finalidade:** comparar soluções corretas por custos e adequação sem antecipar análise assintótica completa.

**Desenvolvimento:** múltiplas soluções; correção, eficiência e adequação; custo; tempo; espaço; número de operações; tamanho de entrada; escalabilidade intuitiva; crescimento constante, linear e quadrático por exemplos; solução correta porém inviável; clareza, manutenção e desempenho; medição; otimização prematura; limitações e trade-offs.

**Matemática:** contagens, tabelas, gráficos simples, razões e crescimento relativo. Big O e formalismos equivalentes ficam para fase posterior.

**Prática prevista:** contar comparações em duas buscas simples e operações em estratégias de conciliação; justificar escolha segundo volume e risco.

**Cuidado:** rapidez observada em caso pequeno não estabelece eficiência geral. Prepara o projeto ao exigir escolha argumentada.

## Aula 14 — Projeto integrado de pensamento computacional

**Finalidade:** integrar formulação, modelagem, algoritmo, verificação e comparação em caso corporativo rico.

**Caso:** controle de estoque e reposição de uma rede de distribuição. O processo recebe cadastro de itens, saldo inicial, recebimentos, vendas e ajustes; rejeita movimentos inválidos; atualiza estoque; identifica itens abaixo do ponto de reposição; calcula sugestão respeitando lote mínimo e limite; e produz resumo rastreável. Interessados incluem operação, compras, auditoria e gestão.

**Entregas planejadas:** formulação e critérios de sucesso; interessados e restrições; entradas, saídas e regras; decomposição; abstrações e padrões; representações escolhidas; algoritmo com sequência, decisões e repetições; módulos e contratos; tabelas de rastreamento; testes normais, limites e inválidos; correções; comparação de alternativa; limites e justificativa final.

**Prática:** projeto progressivo iniciado em versões pequenas ao longo da fase e integrado nesta aula. A solução principal permanece em pseudocódigo e artefatos independentes de linguagem.

**Cuidado:** não avaliar aparência do diagrama ou extensão do texto como substitutos de coerência. A aula prepara implementação futura, sem criar código ou antecipar COBOL.

## Verificação da progressão

Cada aula introduz uma dificuldade nova: conceituar, formular, decompor, abstrair, generalizar, representar, algoritmizar, rastrear, decidir, iterar, modularizar, testar, comparar e integrar. A progressão não requer programação prévia; prática e matemática crescem junto com a necessidade conceitual.
