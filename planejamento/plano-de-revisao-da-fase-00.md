# Plano de revisão da Fase 0 — Alfabetização Técnica

## 1. Objetivo

Revisar a Fase 0 para aumentar precisão conceitual, profundidade, coerência editorial, eficiência pedagógica e capacidade diagnóstica das avaliações, sem reduzir artificialmente o conteúdo. As aulas continuarão extensas; a revisão substituirá redundância por explicações melhores, limites, exceções, modelos, relações, exemplos progressivos e atividades conceituais mais exigentes.

## 2. Princípios

- Fundamentos vêm antes de ferramentas, mas aplicação fundamentada reforça a teoria.
- Extensão é legítima quando tem função pedagógica; preenchimento e reexplicação sem ganho não são.
- Retomadas devem ser breves, funcionais e servir de ponte para o novo conteúdo.
- A complexidade deve crescer a partir do que o aluno já domina.
- Definições devem distinguir modelo introdutório, definição técnica, convenção, interpretação e propriedade universal.
- Exemplos recorrentes só permanecem quando evoluem como estudo de caso progressivo.
- Templates orientam a escrita, mas a estrutura é escolhida pelo conteúdo.
- Fontes sustentam definições, escolhas terminológicas, modelos e controvérsias, sem transformar a aula em aparato de citações.
- Avaliações devem medir diferentes níveis cognitivos e orientar recuperação real.

## 3. O que não será feito

- Apagar a Fase 0.
- Reduzir todas as aulas ou transformá-las em resumos.
- Eliminar toda retomada.
- Reescrever tudo simultaneamente.
- Introduzir prática, código ou ferramentas sem fundamento pedagógico.
- Avançar para a Fase 1.
- Alterar o roadmap acadêmico completo durante a revisão da Fase 0.

## 4. Achados da auditoria

### Conceituais

As definições da Aula 4 tratam a sequência dado–informação–conhecimento como progressão demasiadamente natural; as da Aula 7 aproximam programa e especificação; as da Aula 9 simplificam tradução, compilação, interpretação, bytecode, máquina virtual e runtime; e as da Aula 12 misturam categorias de causa, manifestação e contexto em uma taxonomia de erro sem fonte explícita. Há ainda simplificações menores nas Aulas 2, 3, 8, 10 e 11.

### Pedagógicos

As 12 aulas têm sequência geral adequada e são estudáveis, mas apresentam retomadas longas, carga elevada e pouca variação de atividade. A Fase 0 concentra leitura, compreensão e reconhecimento; precisa preservar o caráter conceitual e aumentar análise, comparação, argumentação e produção de representações.

### Editoriais

O template se tornou estrutura repetida: objetivo, problema, introdução, conexão corporativa, conexão futura, confusões, síntese, glossário e domínio em quase todas as aulas. Banco, folha, estoque, cobrança, governo, relatório e cadastro reaparecem com baixa evolução em algumas seções. Há repetição semântica entre aulas, glossários e consolidação.

### Documentais

Faltam fontes bibliográficas para definições centrais. Há glossários sobrepostos e documentos de estado que ainda anunciam atividades futuras já presentes em `consolidacao/`. Esses pontos não serão corrigidos fora do escopo das etapas definidas, mas devem orientar a revisão de coerência e de referências.

### Avaliativos

Os exercícios têm bons cenários, mas repetem muitas distinções. A avaliação objetiva possui distratores pouco plausíveis e mede sobretudo reconhecimento; questões dissertativas antecipam demais a resposta esperada; a rubrica não tem pesos, critérios por item ou respostas limítrofes; checklist e plano de estudo não produzem evidência suficiente de domínio e revisão espaçada.

## 5. Prioridades conceituais

### Aula 4 — Dados, informação e conhecimento

A revisão deve distinguir dado, informação e conhecimento sem apresentar o modelo DIKW como lei universal. Deve tratar o modelo como lente didática possível, incluindo dados derivados, sintéticos, hipotéticos e incorretos. Deve reforçar contexto, interpretação e evidência, separando o que um sistema representa do significado que pessoas e organizações atribuem.

### Aula 7 — Programa

Deve separar requisito, especificação, algoritmo, programa, software, processo e execução. A aula deve esclarecer que especificações podem não ser executáveis, algoritmos são métodos independentes de uma implementação particular e um processo é uma noção introdutória que será aprofundada em sistemas operacionais.

### Aula 9 — Compilação, interpretação e execução

Deve diferenciar tradução, compilação, interpretação, representação intermediária, bytecode, máquina virtual, runtime e execução. Deve explicar que tecnologias reais podem combinar esses mecanismos e que compilação bem-sucedida evidencia aceitação/preparação segundo determinadas regras, sem provar correção da solução ou do negócio.

### Aula 12 — Erro

Deve diferenciar engano humano, defeito, falha, incidente, sintoma e causa a partir de uma terminologia escolhida e referenciada. Erro lógico, de dado, ambiente e operação devem ser tratados como dimensões ou hipóteses não exclusivas, evitando a impressão de que todo problema recebe uma única etiqueta.

## 6. Revisão das demais aulas

- **Aula 1:** qualificar a definição operacional de TI e reduzir antecipações da Aula 4; preservar a visão sociotécnica.
- **Aula 2:** apresentar sistema, propósito e entrada–processamento–saída–feedback como modelos de análise, não propriedades universais; qualificar categorias de sistemas.
- **Aula 3:** distinguir banco de dados de sistema gerenciador de banco de dados; qualificar o que “software” abrange.
- **Aula 5:** delimitar processamento e distinguir dimensões como manual/automatizado, lote/interativo e contínuo; reduzir sobreposição com a Aula 6.
- **Aula 6:** preservar o modelo EPS, declarar seus limites em sistemas interativos, concorrentes e orientados a eventos; substituir repetição por casos progressivos.
- **Aula 8:** tratar código-fonte como geralmente textual, sem torná-lo definição universal; separar fonte, configuração e artefatos gerados.
- **Aula 10:** qualificar arquivo, diretório e formato por sistema operacional; introduzir bytes e codificação sem antecipar arquitetura em excesso.
- **Aula 11:** separar finalidade do ambiente, localização/hospedagem, plataforma e governança; evitar apresentar local, nuvem, corporativo e mainframe como categorias exclusivas.

## 7. Estratégia editorial

Cada etapa deve localizar blocos repetidos dentro da aula, entre aulas vizinhas e entre aulas/glossário/consolidação. Manter uma retomada quando ela ativa um pré-requisito e cria ponte explícita; revisar quando ela apenas repete definição e exemplo já disponíveis.

Preservar a extensão por meio de aprofundamento: incluir definições em camadas, limites, exceções, consequências, comparações e caso progressivo. Elaborar uma matriz interna de exemplos para evitar que o mesmo domínio ilustre a mesma relação. Um cadastro, por exemplo, pode reaparecer para entrada, qualidade, validação, arquivo, ambiente ou erro, mas cada retorno deve introduzir questão nova.

Não aplicar o template como checklist de seções. A revisão pode combinar, mover ou substituir blocos quando isso melhorar ritmo e progressão, preservando começo, desenvolvimento, reflexão e critérios de domínio.

## 8. Estratégia de fontes

Criar, em etapa posterior, política bibliográfica que associe cada definição central a uma fonte canônica. Organizar referências ao final de cada aula ou em documento bibliográfico por fase, usando identificadores consistentes. Priorizar livros acadêmicos, normas, documentação oficial, ACM/IEEE, universidades e IBM quando aplicável.

Cada referência deve ter finalidade: sustentar uma definição, registrar terminologia, apresentar um modelo/controvérsia ou orientar aprofundamento. A revisão técnica deve registrar quais afirmações exigem fonte; não deve executar ainda uma pesquisa bibliográfica completa. O controle de qualidade verificará autoridade, adequação ao nível, data quando relevante e correspondência entre fonte e afirmação.

## 9. Estratégia de avaliação

Após a revisão das aulas, revisar exercícios, perguntas dissertativas, avaliação objetiva, avaliação dissertativa, rubrica, checklist e plano de estudo. Criar um mapa de competências e níveis cognitivos. Substituir distratores absurdos por alternativas plausíveis; aceitar hipóteses alternativas quando a classificação for multidimensional; usar cenários que exijam justificar.

Para dissertativas, definir conceitos esperados, pesos, erros graves, níveis de desempenho e respostas limítrofes. Para checklist, solicitar evidências produzidas pelo aluno. Para plano de estudo, estimar carga, inserir recuperação ativa, repetição espaçada, retorno a erros e reavaliação com itens diferentes.

## 10. Divisão dos trabalhos

| Etapa | Objetivo | Arquivos | Riscos | Critérios de conclusão | Permitido | Proibido |
|---|---|---|---|---|---|---|
| 1 | Revisar tecnicamente dados/conhecimento e programa | Aulas 4 e 7; glossários apenas se a etapa autorizar | alterar escopo ou introduzir formalismo excessivo | distinções corretas, modelos qualificados, pontes preservadas | editar as duas aulas e referências associadas autorizadas | alterar outras aulas, exercícios, roadmap |
| 2 | Revisar tradução/execução e taxonomia de problemas | Aulas 9 e 12 | impor taxonomia sem fonte; excesso de jargão | termos definidos, categorias não exclusivas, limites claros | editar as duas aulas e fontes autorizadas | alterar avaliações ainda |
| 3 | Revisar base sociotécnica e sistema | Aulas 1, 2 e 3 | reintroduzir conteúdo das aulas 4–12 | definições operacionais qualificadas, exemplos variados | editar somente as três aulas | reduzir volume por meta |
| 4 | Revisar processamento e EPS | Aulas 5 e 6 | duplicação entre as duas ou simplificação linear | fronteiras e limites claros; caso progressivo | editar as duas aulas | criar código/prática artificial |
| 5 | Revisar fonte, arquivos e ambientes | Aulas 8, 10 e 11 | antecipar SO/arquitetura em excesso | terminologia precisa e progressão preservada | editar as três aulas | alterar Aula 9 fora de correção de link |
| 6 | Revisar coerência do conjunto | 12 aulas, roteiros e critérios autorizados | reabrir conteúdo sem evidência | transições, termos e exemplos consistentes | ajustes de coerência aprovados | reescrever tudo simultaneamente |
| 7 | Revisar glossários e referências | glossários e bibliografia autorizada | duplicação e fontes decorativas | fonte canônica, termos coerentes, referências úteis | editar glossários/referências | mudar aulas sem necessidade |
| 8 | Revisar consolidação | todos os arquivos de `consolidacao/` | repetir aulas ou criar gabaritos frágeis | materiais ativos, integrados e sem duplicação | editar consolidação | alterar roadmap/Fase 1 |
| 9 | Reconstruir avaliações | exercícios, avaliações, rubrica, checklist e plano | calibragem sem piloto | blueprint cognitivo, critérios e itens plausíveis | editar instrumentos | declarar domínio sem evidência |
| 10 | Auditar Fase 0 revista | fase inteira e relatório novo | autoaprovação | achados, testes e pendências documentados | criar auditoria final | iniciar Fase 1 automaticamente |

## 11. Critérios de sucesso

- Nenhuma definição central é apresentada indevidamente como universal.
- Distinções terminológicas são claras, consistentes e adequadas ao nível.
- Aulas permanecem extensas e não se tornam resumos.
- Repetições desnecessárias diminuem; retomadas úteis permanecem.
- O espaço editorial recuperado aumenta profundidade, não reduz conteúdo por contagem.
- Exemplos têm progressão e diversidade.
- Fontes são planejadas para cada definição/taxonomia central.
- Avaliações futuras medem raciocínio além de reconhecimento.
- Transições entre aulas se tornam mais fortes e não antecipam conteúdos fora de fase.

## 12. Estado esperado depois da revisão

Uma Fase 0 revista será uma base conceitual extensa, tecnicamente mais precisa e editorialmente mais eficiente. O aluno encontrará modelos identificados como modelos, conexões progressivas entre conceitos, exemplos que evoluem e atividades que revelam o que consegue explicar e analisar. A fase estará pronta para estudo com evidência de domínio e para servir de base à Fase 1, sem afirmar que substitui os fundamentos matemáticos, algorítmicos e práticos a serem construídos adiante.

## Registro de execução

### Etapa 1 — Revisão técnica das Aulas 04 e 07

**Status:** concluída nesta etapa.

**Conceitos corrigidos ou qualificados:** a Aula 04 passou a tratar dado como representação que pode ser observada, declarada, derivada, sintética ou hipotética; distinguiu dado, fato, registro, evidência e interpretação; apresentou DIKW como modelo influente e discutido; e tratou qualidade como adequação ao uso em dimensões não universais. A Aula 07 passou a separar necessidade, requisito, regra de negócio, especificação, algoritmo, implementação, programa, código-fonte, software, sistema e processo; também distinguiu comportamento esperado de comportamento observado.

**Fontes registradas:** `referencias/fontes-da-fase-00.md` recebeu as fontes usadas para as Aulas 04 e 07.

**Pendências observadas para etapas posteriores:** as Aulas 08 e 09 ainda usam formulações mais simplificadas sobre código-fonte, compilação, interpretação e runtime; a Aula 12 ainda precisa revisar sua taxonomia de erro, defeito e falha. As Aulas 03, 05, 06, 10 e 11 devem ser verificadas nas etapas previstas para compatibilizar glossários e exemplos. Nenhuma dessas aulas foi alterada agora.

**Próxima etapa:** revisão técnica das Aulas 09 e 12.
