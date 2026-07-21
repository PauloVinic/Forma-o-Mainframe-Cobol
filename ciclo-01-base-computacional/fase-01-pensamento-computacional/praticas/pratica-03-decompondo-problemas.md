# Prática 03 — Três decomposições do mesmo problema

## Identificação

- **Ciclo:** 1 — Base Computacional
- **Fase:** 1 — Pensamento Computacional
- **Aula associada:** Aula 03 — Decomposição de problemas
- **Competência:** C03 — decompor, preservar dependências e recompor
- **Caso:** concessão do Benefício de Apoio Temporário
- **Produto essencial:** uma decomposição principal completa, duas visões resumidas, comparação, mapa de dependências, recomposição e revisão
- **Produto de aprofundamento:** três decomposições completas, mapa ampliado, recomposição e duas revisões
- **Tempo estimado:** 3h15 a 4h20 no percurso essencial; 5h20 a 7h00 com aprofundamento

## Objetivo

Você examinará o mesmo problema por três critérios: funções, informações e objetos do domínio e etapas ou eventos. Depois comparará o que cada divisão torna visível, registrará dependências e testará se as partes podem ser recompostas sem perder prazo, correção, rastreabilidade, confidencialidade, acesso e contestação. A expressão “informações e objetos do domínio” refina o eixo abreviado como “dados” em C03; não cria um quarto critério.

A atividade não pede solução técnica, automação, código, pseudocódigo, fluxo formal nem estrutura de software. O objetivo é justificar uma divisão analítica. Há mais de uma resposta adequada, desde que o todo permaneça o mesmo e critérios, fronteiras, dependências e consequências sejam explícitos.

## Orientações

Faça os Blocos 1 a 7 antes de consultar a solução comentada e conclua o Bloco 8 depois dela. Os oito blocos permanecem obrigatórios nas duas modalidades. Use a modalidade **essencial** para uma primeira demonstração de domínio; use o **aprofundamento**, opcional, para testar granularidades e alternativas. O aprofundamento não é requisito para a Aula 04.

No Bloco 1, escolha provisoriamente um dos três critérios como decomposição principal. Nos Blocos 2 a 4, desenvolva completamente esse critério e registre os outros dois em formato resumido. No Bloco 5, confirme ou revise a escolha. Com aprofundamento, desenvolva as três decomposições completamente. Marque incertezas em vez de inventar informações. Rótulos como “atividade de análise”, “registro da decisão” ou “documento apresentado” precisam de uma frase que delimite seu papel.

Cada decomposição deve usar um critério principal. Partes de critérios diferentes podem aparecer em níveis distintos, desde que isso seja declarado. Setas devem ter rótulo: “fornece informação”, “requer decisão”, “restringe” ou outro significado preciso. Uma seta sem rótulo não informa se existe ordem, dependência ou causalidade.

## Caso — Benefício de Apoio Temporário

O programa hipotético recebeu **1.000 solicitações em 20 dias úteis**. A coorte foi acompanhada até a primeira decisão autorizada, sua comunicação e, quando apresentada no prazo, a contestação e a reanálise. Destas, 620 tiveram primeira decisão em até cinco dias úteis e 380 ultrapassaram esse prazo: `620 + 380 = 1.000`, ou 62% e 38%.

Entre as 380 solicitações demoradas, 210 passaram por pendência documental, 140 foram reatribuídas e 90 atravessaram uma indisponibilidade de três horas. As categorias podem se sobrepor; por isso, `210 + 140 + 90 > 380` não é contradição. Os números também não estabelecem relação causal. Em 54 casos não houve nova ação por mais de dois dias depois que os documentos foram marcados como recebidos.

As primeiras decisões foram 760 concessões e 240 negativas. Das negativas, 72 foram contestadas. Após reanálise, 24 decisões mudaram: 15 por nova evidência admitida e nove por correção de erro interno. Assim, `24 ≤ 72 ≤ 240`. Em 48 decisões não havia tentativa de comunicação registrada até dois dias úteis depois da decisão.

Uma solicitação pode estar recebida, com pendência, em atividade de análise, aguardando registro de decisão autorizada, concedida ou negada. A contestação tem estados próprios: recebida, em atividade de reanálise e decidida. Solicitação e contestação não são o mesmo objeto do domínio.

Regras hipotéticas do recorte:

- identidade, residência e condição de renda precisam ser sustentadas por documento ou forma equivalente admitida;
- item ausente ou ilegível gera pendência identificada, com prazo; não gera negativa automática antes do prazo;
- a atividade de análise produz uma conclusão recomendada e um registro das regras aplicadas;
- somente papel autorizado pode conceder ou negar;
- o ato de decidir produz um resultado, cujo registro preserva fundamento e autorização;
- a atividade de comunicação emite o resultado da decisão, seu fundamento, prazo e meio de contestação;
- contestação apresentada em até dez dias úteis da comunicação emitida pode trazer nova evidência e retorna para atividade de reanálise;
- nova evidência e correção de erro interno precisam permanecer distinguíveis.

O objetivo é reduzir tempo e interrupções até uma decisão válida, preservando aplicação das regras, rastreabilidade, confidencialidade, acesso e contestação. A meta candidata é que ao menos 90% das solicitações de cada um de três ciclos recebam primeira decisão autorizada em até cinco dias úteis, com população e método comparáveis. Todas as negativas devem registrar fundamento e orientação para contestar; revisões por erro interno não podem ultrapassar 1% da coorte.

Durante os três ciclos, as regras não podem ser alteradas e não haverá aumento de equipe. Informações sensíveis só podem ser acessadas por papéis autorizados, o canal não digital deve permanecer e a atividade não escolherá sistema, automação ou reorganização. Solicitantes, representantes, pessoas com dificuldade de acesso digital, atendimento, analistas, autoridade decisória, responsáveis pela contestação, auditoria e responsáveis pelas regras são interessados ou afetados.

Permanecem abertas a interpretação de documentos equivalentes, a definição de comunicação efetiva, diferenças entre canais, os motivos das reatribuições e a responsabilidade pela divergência entre documento marcado como recebido e documento disponível ao analista.

## Bloco 1 — Reconstruir o todo

No percurso essencial, registre **120 a 160 palavras**; com aprofundamento, use até **180 palavras**. Inclua somente:

1. o todo analisado e a finalidade da decomposição;
2. o estado atual, o estado desejado e o objetivo;
3. escopo, critérios globais e restrições que não podem desaparecer;
4. duas questões abertas capazes de alterar a decomposição — quatro no aprofundamento;
5. o critério principal provisório e, no aprofundamento, o que poderia alterar essa escolha.

Não refaça a ficha completa da Aula 02. O todo não é “todo o programa social”, e preencher campos que não ajudam a próxima decisão não demonstra domínio.

## Bloco 2 — Decomposição funcional

Declare o critério funcional em uma frase.

- **Se for a decomposição principal no essencial:** identifique de cinco a seis funções e preencha o quadro completo; indique uma lacuna e justifique a parada.
- **Se for uma visão alternativa no essencial:** registre quatro funções, a contribuição de cada uma e um ponto cego, sem preencher o quadro completo.
- **Com aprofundamento:** registre de seis a oito funções, divida duas em subpartes, compare uma fronteira ampla e outra estreita e justifique a parada.

| Função | Finalidade | Informação necessária | Resultado parcial | Dependências |
|---|---|---|---|---|
|  |  |  |  |  |

Confirme que as funções respondem “o que precisa ocorrer?” e não foram copiadas de departamentos ou transformadas em elementos de software.

## Bloco 3 — Decomposição por informações e objetos do domínio

Nesta visão, **objeto do domínio** é algo cuja identidade ou condição importa; **dado** é valor ou símbolo cuja interpretação depende de contexto; **informação** é uma representação com significado sobre um objeto ou ocorrência; **registro** evidencia ou armazena informação. Um **documento** é um artefato delimitado que contém informação registrada e pode ser objeto do domínio quando sua identidade ou condição importa. **Atividade** é transformação, e **resultado** é seu efeito ou produto. Portanto, analisar e decidir são atividades; conclusão recomendada e resultado da decisão são resultados; registro da análise e decisão registrada são registros.

- **Se for a decomposição principal no essencial:** selecione de cinco a seis informações, registros ou objetos e preencha o quadro completo.
- **Se for uma visão alternativa no essencial:** registre quatro elementos, sua natureza e relevância, sem preencher o quadro completo.
- **Com aprofundamento:** examine de sete a oito elementos, duas divergências de significado e duas fronteiras ou granularidades alternativas.

| Elemento | Natureza: objeto, dado, informação ou registro | Significado, identidade ou condição no caso | Origem e uso | Dependência ou divergência possível |
|---|---|---|---|---|
|  |  |  |  |  |

Objeto, aqui, não significa tabela, arquivo, banco de dados ou estrutura técnica. Solicitação, documento, pendência e contestação podem ser objetos; a regra atua como restrição, embora sua formulação possa estar registrada como informação; conclusão da análise é resultado; decisão registrada e registro da comunicação emitida são registros de resultados. Esses candidatos não formam gabarito obrigatório. Explique por que cada escolha importa ao todo sem produzir modelo de dados.

## Bloco 4 — Decomposição por etapas ou eventos

Não presuma percurso único.

- **Se for a decomposição principal no essencial:** identifique de seis a oito momentos ou eventos e preencha o quadro completo, incluindo condição, retorno ou paralelismo.
- **Se for uma visão alternativa no essencial:** registre de quatro a cinco momentos e uma ocorrência não linear, sem preencher o quadro completo.
- **Com aprofundamento:** complete o quadro, inclua exceção, retorno, paralelismo, um caso de ordem sem dependência necessária e compare duas granularidades.

| Momento ou evento | Estado ou condição anterior e posterior | Informação necessária | Dependência relevante | Retorno ou exceção |
|---|---|---|---|---|
|  |  |  |  |  |

Na visão principal ou no aprofundamento, explique em duas frases por que seu quadro não é algoritmo nem fluxo obrigatório.

## Bloco 5 — Comparar os critérios

Preencha exatamente três linhas:

| Critério | O que evidencia | O que deixa menos visível | Vantagem | Risco | Pergunta atendida | Complemento necessário |
|---|---|---|---|---|---|---|
| funcional |  |  |  |  |  |  |
| informações e objetos do domínio |  |  |  |  |  |  |
| etapas/eventos |  |  |  |  |  |  |

Escolha qual decomposição usaria como principal para investigar os 54 casos sem nova ação e justifique pela pergunta, não por preferência pessoal. Confirme ou revise sua escolha provisória e declare o complemento necessário. Outra escolha pode ser válida quando explicita seus limites. No aprofundamento, compare também o custo analítico e o risco das granularidades adotadas.

## Bloco 6 — Construir o mapa de dependências

Use como base a decomposição desenvolvida completamente. Se o Bloco 5 favoreceu outra visão, registre esse limite e uma dependência complementar, sem fingir que o resumo virou quadro completo. No percurso essencial, registre pelo menos cinco partes e cinco dependências. Com aprofundamento, registre sete ou mais partes e oito ou mais dependências.

| Origem → destino | O que atravessa a interface | Natureza ou condição | Consequência se faltar |
|---|---|---|---|
|  |  |  |  |

No essencial, o mapa precisa conter uma dependência condicional e uma restrição transversal. No aprofundamento, inclua também retorno, transversalidade ampliada e possível circularidade a examinar. Para cada linha, identifique origem, destino, significado do conteúdo, condição e consequência da ausência. **Interface é a relação ou o ponto de interação pelo qual informação, material, decisão, regra ou mudança de estado atravessa a fronteira entre partes**; não é sinônimo de tela ou contrato técnico. Um retorno não transforma o mapa em procedimento formal e não demonstra causa.

## Bloco 7 — Recompor e avaliar

No percurso essencial, produza quatro resultados compactos:

1. verifique a cobertura de solicitação, documentos, pendência, atividade e registro da análise, ato e registro da decisão, comunicação emitida e contestação;
2. identifique uma lacuna, uma duplicidade problemática e uma sobreposição legítima;
3. registre uma interface ambígua e um risco de otimização local;
4. escreva **120 a 160 palavras** explicando como resultados parciais recompõem o objetivo global.

O texto deve mencionar critérios globais, pessoas afetadas e ao menos uma propriedade do todo: tempo total, rastreabilidade, confidencialidade ou capacidade de contestação. Se a recomposição falhar, diga se revisaria parte, critério, granularidade, dependência ou o próprio todo. Com aprofundamento, amplie a auditoria, compare interfaces alternativas e escreva **170 a 220 palavras**.

## Entrega esperada

- **Percurso essencial:** registro breve do todo; uma decomposição principal completa; duas visões resumidas; comparação em três linhas; mapa com ao menos cinco partes e cinco dependências; recomposição; uma revisão justificada; uma questão aberta; e marcação dos seis critérios decisivos indicados ao final.
- **Com aprofundamento:** registro ampliado; três decomposições completas; comparação de granularidades; mapa com sete ou mais partes e oito ou mais dependências; recomposição ampliada; duas revisões; uma questão aberta; e marcação dos 12 critérios.

Indique a modalidade realizada. Qualidade não será medida pelo maior número de partes, e sim por coerência, cobertura, relações preservadas e capacidade de revisão.

## Organização do tempo

| Etapa | Essencial | Com aprofundamento |
|---|---:|---:|
| leitura e escolha provisória | 15–20 min | 20–25 min |
| Bloco 1 | 15–20 min | 20–25 min |
| decomposição principal | 35–45 min | — |
| duas visões alternativas resumidas | 40–50 min | — |
| três decomposições completas | — | 2h15–3h00 |
| Bloco 5 — comparação | 15–20 min | 25–35 min |
| Bloco 6 — mapa | 25–35 min | 40–50 min |
| Bloco 7 — recomposição | 25–35 min | 35–45 min |
| consulta da solução | 10–15 min | 15–20 min |
| Bloco 8 e autoavaliação | 15–20 min | 30–40 min |
| **total** | **3h15–4h20** | **5h20–7h00** |

Os totais resultam da soma das etapas e não incluem pausas longas. Divida a prática em duas ou três sessões; não sacrifique a recomposição para terminar de uma vez. O aprofundamento é opcional e pode ser retomado depois da Aula 04.

# Solução comentada — consulte somente depois da tentativa

O que segue é uma possibilidade proporcional, não uma decomposição única. Ela comenta apenas escolhas representativas, não apresenta quadro nem decomposição principal completa e limita o mapa a quatro relações, para que a prática não vire cópia mecânica.

No Bloco 1, o todo pode ser descrito como o problema de reduzir demora e interrupções desde o recebimento das 1.000 solicitações até o registro da decisão autorizada e a emissão de sua comunicação, preservando eventual contestação, reanálise, regras, acesso e registros. Os 54 casos orientam uma pergunta, mas não substituem o todo nem demonstram causa. Questões sobre documento disponível, reatribuição e comunicação podem alterar fronteiras, dependências e a escolha da visão principal.

“Tratar pendência” e “comunicar o resultado da decisão e os direitos” são duas funções possíveis. A primeira poderia ser detalhada sem descrever ações de tela. Atividade de análise e ato de autorização precisariam permanecer distintos porque conclusão recomendada e decisão autorizada têm responsabilidades diferentes. Os exemplos não completam uma decomposição.

Na visão por informações e objetos do domínio, solicitação e documento são candidatos a objetos; a informação de que o documento está disponível descreve uma condição; registro da análise é registro. Analisar e decidir são atividades; conclusão recomendada e resultado da decisão são resultados distintos. Documento marcado como recebido não equivale a documento legível e disponível. Essas distinções pertencem ao domínio, não a um desenho de dados, e não completam o quadro.

Entre os momentos ou eventos possíveis estão recebimento, identificação de pendência, chegada de complemento, registro da decisão e eventual contestação com reanálise. Há retorno e caminhos condicionais. Preparar informação geral de comunicação pode ocorrer em paralelo à atividade de análise, embora a comunicação individual dependa de decisão autorizada. Esses exemplos não completam o quadro nem formam algoritmo obrigatório.

Uma comparação razoável diria que a visão funcional evidencia contribuições e responsabilidades; a visão por informações e objetos evidencia identidade, significado e mudanças da informação; a visão por etapas evidencia espera, retorno e condição. Para os 54 casos, etapas e eventos podem ser a visão principal porque localizam a interrupção entre recebimento marcado e nova ação. Informações e objetos são complemento indispensável para distinguir o que “recebido” significa. Escolher essa segunda visão como principal também seria defensável se a pergunta priorizasse a divergência semântica.

Tomando uma base funcional, um mapa seletivo pode conter três dependências entre funções e uma relação transversal:

1. registrar solicitação → verificar suficiência documental: fornece referências dos documentos e seu significado; sem isso, a verificação pode examinar o caso errado;
2. verificar suficiência documental → tratar pendência: fornece itens ausentes ou ilegíveis e prazo, **se** houver pendência; sem isso, a complementação pode ser inadequada;
3. examinar contestação → reanalisar elegibilidade: fornece alegação e nova evidência, **se** a contestação for admissível; sem isso, o retorno usa base incompleta;
4. restrição de acesso → analisar elegibilidade e comunicar resultado: limita em cada destino o uso de informações sensíveis; sua ausência pode expor informação ou impedir acesso legítimo.

Uma lacuna possível é não definir qual registro sustenta que o documento ficou disponível. Há duplicidade problemática se a atividade de análise e o ato de decidir aplicarem versões diferentes da regra sem coordenação; a regra alcançar ambas e a contestação é sobreposição legítima. Reduzir o tempo local devolvendo todo caso duvidoso pode piorar tempo total, correção e acesso. Uma demonstração parcial de recomposição conecta os registros de recebimento, decisão e comunicação à verificação de 90% no prazo, fundamento e orientação em 100% das negativas e no máximo 1% de revisões por erro interno, preservando o canal não digital. O aluno ainda deve mostrar como suas próprias partes, interfaces e retornos sustentam esse argumento.

## Bloco 8 — Revisar depois da solução

Compare sua tentativa com os comentários sem substituí-la. No percurso essencial, registre uma mudança justificada e uma questão que continuará aberta. Com aprofundamento, registre duas mudanças, defenda uma alternativa e mantenha uma questão aberta.

| Decisão inicial | Decisão revista | Base da mudança | Efeito sobre cobertura ou recomposição |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |

Preencha a primeira linha no essencial e as duas no aprofundamento. A mudança pode atingir critério, fronteira, granularidade, dependência, interface ou tratamento de lacuna. “Fiz igual à solução” não basta: explique a razão e a consequência. Se mantiver uma decisão diferente, defenda-a pelo propósito e declare seu risco.

## Critérios de autocorreção

No percurso essencial, marque apenas os seis critérios em **negrito**: critério explícito, cobertura, dependências, interfaces, recomposição e revisão. Com aprofundamento, marque os 12. A tabela completa permanece disponível para orientar melhorias, mas não transforma o aprofundamento em requisito normal de avanço.

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| **critério explícito** | mistura formas | declara um por quadro | justifica pela pergunta |
| **cobertura** | deixa partes centrais fora | cobre o núcleo | demonstra cobertura e resíduos |
| coerência das partes | lista arbitrária | segue o critério | explica cada contribuição |
| **dependências** | registra só ordem | identifica origem e destino | inclui condição e consequência |
| granularidade | partes vagas ou mínimas | permite análise | justifica a parada |
| **interfaces** | reduz a interface a contato ou tela | diz o que atravessa | preserva significado e responsabilidade |
| lacunas | não procura | identifica uma | avalia efeito no todo |
| sobreposição | trata toda como erro | distingue duplicidade | justifica transversalidade |
| **recomposição** | apenas reúne quadros | conecta resultados | preserva propriedades globais |
| objetivo global | desaparece | volta na validação | limita métricas locais por proteções |
| justificativa | usa preferência | remete ao caso | compara alternativa e consequência |
| **revisão** | copia o comentário | altera uma decisão | registra a quantidade exigida na modalidade, com base, efeito e questão aberta |

Considere a prática pronta para entrega quando nenhum critério exigido para sua modalidade estiver em “precisa de revisão” e você conseguir explicar oralmente, sem ler, por que três decomposições do mesmo todo podem ser diferentes e ainda assim válidas.
