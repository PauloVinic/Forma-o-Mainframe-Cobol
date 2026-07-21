# Glossário da Fase 1 — Pensamento Computacional

As definições são operacionais para esta fase. Quando um termo possui formulações diferentes entre áreas, a aula correspondente deverá apresentar a variação relevante e declarar a convenção adotada. O glossário complementa, sem substituir, as explicações e o glossário da Fase 0.

## Formulação de problemas

**Pensamento computacional:** conjunto de perspectivas e práticas para formular problemas e desenvolver soluções que possam ser representadas, examinadas e, quando adequado, executadas por um agente humano ou computacional. Não é sinônimo de programação e não possui uma única decomposição consensual em “pilares”.

**Situação:** contexto observado que reúne fatos, participantes, condições e acontecimentos; pode conter problemas, mas não é automaticamente uma formulação de problema.

**Problema:** diferença ou obstáculo relevante entre um estado inicial e um estado desejado, delimitado por objetivos, condições e critérios que permitam examinar uma solução.

**Sintoma:** manifestação observável associada a um problema ou falha; indica que algo merece investigação, mas não identifica sozinho a causa.

**Causa:** condição ou evento que contribui para produzir um efeito. Nesta fase, deve ser distinguida de hipótese de causa, que ainda precisa de evidência.

**Objetivo:** estado ou resultado que se pretende alcançar. Um objetivo útil é suficientemente claro para orientar decisões e verificar sucesso.

**Interessado:** pessoa, grupo ou organização que influencia a solução, é afetado por ela ou possui responsabilidade relevante sobre o problema.

**Escopo:** fronteira que declara o que será tratado e o que ficará fora da solução atual.

**Restrição:** condição que limita soluções admissíveis, como prazo, recurso, regra, capacidade, segurança ou formato obrigatório.

**Critério de sucesso:** condição observável usada para decidir se o objetivo foi atingido no escopo declarado.

**Recurso:** meio disponível ou necessário para executar uma solução, como tempo, pessoas, dados, memória, equipamento ou autorização.

**Ambiguidade:** possibilidade de uma expressão ou representação sustentar mais de uma interpretação relevante sem indicar qual é pretendida.

## Estruturação e modelagem

**Decomposição:** divisão orientada de um problema ou solução em partes menores, preservando responsabilidades, relações, dependências e possibilidade de recomposição.

**Recomposição:** integração das partes decompostas para verificar se, juntas, atendem ao objetivo do todo.

**Dependência:** relação na qual uma parte, decisão ou etapa precisa de resultado, condição ou recurso fornecido por outra.

**Abstração:** seleção intencional de aspectos relevantes para um propósito, com omissão controlada de detalhes que não precisam ser considerados naquele nível.

**Modelo:** construção deliberada que representa certos aspectos de algo para descrever, explicar, prever ou decidir. Todo modelo possui propósito, fronteira e limites.

**Fronteira:** separação conceitual entre o que pertence ao objeto ou modelo em análise e o que é tratado como ambiente externo.

**Padrão:** regularidade ou estrutura recorrente reconhecida por critérios explícitos entre casos, dados ou processos.

**Classificação:** atribuição de elementos a classes segundo propriedades e regras declaradas.

**Generalização:** formulação de regra ou solução aplicável a uma classe de casos além dos exemplos originais, com condições de validade e exceções registradas.

**Exemplo:** caso que satisfaz uma definição, regra ou propriedade e ajuda a compreendê-la.

**Contraexemplo:** caso que contradiz uma afirmação geral e mostra que ela precisa ser rejeitada, limitada ou reformulada.

**Representação:** forma escolhida para expressar informações sobre problema, modelo, estado ou solução. Não é necessariamente o objeto representado.

## Algoritmos e controle

**Algoritmo:** procedimento preciso, composto de passos efetivos, que transforma entradas admissíveis em saídas esperadas para uma classe delimitada de problemas e possui condição de término quando a tarefa exige conclusão.

**Heurística:** estratégia prática que orienta busca ou decisão e pode produzir solução útil, mas não oferece necessariamente as mesmas garantias de correção, completude ou qualidade de um algoritmo especificado.

**Entrada:** dado, evento, condição ou recurso fornecido a um procedimento para ser usado no processamento. Retoma a Fase 0 e acrescenta o papel no contrato do algoritmo.

**Saída:** resultado observável produzido por um procedimento, conforme formato e significado esperados.

**Pré-condição:** condição que deve valer antes da execução de um procedimento para que seu contrato seja aplicável.

**Pós-condição:** condição que o procedimento se compromete a estabelecer ao terminar corretamente, dadas as pré-condições.

**Estado:** conjunto de informações relevantes que descreve a situação de um processo ou sistema em determinado momento.

**Transição:** passagem de um estado a outro causada por ação, evento ou regra.

**Sequência:** ordem definida de elementos ou passos. Em algoritmo, a ordem pode determinar estados e resultados diferentes.

**Variável:** representação conceitual nomeada de um valor que pode variar entre estados durante um procedimento. A definição será refinada quando linguagens e memória forem estudadas.

**Invariante:** propriedade que permanece verdadeira nos pontos relevantes de uma execução, apesar de mudanças de estado. Nesta fase, é usada intuitivamente para auxiliar rastreamento e correção.

**Condição:** expressão cujo resultado orienta decisão, continuidade ou parada; deve ser interpretável como verdadeira ou falsa no contexto definido.

**Proposição:** enunciado declarativo ao qual se pode atribuir valor lógico verdadeiro ou falso sob interpretação definida.

**Valor lógico:** um dos valores usados para representar verdade de uma proposição; nesta fase, verdadeiro e falso.

**Negação:** operação lógica que inverte o valor de verdade de uma proposição.

**Conjunção:** combinação lógica verdadeira quando todas as proposições combinadas são verdadeiras.

**Disjunção:** nesta fase, combinação lógica inclusiva verdadeira quando pelo menos uma das proposições é verdadeira.

**Decisão:** seleção de um caminho ou ação entre alternativas com base em uma ou mais condições.

**Repetição:** estrutura em que um conjunto de passos pode ser executado mais de uma vez.

**Iteração:** uma execução particular do corpo de uma repetição; o termo também pode designar o processo repetitivo como um todo conforme o contexto.

**Condição de parada:** condição que determina quando uma repetição ou busca deve terminar.

**Progresso:** mudança mensurável que aproxima uma repetição de sua condição de parada.

**Contador:** estado numérico atualizado para registrar quantas ocorrências, elementos ou iterações foram considerados.

**Acumulador:** estado atualizado sucessivamente para combinar valores, como uma soma ou total parcial.

## Modularização

**Módulo:** parte delimitada de uma solução com responsabilidade, entradas, saídas e dependências identificáveis.

**Procedimento:** conjunto nomeado de passos que realiza uma tarefa e pode produzir efeitos ou resultados segundo um contrato.

**Função:** nesta fase, procedimento ou relação que associa entradas a um resultado, com ênfase no valor produzido. Definições matemáticas e de linguagens serão aprofundadas posteriormente.

**Parâmetro:** elemento nomeado do contrato por meio do qual um módulo recebe um valor ou referência necessária à sua tarefa.

**Contrato:** declaração das responsabilidades de uma parte, incluindo entradas, pré-condições, saídas, pós-condições e efeitos relevantes.

**Coesão:** grau em que os elementos de um módulo contribuem para uma responsabilidade relacionada. É introduzida qualitativamente.

**Acoplamento:** grau de dependência entre módulos. É introduzido qualitativamente, sem arquitetura avançada.

**Composição:** construção de solução maior pela combinação coordenada de partes ou procedimentos.

## Representações operacionais

**Pseudocódigo:** notação textual didática, independente de uma linguagem específica, usada para representar algoritmos com clareza e consistência.

**Fluxograma:** diagrama que usa símbolos e conexões para representar fluxo de passos, decisões e repetições. É uma representação possível, não o algoritmo em si.

**Tabela de decisão:** tabela que relaciona combinações de condições a ações ou resultados, ajudando a verificar completude e sobreposição de regras.

**Modelo de estado:** representação dos estados relevantes, transições possíveis e condições ou eventos associados.

**Tabela de rastreamento:** registro tabular dos passos, condições, valores e saídas intermediárias de uma execução manual.

## Verificação e escolha

**Teste:** atividade planejada que aplica casos e compara comportamento observado com resultado esperado para produzir evidência sobre uma solução.

**Caso de teste:** especificação de entradas, condições de execução, passos pertinentes e resultados esperados para um cenário determinado.

**Caso normal:** caso representativo do uso esperado, sem estar especialmente próximo de uma fronteira ou violar uma regra.

**Caso limite:** caso situado em fronteira relevante, como mínimo, máximo, vazio, primeiro, último ou ponto de mudança de condição.

**Entrada inválida:** entrada que não satisfaz formato, domínio ou pré-condição declarada e deve receber tratamento definido.

**Resultado esperado:** comportamento ou saída declarado antes da verificação, derivado do contrato e das regras, usado como referência de comparação.

**Defeito:** problema existente em requisito, modelo, algoritmo, representação ou implementação que pode causar falha. Mantém a distinção operacional iniciada na Aula 12 da Fase 0.

**Falha:** comportamento observado que se desvia do esperado; é manifestação, não sinônimo automático de causa.

**Depuração:** investigação sistemática destinada a localizar e compreender defeitos a partir de sintomas, hipóteses, rastreamentos e evidências, seguida de correção e nova verificação.

**Regressão:** reaparecimento de defeito ou perda de comportamento previamente correto após mudança. Teste de regressão busca detectar esse tipo de efeito.

**Correção:** propriedade de uma solução que satisfaz a especificação para o domínio e as condições declaradas. Um conjunto finito de testes apoia evidência, mas geralmente não prova correção universal.

**Eficiência:** relação entre trabalho realizado e recursos consumidos por uma solução, como tempo, espaço e número de operações.

**Adequação:** compatibilidade da solução com objetivos, restrições, riscos, público e ambiente de uso, além de sua correção e eficiência.

**Custo:** recurso consumido ou consequência assumida por uma estratégia; pode incluir operações, tempo, espaço, manutenção, risco ou esforço humano.

**Complexidade:** nesta fase, noção de como necessidades de recursos crescem em relação ao tamanho da entrada. A análise assintótica formal será estudada depois.

**Tamanho da entrada:** medida escolhida para representar a escala do problema, como número de registros, itens ou transações.

**Escalabilidade:** capacidade de manter comportamento aceitável quando o tamanho da entrada ou a demanda cresce, dentro de critérios declarados.
