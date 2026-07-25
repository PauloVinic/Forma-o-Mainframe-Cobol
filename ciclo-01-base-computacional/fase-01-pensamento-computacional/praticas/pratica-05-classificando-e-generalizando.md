# Prática 05 — Classificar, testar e restringir regras

## Objetivo e modalidades

Construir classificação e regra provisória a partir de casos, procurar contraexemplos, restringir domínio e aplicar a casos novos. A prática usa estoque como núcleo e transações como transferência opcional, preservando desconhecidos, classes sobrepostas e a separação entre classificação e decisão.

Na **trilha essencial**, percorra os nove blocos usando dez casos iniciais, quatro reservados para examinar a primeira regra e três casos novos; a transferência é opcional. Produza classificação, sobreposição, padrão, regra, contraexemplo, revisão e autoavaliação. Tempo: **3h–4h15**.

No **aprofundamento opcional**, acrescente segunda classificação, partição ou função, dois padrões concorrentes, conjunto ampliado, caso limítrofe, transferência completa e análise de consequências. Não é requisito para avançar.

## Bloco 1 — Declarar o recorte

Preencha antes de classificar:

| Dimensão | Declaração |
|---|---|
| pergunta |  |
| unidade de comparação |  |
| universo |  |
| atributos escolhidos |  |
| atributos desconhecidos |  |
| período e definições |  |
| uso permitido |  |
| uso proibido |  |

Use como pergunta inicial: “Que ocorrências hipotéticas podem ser tratadas conjuntamente para investigar qualidade de registro, divergência e impacto, sem inferir causa nem decidir intervenção?”

## Bloco 2 — Matriz hipotética de casos

Os 14 casos são didáticos e não acrescentam fatos ao projeto. `C` = completo/conhecido; `I` = incompleto; `D` = desconhecido. Use primeiro somente E1–E10 para formular classes e regra. E11–E14 ficam reservados ao Bloco 6.

| Caso | Centro | Produto | Histórico | Divergência | Condição física | Impacto | Ação posterior |
|---|---|---|---|---|---|---|---|
| E1 | A | P1 | C | registrada | conhecida | baixo | revisar registro |
| E2 | A | P2 | I | desconhecida | desconhecida | alto | obter evidência |
| E3 | B | P2 | C | não registrada | conhecida | baixo | acompanhar |
| E4 | B | P3 | I | registrada | conhecida | médio | investigar |
| E5 | A | P3 | C | registrada | desconhecida | alto | investigar |
| E6 | B | P1 | D | desconhecida | desconhecida | alto | obter evidência |
| E7 | A | P2 | C | não registrada | conhecida | médio | acompanhar |
| E8 | B | P2 | I | não registrada | conhecida | baixo | completar histórico |
| E9 | A | P1 | C | registrada | conhecida | alto | investigar |
| E10 | B | P3 | C | não registrada | conhecida | médio | acompanhar |
Não antecipe os reservados. E2 e E6 não confirmam nem negam divergência; E4 permite sobreposição. No aprofundamento, classifique os 14 simultaneamente e examine limites de impacto.

## Bloco 3 — Classificação

Proponha de três a cinco classes. No essencial, classifique E1–E10, mantenha desconhecidos e indique sobreposição.

| Classe | Critério de pertencimento | Casos | Pode sobrepor? | Informação insuficiente |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

Classes possíveis, sem obrigação de copiar: qualidade de registro comprometida; divergência registrada; impacto alto; evidência suficiente para a pergunta; ainda não classificável. Evite “outros” sem critério.

Identifique a dimensão: as três primeiras são classes analíticas; “pendente quanto à divergência” é estado informacional usado operacionalmente. Ele pode coexistir com classes analíticas e não descreve causa.

Depois verifique:

- todos os casos do universo continuam visíveis?
- alguma classe foi forçada a ser exclusiva?
- desconhecido foi confundido com “não”?
- os rótulos descrevem atributo ou insinuam causa/decisão?

Registre ainda uma justificativa de 100–150 palavras. Explique por que escolheu classificação sobreposta ou exclusiva, que caso foi mais difícil e como tratou informação ausente. Se duas classes repetirem o mesmo critério com nomes diferentes, consolide-as. Se uma classe depender da ação posterior, verifique se ela está descrevendo o caso ou apenas reproduzindo uma decisão já tomada.

## Bloco 4 — Padrões candidatos

Na trilha essencial, desenvolva um padrão. No aprofundamento, desenvolva dois.

| Elemento | Padrão 1 | Padrão 2 opcional |
|---|---|---|
| declaração |  |  |
| atributos |  |  |
| domínio |  |  |
| casos favoráveis |  |  |
| casos contrários |  |  |
| desconhecidos |  |  |
| risco de interpretação |  |  |
| utilidade |  |  |

Use linguagem como “no conjunto examinado, aparece...” e não “causa”. Repetição sem pergunta relevante não basta.

## Bloco 5 — Regra candidata

Formule uma regra em linguagem natural:

| Componente | Registro |
|---|---|
| domínio |  |
| condições |  |
| conclusão |  |
| evidência favorável |  |
| desconhecidos |  |
| uso permitido |  |
| uso proibido |  |

A regra pode descrever ou classificar. Identifique qual tipo. Não crie procedimento, sequência de ações ou decisão automática.

## Bloco 6 — Contraexemplo e revisão

Somente agora revele os reservados:

| Caso | Centro | Produto | Histórico | Divergência | Condição | Impacto |
|---|---|---|---|---|---|---|
| E11 | A | P3 | I | desconhecida | desconhecida | baixo |
| E12 | B | P1 | C | registrada | conhecida | baixo |
| E13 | A | P2 | C | não registrada | conhecida | alto |
| E14 | B | P3 | I | registrada | desconhecida | alto |

No essencial, localize um contraexemplo da formulação universal e um desconhecido. No aprofundamento, identifique também:

- um contraexemplo dentro do domínio;
- uma possível exceção somente se tiver condição prévia e justificável;
- um caso fora do domínio;
- um caso desconhecido.

| Caso | Tipo | Por que | Efeito sobre a regra |
|---|---|---|---|
|  | contraexemplo |  |  |
|  | exceção ou não |  |  |
|  | fora do domínio |  |  |
|  | desconhecido |  |  |

Escolha: restringir domínio, alterar condição ou rejeitar regra. Não transforme o contraexemplo em exceção apenas para preservar a formulação inicial.

Antes de revisar, confirme que o dado contrário é conhecido e que o caso realmente pertence ao domínio. Depois registre a versão:

| Versão | Regra | Domínio | Evidência contrária | Uso que permanece permitido |
|---|---|---|---|---|
| inicial |  |  |  |  |
| revista ou rejeitada |  |  |  |  |

Uma regra rejeitada é resultado legítimo. Não crie detalhes específicos de E8 ou E13 apenas para memorizar o conjunto.

## Bloco 7 — Casos novos

Estes casos não participaram da formulação:

| Caso | Centro | Produto | Histórico | Divergência | Condição | Impacto |
|---|---|---|---|---|---|---|
| N1 | A | P2 | I | registrada | conhecida | médio |
| N2 | B | P3 | C | não registrada | desconhecida | alto |
| N3 | A | P1 | D | desconhecida | desconhecida | baixo |
| N4 | B | P2 | C | registrada | conhecida | alto |

No essencial, use N1–N3; N4 fica no aprofundamento. Classifique, aplique a regra revista, recuse conclusão quando faltar informação e avalie sustentação. N2 examina regras que ligam impacto a divergência; N3 exige estado pendente.

| Caso novo | Classes | Regra aplicável? | Resultado ou pendência | Efeito sobre a regra |
|---|---|---|---|---|
| N1 |  |  |  |  |
| N2 |  |  |  |  |
| N3 |  |  |  |  |
| N4 |  |  |  |  |

Não altere a regra antes de registrar o resultado. Se a revisar novamente, preserve as duas versões.

## Bloco 8 — Transferência opcional para transações

Casos hipotéticos:

| Transação | Valor | Autorização | Contestação | Cadastro |
|---|---:|---|---|---|
| T1 | R$ 15.000 | confirmada | não registrada | completo |
| T2 | R$ 800 | desconhecida | registrada | completo |
| T3 | R$ 12.000 | desconhecida | desconhecida | completo |
| T4 | R$ 20.000 | confirmada | não registrada | incompleto |

No aprofundamento opcional, identifique a semelhança superficial “valor alto”, produza contraexemplo para “valor alto = fraude”, proponha classe descritiva, preserve desconhecidos e explique por que classificação não decide bloqueio. Esta transferência não integra a entrega essencial.

## Bloco 9 — Revisão após solução

Depois de consultar os comentários, revise uma classe e uma regra:

| Artefato | Antes | Depois | Evidência | Mudança no domínio | Consequência |
|---|---|---|---|---|---|
| classe |  |  |  |  |  |
| regra |  |  |  |  |  |

Explique quem pode ser afetado por rótulo ou regra, como contestar e que evidência exigiria nova revisão.

## Entrega esperada

Entregue recorte, dez casos iniciais classificados, critérios, padrão, regra, exame dos reservados, contraexemplo, regra revista ou rejeitada, três casos novos, revisão e autoavaliação.

No aprofundamento, acrescente somente os itens opcionais escolhidos. A quantidade não substitui justificativa.

Mantenha versões inicial e revista identificáveis; uma entrega apenas final não demonstra como a evidência alterou o raciocínio.

## Solução comentada — consulte somente depois da tentativa

Não existe classificação única. Uma possibilidade sobreposta usa:

- **qualidade de registro comprometida:** E2, E4 e E8 inicialmente; E11 e E14 após revelar os reservados; E6 permanece desconhecido;
- **divergência registrada:** E1, E4, E5, E9, E12 e E14;
- **impacto alto:** E2, E5, E6, E9, E13 e E14;
- **pendente quanto à divergência:** estado informacional de E2, E6 e, depois, E11.

E4 e E14 pertencem a mais de uma classe. Isso não é defeito se o objetivo examina dimensões diferentes. “Pendente” preserva insuficiência sem inventar valor.

O padrão “impacto alto acompanha divergência” deve virar regra examinável: “toda ocorrência de impacto alto possui divergência registrada”. E5/E9 favorecem inicialmente; E13, revelado depois, é contraexemplo; E2/E6 são desconhecidos. A regra universal deve ser rejeitada ou revista com justificativa. Uma descrição frequencial exigiria contagens e denominadores e não é confirmada por esse contraste.

Nos casos novos, N1 pertence a qualidade e divergência; N2 pertence a impacto alto e contraria a regra ampla; N3 permanece pendente para histórico e divergência; N4 pertence a divergência e impacto. Outras classes são aceitáveis com critérios.

Nas transações, T1 é contraexemplo à equivalência entre valor alto e fraude; T2 mostra sinal relevante em valor baixo; T3 contém desconhecidos; T4 sobrepõe valor alto e cadastro incompleto. “Valor alto” pode ser classe descritiva, não decisão. Nenhuma ocorrência estabelece causa.

Compare com sua tentativa sem copiar rótulos. Uma revisão forte explica por que alterou critério ou domínio e que consequência reduziu.

Uma classificação exclusiva também seria possível para outro propósito, desde que declare prioridade entre critérios e preserve as dimensões perdidas. Por exemplo, escolher uma única “situação principal” não autoriza apagar impacto ou incompletude; esses atributos continuam disponíveis. Essa alternativa custa informação e precisa justificar por que a decisão exige exclusividade.

Se a regra escolhida for “histórico incompleto acompanha divergência”, E8 é contraexemplo conhecido e E2/E11 permanecem desconhecidos. Não conte desconhecidos como favoráveis. Se a regra tratar apenas casos com divergência conhecida, declare a restrição e reconheça que o conjunto menor não representa automaticamente todos os 14 casos.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| unidade | mistura escalas | declara caso | sustenta a pergunta |
| atributos | usa disponibilidade | seleciona por propósito | distingue desconhecido e rótulo |
| comparabilidade | ignora definições | verifica contexto | limita comparações |
| critérios | rótulos vagos | pertencimento explícito | entrada e saída explicáveis |
| pertencimento | arbitrário | aplica critério | trata limites |
| desconhecidos | converte em não | mantém visível | informa efeito |
| sobreposição | força exclusividade | permite quando útil | justifica dimensões |
| regularidade | confunde repetição | identifica recorrência | considera base de comparação |
| padrão | afirma universal | declara candidato | limita domínio |
| regra | vira decisão | declara tipo e uso | separa descrição e norma |
| contraexemplo | ignora caso | procura deliberadamente | revisa ou rejeita |
| exceção | protege regra | exige condição | distingue fora do domínio |
| domínio | implícito | declara conjunto | registra exclusões |
| caso novo | força resposta | admite insuficiência | avalia sustentação |
| revisão | copia solução | muda por evidência | registra consequência |
| consequência | ausente | identifica afetados | prevê contestação |

O essencial está concluído quando nenhum critério está em “precisa de revisão” e você consegue explicar por que um exemplo favorável não prova a regra, como o contraexemplo mudou o domínio e por que desconhecido não é negativo.

## Carga

- Prática essencial: 3h–4h15.
- Solução, revisão e autoavaliação: 30–45 min.
- Aprofundamento opcional da prática: 2h–3h adicionais.
- Trilha integrada com aula e exercícios essenciais: aproximadamente 7h20–9h45.
- Percurso completo opcional: aproximadamente 10h30–14h, incluindo 14 casos simultâneos, segundo padrão e regra, N4, transferência, matemática e consequências.
