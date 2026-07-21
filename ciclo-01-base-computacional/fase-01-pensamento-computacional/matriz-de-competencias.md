# Matriz de Competências — Fase 1

## Leitura da matriz

As competências agrupam os 24 resultados de aprendizagem em desempenhos observáveis. “Introdução” indica a primeira aula que ensina deliberadamente a competência; “desenvolvimento” indica onde ela é retomada com dificuldade adicional. Os níveis cognitivos usam a progressão recordar, compreender, aplicar, analisar, avaliar e criar. O nível mínimo de domínio remete a `criterios-de-dominio.md`.

| ID | Competência e descrição | Introdução | Desenvolvimento | Evidência de domínio | Cognitivo | Pré-requisitos | Erro comum | Recuperação | Mín. |
|---|---|---:|---|---|---|---|---|---|---:|
| C01 | **Formular o problema:** separar situação, necessidade, problema, sintoma, hipótese de causa, objetivo, interessado, escopo e restrição. | 02 | 03, 06, 12, 14 | reformulação de caso ambíguo com justificativa e questões ainda abertas | analisar | vocabulário de sistema, requisito e erro da Fase 0 | tratar sintoma ou solução desejada como o problema | comparar três formulações; marcar evidência, inferência e decisão; refazer com feedback | 4 |
| C02 | **Especificar transformação:** declarar estado inicial e desejado, entradas, saídas, regras, recursos, condições e critérios de sucesso. | 02 | 06–12, 14 | ficha de especificação verificável e casos que demonstram sucesso ou fracasso | criar | C01; entrada, processamento e saída | omitir pré-condições ou usar “funcionar” como critério | preencher quadro de lacunas e testar a especificação contra casos fornecidos | 4 |
| C03 | **Decompor e recompor:** dividir por função, dados ou etapas, preservar dependências e mostrar como as partes recompõem o todo. | 03 | 06, 11, 14 | árvore ou quadro de decomposição com dependências, ordem e critério de recomposição | analisar | C01–C02; sistema e componente | criar partes arbitrárias, duplicadas ou desconectadas | decompor mesmo caso por dois critérios e revisar fronteiras | 4 |
| C04 | **Abstrair e modelar:** selecionar aspectos relevantes, omitir de forma controlada, declarar fronteira e nível de detalhe. | 04 | 05–08, 11, 14 | dois modelos do mesmo caso para públicos distintos, com justificativa das omissões | avaliar | C01–C03; fronteira e representação | confundir abstração com vagueza ou apagar exceção crítica | usar exemplos e contraexemplos; listar pergunta, público e informação indispensável | 4 |
| C05 | **Reconhecer padrões e generalizar:** classificar casos, explicitar regra, exceções e condições de validade. | 05 | 07, 09–10, 13–14 | regra geral validada contra exemplos, contraexemplos e caso novo | avaliar | C04; igualdade, diferença e conjuntos simples | generalizar por semelhança superficial | matriz de atributos; procurar contraexemplo; restringir a regra | 4 |
| C06 | **Selecionar representações:** escolher e combinar linguagem natural, tabela, diagrama, fluxograma, modelo de estado e pseudocódigo conforme finalidade. | 06 | 07–14 | representação principal e complementar do mesmo problema, com rastreabilidade e justificativa | avaliar | C02–C05 | escolher pelo formato conhecido ou ornamentar sem informar | converter uma representação em outra e auditar perdas e ambiguidades | 4 |
| C07 | **Formular e explicar algoritmos:** definir classe de entradas, saídas, passos efetivos, condição de término e argumento de por que resolve o problema. | 07 | 08–14 | algoritmo independente de linguagem acompanhado de explicação e limites | criar | C01–C06 | confundir algoritmo com código, exemplo isolado ou intenção vaga | separar contrato, passos e representação; executar manualmente casos pequenos | 4 |
| C08 | **Rastrear sequência e estado:** identificar estados, transições, valores mutáveis, dependências de ordem e invariantes iniciais. | 08 | 09–12, 14 | tabela de rastreamento completa que localiza mudança ou passo incorreto | aplicar/analisar | C07; sequência e registro | narrar o resultado sem registrar estados intermediários | preencher rastreio passo a passo, comparar ordens e conferir invariante | 4 |
| C09 | **Construir decisões completas:** formular proposições e condições, usar comparação, negação, conjunção e disjunção, cobrir alternativas. | 09 | 10–12, 14 | tabela de decisão e pseudocódigo equivalentes, incluindo fronteiras e combinações relevantes | criar | C02, C06–C08; comparação | condição ambígua, sobreposta ou sem caso restante | reescrever condições atômicas; montar tabela verdade ou de decisão reduzida | 4 |
| C10 | **Construir repetições com progresso:** definir coleção ou intervalo, estado inicial, corpo, atualização e parada; usar contador e acumulador. | 10 | 12–14 | rastreamento de iterações que prova progresso em casos normal, vazio e limite | criar | C07–C09; contagem e intervalos | esquecer atualização, parada ou tratamento de coleção vazia | identificar variante de progresso; simular 0, 1 e vários elementos | 4 |
| C11 | **Modularizar e compor:** atribuir responsabilidades, entradas, saídas, contrato, ordem e dependências a módulos coesos. | 11 | 12–14 | mapa de módulos e contratos que permite recompor a solução sem estado oculto relevante | criar | C03, C06–C10 | módulo por conveniência textual, responsabilidade misturada ou acoplamento oculto | cartões de responsabilidade; revisar cada entrada, saída e dependência | 4 |
| C12 | **Projetar testes e depurar:** criar casos normais, limites e inválidos, declarar resultados esperados, comparar observado e esperado e investigar hipóteses. | 12 | 13–14 | conjunto de testes com rastreio de falha, hipótese sustentada e teste de regressão | analisar/avaliar | C02, C07–C11; erro, falha, log e evidência | testar apenas exemplos favoráveis ou corrigir sem localizar causa | usar tabela entrada–esperado–observado–evidência; teste que reproduz e teste de regressão | 4 |
| C13 | **Avaliar correção, eficiência e adequação:** separar propriedades, contar operações, relacionar custo ao tamanho da entrada e comparar limitações. | 13 | 14 | comparação de duas soluções corretas com critérios explícitos de tempo, espaço, clareza, risco e contexto | avaliar | C07–C12; contagem e crescimento | chamar solução rápida de correta ou otimizar antes de medir | primeiro verificar correção; contar pequenos tamanhos; explicitar prioridades do contexto | 4 |
| C14 | **Integrar e defender uma solução:** produzir pacote rastreável do problema aos testes, justificar escolhas e preparar implementação futura. | 14 | — | projeto individual ou contribuição identificável, defesa oral/escrita e revisão após feedback | criar/avaliar | C01–C13 | apresentar artefatos sem coerência ou defender por preferência pessoal | matriz de rastreabilidade, revisão por pares guiada e nova versão justificada | 5 |

## Cobertura dos resultados de aprendizagem

- Resultados 1–3: C01 e C02.
- Resultados 4–7: C03, C04 e C05.
- Resultados 8, 14 e 15: C06.
- Resultados 9 e 10: C07.
- Resultados 11–13: C08, C09 e C10.
- Resultados 16–18: C12.
- Resultados 19–21: C13.
- Resultados 22 e 23: C11.
- Resultado 24: C14.

## Competências essenciais para avanço

C01, C02, C03, C06, C07, C08, C09, C10, C11 e C12 são essenciais: nenhuma pode permanecer abaixo do Nível 4. C04, C05 e C13 também requerem Nível 4, mas uma lacuna localizada pode ser recuperada por tarefa específica antes da conclusão. C14 exige Nível 5 porque a integração deve incluir justificação e comparação, não apenas aplicação.

Autodeclaração, leitura concluída e reprodução literal não constituem evidência suficiente. Toda decisão de domínio deve se apoiar em artefato, explicação, rastreamento, resolução, teste, revisão ou defesa observável.
