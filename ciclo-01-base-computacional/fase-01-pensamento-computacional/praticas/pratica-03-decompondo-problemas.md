# Prática 03 — Três decomposições do mesmo problema

## Identificação

- **Ciclo:** 1 — Base Computacional
- **Fase:** 1 — Pensamento Computacional
- **Aula associada:** Aula 03 — Decomposição de problemas
- **Competência:** C03 — decompor, preservar dependências e recompor
- **Caso:** concessão do Benefício de Apoio Temporário
- **Produto:** três decomposições comparáveis, mapa de dependências, recomposição e revisão

## Objetivo

Você examinará o mesmo problema por três critérios: funções, dados ou objetos de atenção e etapas ou eventos. Depois comparará o que cada divisão torna visível, registrará dependências e testará se as partes podem ser recompostas sem perder prazo, correção, rastreabilidade, confidencialidade, acesso e contestação.

A atividade não pede solução técnica, automação, código, pseudocódigo, fluxo formal nem estrutura de software. O objetivo é justificar uma divisão analítica. Há mais de uma resposta adequada, desde que o todo permaneça o mesmo e critérios, fronteiras, dependências e consequências sejam explícitos.

## Orientações

Faça os Blocos 1 a 7 antes de consultar a solução comentada. Use a modalidade **essencial** para uma primeira demonstração de domínio; use o **aprofundamento** para testar granularidades e alternativas. Marque incertezas em vez de inventar dados. Rótulos como “análise” ou “documentos” precisam de uma frase que delimite seu papel.

Cada decomposição deve usar um critério principal. Partes de critérios diferentes podem aparecer em níveis distintos, desde que isso seja declarado. Setas devem ter rótulo: “fornece informação”, “requer decisão”, “restringe” ou outro significado preciso. Uma seta sem rótulo não informa se existe ordem, dependência ou causalidade.

## Caso — Benefício de Apoio Temporário

O programa hipotético recebeu **1.000 solicitações em 20 dias úteis**. A coorte foi acompanhada até a primeira decisão autorizada, sua comunicação e, quando apresentada no prazo, a contestação e a reanálise. Destas, 620 tiveram primeira decisão em até cinco dias úteis e 380 ultrapassaram esse prazo: `620 + 380 = 1.000`, ou 62% e 38%.

Entre as 380 solicitações demoradas, 210 passaram por pendência documental, 140 foram reatribuídas e 90 atravessaram uma indisponibilidade de três horas. As categorias podem se sobrepor; por isso, `210 + 140 + 90 > 380` não é contradição. Os números também não estabelecem relação causal. Em 54 casos não houve nova ação por mais de dois dias depois que os documentos foram marcados como recebidos.

As primeiras decisões foram 760 concessões e 240 negativas. Das negativas, 72 foram contestadas. Após reanálise, 24 decisões mudaram: 15 por nova evidência admitida e nove por correção de erro interno. Assim, `24 ≤ 72 ≤ 240`. Em 48 decisões não havia tentativa de comunicação registrada até dois dias úteis depois da decisão.

Uma solicitação pode estar recebida, com pendência, em análise, aguardando decisão autorizada, concedida ou negada. A contestação tem estados próprios: recebida, em reanálise e decidida. Solicitação e contestação não são o mesmo objeto.

Regras hipotéticas do recorte:

- identidade, residência e condição de renda precisam ser sustentadas por documento ou forma equivalente admitida;
- item ausente ou ilegível gera pendência identificada, com prazo; não gera negativa automática antes do prazo;
- a análise registra regras aplicadas e conclusão recomendada;
- somente papel autorizado pode conceder ou negar;
- a decisão registra resultado e fundamento;
- a comunicação informa decisão, fundamento, prazo e meio de contestação;
- contestação apresentada em até dez dias úteis da comunicação pode trazer nova evidência e retorna para análise;
- nova evidência e correção de erro interno precisam permanecer distinguíveis.

O objetivo é reduzir tempo e interrupções até uma decisão válida, preservando aplicação das regras, rastreabilidade, confidencialidade, acesso e contestação. A meta candidata é que ao menos 90% das solicitações de cada um de três ciclos recebam primeira decisão autorizada em até cinco dias úteis, com população e método comparáveis. Todas as negativas devem registrar fundamento e orientação para contestar; revisões por erro interno não podem ultrapassar 1% da coorte.

Durante os três ciclos, as regras não podem ser alteradas e não haverá aumento de equipe. Dados sensíveis só podem ser acessados por papéis autorizados, o canal não digital deve permanecer e a atividade não escolherá sistema, automação ou reorganização. Solicitantes, representantes, pessoas com dificuldade de acesso digital, atendimento, analistas, autoridade decisória, responsáveis pela contestação, auditoria e responsáveis pelas regras são interessados ou afetados.

Permanecem abertas a interpretação de documentos equivalentes, a definição de comunicação efetiva, diferenças entre canais, os motivos das reatribuições e a responsabilidade pela divergência entre documento marcado como recebido e documento disponível ao analista.

## Bloco 1 — Reconstruir o todo

Em **120 a 180 palavras**, registre somente:

1. o todo analisado e a finalidade da decomposição;
2. o estado atual, o estado desejado e o objetivo;
3. escopo, critérios globais e restrições que não podem desaparecer;
4. duas a quatro questões abertas capazes de alterar a decomposição.

Não refaça a ficha completa da Aula 02. O todo não é “todo o programa social”, e preencher campos que não ajudam a próxima decisão não demonstra domínio.

## Bloco 2 — Decomposição funcional

Declare o critério funcional em uma frase. Na modalidade essencial, identifique de cinco a sete funções; no aprofundamento, divida duas delas em subpartes.

| Função | Finalidade | Informação necessária | Resultado parcial | Dependências |
|---|---|---|---|---|
|  |  |  |  |  |

Depois, indique uma lacuna possível, uma função ampla ou estreita demais e seu critério de parada. Confirme que as funções respondem “o que precisa ocorrer?” e não foram copiadas de departamentos ou transformadas em elementos de software.

## Bloco 3 — Decomposição por dados ou objetos

Selecione seis objetos na modalidade essencial. No aprofundamento, acrescente dois e examine uma divergência de significado.

| Objeto tratado | Significado no caso | Origem | Uso | Quem atualiza | Partes dependentes e divergência possível |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

Objeto, aqui, não significa tabela, arquivo, banco de dados ou estrutura técnica. Solicitação, documento, pendência, regra, análise, decisão, comunicação e contestação são candidatos, não um gabarito obrigatório. Explique por que cada escolha importa ao todo.

## Bloco 4 — Decomposição por etapas ou eventos

Identifique de seis a oito momentos ou eventos. Não presuma percurso único.

| Momento ou evento | Estado ou condição anterior e posterior | Informação necessária | Dependência relevante | Retorno ou exceção |
|---|---|---|---|---|
|  |  |  |  |  |

Inclua um par de atividades que possa ocorrer em paralelo, uma ordem apenas cronológica sem dependência necessária, um retorno justificado e uma exceção. Explique em duas frases por que seu quadro não é algoritmo nem fluxo obrigatório. No aprofundamento, compare duas granularidades possíveis de uma etapa.

## Bloco 5 — Comparar os critérios

Preencha exatamente três linhas:

| Critério | O que evidencia | O que deixa menos visível | Vantagem | Risco | Pergunta atendida | Complemento necessário |
|---|---|---|---|---|---|---|
| funcional |  |  |  |  |  |  |
| dados/objetos |  |  |  |  |  |  |
| etapas/eventos |  |  |  |  |  |  |

Escolha qual decomposição usaria como principal para investigar os 54 casos sem nova ação e justifique pela pergunta, não por preferência pessoal. Outra escolha pode ser válida quando explicita seus limites e o complemento necessário.

## Bloco 6 — Construir o mapa de dependências

Escolha uma decomposição como base. Registre pelo menos seis partes e sete dependências.

| Origem → destino | O que atravessa a interface | Natureza ou condição | Consequência se faltar |
|---|---|---|---|
|  |  |  |  |

O mapa precisa conter dependência condicional, elemento transversal e possível retorno. Para cada linha, identifique origem, destino, conteúdo, natureza — por exemplo informacional, decisória, regulatória, de estado ou de ordem — e consequência da ausência. Interface significa interação na fronteira, não tela. Um retorno não transforma o mapa em procedimento formal e não demonstra causa.

## Bloco 7 — Recompor e avaliar

Produza quatro resultados:

1. verifique a cobertura de solicitação, documentos, pendência, análise, decisão, comunicação e contestação;
2. identifique uma lacuna, uma duplicidade problemática e uma sobreposição legítima;
3. registre uma interface ambígua e um risco de otimização local;
4. escreva **140 a 200 palavras** explicando como resultados parciais recompõem o objetivo global.

O texto deve mencionar critérios globais, pessoas afetadas e ao menos uma propriedade do todo: tempo total, rastreabilidade, confidencialidade ou capacidade de contestação. Se a recomposição falhar, diga se revisaria parte, critério, granularidade, dependência ou o próprio todo.

## Entrega esperada

Entregue um documento com o registro breve do todo, os três quadros de decomposição, a comparação, o mapa com pelo menos sete dependências e a recomposição. Depois de consultar a solução, anexe a revisão justificada do Bloco 8 e marque seu nível nos 12 critérios de autoavaliação. Indique a modalidade realizada e as questões abertas. Qualidade não será medida pelo maior número de partes, e sim por coerência, cobertura, relações preservadas e capacidade de revisão.

## Organização do tempo

| Etapa | Essencial | Com aprofundamento |
|---|---:|---:|
| leitura do caso | 15–20 min | 20–25 min |
| Bloco 1 | 15–20 min | 20–25 min |
| decomposição funcional | 35–45 min | 45–60 min |
| decomposição por dados | 35–45 min | 45–60 min |
| decomposição por etapas | 35–45 min | 45–60 min |
| comparação | 20–25 min | 25–35 min |
| mapa | 30–40 min | 40–50 min |
| recomposição | 25–35 min | 35–45 min |
| consulta da solução | 15–20 min | 20–25 min |
| revisão e autoavaliação | 20–25 min | 25–35 min |
| **total** | **4h05–5h20** | **5h20–7h00** |

Os totais não incluem pausas longas. Divida a prática em duas ou três sessões; não sacrifique a recomposição para terminar de uma vez.

# Solução comentada — consulte somente depois da tentativa

O que segue é uma possibilidade proporcional, não uma decomposição única. Ela comenta decisões centrais e deixa células sem preenchimento para que a prática não vire cópia mecânica.

No Bloco 1, o todo pode ser descrito como o problema de reduzir demora e interrupções desde o recebimento das 1.000 solicitações até a decisão autorizada e sua comunicação, preservando a eventual contestação e reanálise, regras, acesso e registros. Os 54 casos orientam uma pergunta, mas não substituem o todo nem demonstram causa. Questões sobre documento disponível, reatribuição e comunicação podem alterar fronteiras e dependências.

Uma decomposição funcional possível contém: registrar solicitação; verificar suficiência documental; tratar pendências; analisar elegibilidade; produzir decisão autorizada; comunicar decisão e direitos; examinar contestação. “Produzir decisão” foi separada de “analisar” porque recomendação e autorização têm responsabilidades distintas. “Tratar pendência” pode ser detalhada em registrar itens, comunicar prazo e associar complementação, mas não é necessário descrever ações de tela.

Por objetos de atenção, uma seleção possível é: solicitante, solicitação, documento, pendência, regra, análise, decisão, comunicação e contestação. Documento marcado como recebido não equivale a documento legível ou disponível. Análise e decisão são resultados distintos. A contestação possui estado próprio e pode gerar nova análise sem apagar a decisão anterior. Essas distinções são do domínio, não um desenho de dados.

Por momentos ou eventos, podemos registrar recebimento, verificação documental, identificação e comunicação de pendência, chegada de complemento, retomada da análise, decisão, comunicação e eventual contestação com reanálise. Há retorno e caminhos condicionais. Preparar informação geral de comunicação pode ocorrer em paralelo à análise, embora a comunicação individual dependa de decisão autorizada. Portanto, a lista não é algoritmo obrigatório.

Uma comparação razoável diria que a visão funcional evidencia contribuições e responsabilidades; a visão por objetos evidencia significado e mudanças da informação; a visão por etapas evidencia espera, retorno e condição. Para os 54 casos, etapas/eventos podem ser a visão principal porque localizam a interrupção entre recebimento marcado e nova ação. Dados/objetos são complemento indispensável para distinguir o que “recebido” significa. Escolher objetos como visão principal também seria defensável com essa justificativa invertida.

Um mapa selecionado pode conter:

1. registro → verificação: fornece solicitação e referências dos documentos;
2. verificação → tratamento de pendência: fornece itens ausentes ou ilegíveis e prazo, **se** houver pendência;
3. resposta à pendência → análise: fornece documentos e condição atualizada;
4. análise → decisão: fornece conclusão, regras aplicadas e base registrada;
5. decisão → comunicação: fornece resultado, fundamento e direitos;
6. comunicação → contestação: fornece conteúdo e data que sustentam o prazo;
7. contestação → análise: fornece alegação e nova evidência, criando retorno;
8. confidencialidade e rastreabilidade → todas as partes: restringem acesso e exigem preservação dos registros.

Uma lacuna possível é não definir qual registro sustenta que o documento ficou disponível. Há duplicidade problemática se análise e decisão aplicarem versões diferentes da regra sem coordenação. A regra atravessar análise, decisão e contestação é sobreposição legítima. Reduzir o tempo local devolvendo todo caso duvidoso pode piorar o tempo total, a correção e o acesso. O todo só se recompõe quando resultados, significados, decisões, comunicações e retornos permitem verificar 90% no prazo, fundamento e orientação em 100% das negativas e no máximo 1% de revisões por erro interno, sem excluir quem usa o canal não digital.

## Bloco 8 — Revisar depois da solução

Compare sua tentativa com os comentários sem substituí-la. Registre pelo menos duas mudanças e uma questão que continuará aberta.

| Decisão inicial | Decisão revista | Base da mudança | Efeito sobre cobertura ou recomposição |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |

A mudança pode atingir critério, fronteira, granularidade, dependência, interface ou tratamento de lacuna. “Fiz igual à solução” não basta: explique a razão e a consequência. Se mantiver uma decisão diferente, defenda-a pelo propósito e declare seu risco.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| critério explícito | mistura formas | declara um por quadro | justifica pela pergunta |
| cobertura | deixa partes centrais fora | cobre o núcleo | demonstra cobertura e resíduos |
| coerência das partes | lista arbitrária | segue o critério | explica cada contribuição |
| dependências | registra só ordem | identifica origem e destino | inclui condição e consequência |
| granularidade | partes vagas ou mínimas | permite análise | justifica a parada |
| interfaces | reduz a interface a contato ou tela | diz o que atravessa | preserva significado e responsabilidade |
| lacunas | não procura | identifica uma | avalia efeito no todo |
| sobreposição | trata toda como erro | distingue duplicidade | justifica transversalidade |
| recomposição | apenas reúne quadros | conecta resultados | preserva propriedades globais |
| objetivo global | desaparece | volta na validação | limita métricas locais por proteções |
| justificativa | usa preferência | remete ao caso | compara alternativa e consequência |
| revisão | copia o comentário | altera duas decisões | registra base, efeito e questão aberta |

Considere a prática pronta para entrega quando nenhum critério estiver em “precisa de revisão” e você conseguir explicar oralmente, sem ler, por que três decomposições do mesmo todo podem ser diferentes e ainda assim válidas.
