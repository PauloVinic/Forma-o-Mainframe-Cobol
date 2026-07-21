# Prática 02 — De situações vagas a problemas verificáveis

## Identificação

- **Fase:** Fase 1 — Pensamento Computacional
- **Aula relacionada:** Aula 02 — O que é um problema
- **Competências:** C01 — Formular o problema; C02 — Especificar a transformação em nível inicial
- **Nível esperado:** Nível 2 — Explicação; Nível 3 — Aplicação guiada; início de aplicação autônoma em caso simples
- **Tempo estimado:** 3 a 4 horas, incluindo tentativa, consulta da solução e revisão

## Objetivo

Nesta prática, você transformará relatos, registros, interesses e soluções sugeridas em formulações iniciais examináveis. O objetivo não é escolher ferramenta, arquitetura, algoritmo, código ou automação completa. É distinguir o que se sabe do que se supõe, delimitar o problema, reconhecer quem participa ou é afetado e declarar critérios de avaliação.

Os blocos têm funções diferentes: formulação guiada; análise causal; conflitos entre interessados; e crítica de solução prematura.

## Orientações

Todos os números e registros dos casos são **hipotéticos** e existem apenas para esta atividade. Eles não descrevem uma organização real. Ao responder:

1. associe cada afirmação à evidência fornecida ou marque-a como inferência, hipótese, decisão ou questão em aberto;
2. não trate associação como prova de causa;
3. não invente regras, metas, responsáveis ou restrições;
4. mantenha soluções sugeridas separadas da formulação do problema;
5. use “não informado” quando a lacuna não puder ser resolvida;
6. formule critérios com população, período e forma de observação quando disponíveis;
7. preserve incertezas relevantes.

## Bloco 1 — Estoque e reposição: formulação completa guiada

Uma rede fictícia deseja reduzir ocorrências nas quais uma linha de solicitação não é atendida integralmente na primeira separação. Para o exercício, considere o período hipotético de 28 dias e somente os produtos críticos P-101, P-205 e P-330 nos centros Norte e Sul.

| Registro hipotético | CD Norte | CD Sul | Total |
|---|---:|---:|---:|
| Linhas solicitadas | 1.400 | 1.000 | 2.400 |
| Linhas não atendidas integralmente na primeira separação | 84 | 108 | 192 |
| Taxa observada | 6,0% | 10,8% | 8,0% |

A taxa foi calculada dividindo as linhas não atendidas integralmente pelo total de linhas solicitadas no mesmo centro e período. Entre as 192 ocorrências hipotéticas, 48 possuíam saldo positivo na última atualização registrada, 73 estavam associadas a uma entrada cuja data prometida já havia passado e 29 não possuíam histórico completo dos eventos. Esses grupos podem se sobrepor. Os registros não demonstram que saldo desatualizado ou atraso de fornecedor sejam causas.

Estão disponíveis linhas solicitadas, quantidades separadas, saldos diários registrados às 18 horas, entradas e saídas pendentes e pedidos de compra. A área física não poderá ser ampliada nos seis meses seguintes. Um analista pode dedicar oito horas semanais durante seis semanas à investigação. A gestão sugeriu, mas ainda não aprovou, uma taxa inferior a 3% em cada centro durante três ciclos consecutivos de 28 dias.

Também foram sugeridos aumento de estoque, redistribuição entre centros, revisão dos registros e aquisição de uma ferramenta de previsão. Nenhuma alternativa foi avaliada.

### Tarefa

Preencha a ficha. Em **base ou pendência**, indique a origem da resposta ou a pergunta que ainda precisa ser investigada.

| Elemento | Formulação do aluno | Base ou pendência |
|---|---|---|
| Evidências disponíveis |  |  |
| Inferências possíveis |  |  |
| Hipóteses causais |  |  |
| Interessados, pessoas afetadas e responsável pela decisão |  |  |
| Estado atual |  |  |
| Estado desejado |  |  |
| Objetivo |  |  |
| Escopo |  |  |
| Exclusões de escopo |  |  |
| Restrições |  |  |
| Recursos |  |  |
| Pressupostos |  |  |
| Entradas ou informações relevantes |  |  |
| Resultados esperados |  |  |
| Critérios de sucesso |  |  |
| Efeitos a evitar |  |  |
| Questões em aberto |  |  |
| Soluções sugeridas, mantidas separadamente |  |  |

Depois, escreva uma declaração inicial de 140 a 200 palavras. Trate a taxa de 3% como meta candidata, não como requisito confirmado. Sua formulação deve continuar útil se uma das soluções sugeridas for descartada.

## Bloco 2 — Benefício: sintoma, causa e hipótese

Em um cenário hipotético de 20 dias úteis, foram concluídas 1.000 solicitações de benefício. Destas, 620 receberam resposta em até cinco dias úteis e 380 ultrapassaram esse prazo. Entre as 380 solicitações demoradas, 210 tiveram pendência documental registrada, 140 foram reatribuídas ao menos uma vez e 90 atravessaram uma indisponibilidade do sistema de três horas. As categorias podem se sobrepor. Em 54 casos, passaram-se mais de dois dias úteis sem nova ação depois de todos os documentos terem sido marcados como recebidos.

Classifique os itens seguintes:

1. “Trinta e oito por cento das solicitações ultrapassaram cinco dias úteis.”
2. “Documentos incorretos são a causa dos atrasos”, afirma um analista.
3. Uma solicitante relata ter enviado o mesmo documento duas vezes.
4. O registro técnico confirma a indisponibilidade do sistema por três horas.
5. “A indisponibilidade explica todo o acúmulo”, afirma a equipe técnica.
6. A gestão decide testar horas extras na semana seguinte.
7. Cinquenta e quatro casos ficaram sem nova ação após o registro da documentação completa.

| Item | Classificação principal | O que sustenta | O que não permite concluir | Evidência adicional necessária |
|---|---|---|---|---|
| 1 |  |  |  |  |
| 2 |  |  |  |  |
| 3 |  |  |  |  |
| 4 |  |  |  |  |
| 5 |  |  |  |  |
| 6 |  |  |  |  |
| 7 |  |  |  |  |

Use, quando pertinente, **sintoma**, **evidência**, **testemunho**, **inferência**, **hipótese causal**, **causa não confirmada** ou **decisão**. Uma resposta pode combinar categorias, desde que explique a relação. Ao final, proponha duas hipóteses concorrentes e diga que evidência permitiria examiná-las. Não escolha uma “causa correta” com os dados disponíveis.

## Bloco 3 — Atendimento: objetivos e interessados

Em cinco dias hipotéticos, uma unidade emitiu 600 senhas: 540 atendimentos foram concluídos e 60 pessoas saíram antes de serem atendidas. Entre os atendimentos concluídos, a mediana de espera foi 42 minutos e o percentil 90 foi 96 minutos. A mediana informada não inclui quem abandonou a fila.

Uma representação de usuários pede previsão compreensível de espera e preservação da posição. Atendentes pedem critérios claros de prioridade e margem para tratar urgências. A gestão propõe mediana máxima de 25 minutos. Pessoas com prioridade querem que sua condição seja respeitada sem exposição indevida. A auditoria precisa reconstruir a ordem e as alterações de prioridade. As pessoas que abandonaram a fila não participaram da reunião.

### Tarefa

| Perspectiva | Objetivo | Evidência ou alegação | Critério possível | Conflito ou efeito colateral |
|---|---|---|---|---|
| Usuários |  |  |  |  |
| Atendentes |  |  |  |  |
| Gestão |  |  |  |  |
| Pessoas com prioridade |  |  |  |  |
| Auditoria |  |  |  |  |

Identifique dois conflitos entre objetivos. Indique uma pessoa ou grupo afetado ausente e formule uma pergunta que deveria ser feita a esse grupo. Proponha um conjunto equilibrado de critérios contendo uma métrica central, uma medida de distribuição ou proteção, um critério sobre abandono e um critério de rastreabilidade. Declare quem deve decidir a priorização e que informação sustenta essa responsabilidade. Não trate a redução da mediana como garantia de melhora para todos.

## Bloco 4 — Reembolsos: crítica de solução prematura

Considere a solicitação:

> Precisamos comprar um sistema novo com inteligência artificial, aprovar automaticamente 80% dos reembolsos e controlar as exceções em uma planilha.

No último mês hipotético, foram recebidas 500 solicitações. Noventa e cinco foram devolvidas para correção: 42 por comprovante ausente, 31 por divergência entre política e centro de custo e 22 por duplicidade ou valor inconsistente. Portanto, 95 de 500, ou 19%, foram devolvidas. A mediana hipotética até a primeira resposta foi de seis dias úteis. Existe uma referência interna a quatro dias, mas não estão definidos início, término ou exceções da medição. Dezoito solicitações aprovadas exigiram ajuste posterior.

Não há evidência que atribua os resultados à ausência de inteligência artificial, ao sistema atual ou ao trabalho manual.

### Tarefa

1. Separe as evidências, os objetivos, as metas e as soluções embutidas na solicitação.
2. Registre pelo menos cinco questões em aberto.
3. Reescreva o problema em 140 a 200 palavras, sem nomear uma ferramenta.
4. Proponha um critério principal e dois critérios de proteção.
5. Crie um contraexemplo de 80 a 120 palavras no qual a ferramenta sugerida seja implantada, mas o problema permaneça ou piore.

O percentual de aprovação automática não é, por si só, evidência de correção, rapidez ou adequação. A reformulação pode priorizar demora, retrabalho ou ajustes posteriores, mas deve declarar essa escolha e preservar os outros efeitos como limites ou questões.

## Entrega esperada

Entregue a ficha e a declaração do Bloco 1; a classificação e as duas hipóteses do Bloco 2; o quadro, os conflitos e os critérios do Bloco 3; a crítica, a reformulação e o contraexemplo do Bloco 4. Depois de consultar a solução, registre duas revisões: o que mudou, que evidência ou critério motivou a mudança e que dúvida permaneceu. Finalize com uma autoavaliação breve baseada na rubrica: um ponto consistente e um que ainda precisa de revisão.

## Organização do tempo

- leitura e orientação: 15 a 20 minutos;
- Bloco 1: 55 a 70 minutos;
- Bloco 2: 25 a 35 minutos;
- Bloco 3: 30 a 40 minutos;
- Bloco 4: 30 a 40 minutos;
- solução, autocorreção e revisões: 25 a 35 minutos.

Total: 3 a 4 horas, sem pausas longas.

# Solução comentada — consulte somente depois da tentativa

O Bloco 1 recebe um modelo completo porque introduz a ficha. Nos demais, apenas escolhas selecionadas são comentadas. Alternativas são aceitáveis quando preservam evidência, limites e rastreabilidade.

## Bloco 1 — Um modelo possível

- **Evidência e fatos:** a tabela, os registros e a regra de contagem são evidências; sustentam os fatos de 192 ocorrências em 2.400 linhas e 29 históricos incompletos.
- **Inferências:** as taxas calculadas são 6% no Norte, 10,8% no Sul e 8% no total; a taxa Sul foi maior somente no recorte. O impacto final é questão aberta.
- **Hipóteses:** atualização tardia, atraso de entrada, reserva não representada ou divergência física são explicações examináveis, não causas confirmadas.
- **Pessoas:** estoque, compras, fornecedores, gestão e unidades que solicitam os produtos são interessados; usuários finais podem ser afetados; o responsável por aprovar objetivo e meta não foi informado.
- **Estados e objetivo:** o estado atual possui taxa total de 8% no recorte; deseja-se reduzi-la de forma sustentada, tendo perdas, custos e deslocamento como proteções candidatas. Não se conhece estado desejado aprovado.
- **Escopo e exclusões:** dois centros, três produtos, primeira separação e ciclos de 28 dias; outros centros, outros produtos, escolha de ferramenta e construção de procedimento ficam fora do recorte inicial.
- **Restrições e recursos:** não ampliar a área por seis meses; usar registros existentes e a disponibilidade limitada do analista.
- **Pressupostos:** identificadores e critérios de contagem são comparáveis. Isso precisa ser verificado.
- **Entradas e resultados:** linhas solicitadas, separações, saldos, movimentos e pedidos sustentam a análise. O resultado esperado é redução sustentada sem piorar efeitos protegidos; linha de base e critérios são produtos da análise.
- **Critério candidato:** taxa inferior a 3% em cada centro por três ciclos, condicionada à validação da meta e a proteções sobre perdas, custo e transferências.
- **Efeitos e questões:** evitar excesso, vencimento, custo desproporcional e transferência da falta para outro produto ou centro. Faltam definição de atendimento, impacto, qualidade dos registros, linhas de base das proteções e autoridade de aprovação.
- **Soluções separadas:** aumentar estoque, redistribuir, revisar registros ou adquirir ferramenta permanecem alternativas não avaliadas.

Uma declaração possível é:

> No recorte hipotético de três produtos e dois centros, 192 de 2.400 linhas não foram atendidas integralmente na primeira separação durante 28 dias. Deseja-se reduzir essa ocorrência de forma sustentada; capacidade, perdas e custo são proteções candidatas a validar, sem assumir como confirmadas hipóteses sobre registros ou fornecedores. A taxa inferior a 3% por centro é uma meta candidata. Permanecem abertas a definição operacional de atendimento, a qualidade dos registros, os efeitos sobre usuários, as linhas de base dos critérios de proteção e a responsabilidade por validar a meta. A escolha entre estoque adicional, redistribuição, correção de dados ou ferramenta deve ser avaliada separadamente.

## Bloco 2 — Classificações selecionadas

O item 1 é inferência aritmética sustentada pelos registros e quantifica um sintoma. O item 2 é hipótese causal generalizada, não causa confirmada. O item 4 comprova a indisponibilidade, não seu impacto total. O item 6 registra decisão, não evidência causal. Hipóteses alternativas são aceitáveis quando indicam evidência capaz de contrariá-las.

## Bloco 3 — Um conflito para comparação

Usuários buscam previsibilidade; atendentes, regras aplicáveis; gestão, capacidade; pessoas prioritárias, proteção sem exposição; auditoria, rastreabilidade. Reduzir a mediana pode omitir abandono e espera extrema; flexibilizar urgências pode tensionar ordem auditável. Uma resposta consistente combina tendência central, distribuição, abandono, prioridade e rastreabilidade, com população e período. Os objetivos não são homogêneos.

## Bloco 4 — Exemplo de reformulação aberta

> No processamento hipotético de reembolsos de **[escopo a delimitar]**, 95 de 500 solicitações foram devolvidas e a primeira resposta apresentou mediana de seis dias úteis. Deseja-se reduzir **[retrabalho, demora ou ajustes posteriores: escolha a prioridade]** sem prejudicar conformidade, correção, rastreabilidade, contestação ou proteção de dados. Ainda precisam ser definidos o início e o fim da medição, os grupos e exceções, a linha de base dos efeitos protegidos e o responsável pelas metas. Sistemas, inteligência artificial, automação e planilhas permanecem alternativas a avaliar, não partes da definição do problema.

O exemplo permanece aberto de propósito. Uma resposta que escolha outra prioridade pode ser melhor para determinado interessado, desde que declare a perspectiva e não apresente a ferramenta como causa ou requisito. Um contraexemplo forte mostra um mecanismo concreto: a ferramenta pode processar rapidamente documentos incompletos, reproduzir regra inadequada ou elevar aprovações automáticas enquanto aumentam ajustes posteriores.

## Critérios de autocorreção

| Critério | Precisa de revisão | Adequado | Consistente |
|---|---|---|---|
| Precisão conceitual | mistura categorias | distingue os termos principais | relaciona-os sem apagar limites |
| Evidência | afirma sem origem | usa os registros fornecidos | mostra alcance e limite da evidência |
| Fato e hipótese | trata hipótese como fato | separa as categorias | indica como examinar ou contrariar hipótese |
| Delimitação | omite ou arbitra o escopo | declara escopo e exclusões | justifica o recorte e reconhece dependências |
| Neutralidade | incorpora ferramenta ao problema | separa solução sugerida | preserva alternativas reais |
| Interessados | considera apenas quem solicitou | identifica grupos relevantes | inclui afetados ausentes e responsabilidade |
| Critérios verificáveis | usa “melhorar” sem medida | propõe observação possível | inclui população, período e proteção |
| Pressupostos | deixa-os implícitos | declara pressupostos | prevê revisão diante de evidência |
| Questões abertas | inventa respostas | registra lacunas | converte lacunas em investigação útil |
| Conflitos | presume objetivo único | identifica tensão | inclui proteção sem fingir consenso |
| Clareza | produz texto circular | formula de modo legível | é conciso, preciso e proporcional |
| Rastreabilidade | apresenta conclusões soltas | conecta resposta ao caso | distingue origem, escolha e pendência |

Preencher todos os campos não garante consistência. Localize duas mudanças relevantes, revise os trechos e justifique a nova versão.
