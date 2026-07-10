# Revisão completa do projeto Formação Mainframe COBOL

## 1. Resumo executivo

**Estado geral:** o repositório está organizado, legível e coerente como fundação editorial e como módulo introdutório conceitual. Não está, porém, planejado com conteúdo, profundidade, prática e mecanismos de avaliação suficientes para sustentar a afirmação de equivalência acadêmica com uma formação universitária forte em Ciência da Computação. O maior problema não é a Fase 0 isoladamente; é a distância entre a ambição declarada e o roadmap efetivamente especificado.

- **O projeto está bem estruturado?** Estruturalmente, sim, com ressalvas. Há separação clara entre documentos globais, ciclos, planejamento, prompts, templates e a Fase 0. A estrutura sofre com documentos de estado desatualizados, pastas-placeholder que contradizem a consolidação já criada e regras repetidas em muitos arquivos.
- **A Fase 0 está estudável?** Sim. A sequência é compreensível, o português é claro e há materiais de revisão. Contudo, o volume de aproximadamente 58,5 mil palavras nas aulas é excessivo para alfabetização técnica e pode produzir fadiga, baixa retenção e falsa sensação de domínio baseada em leitura.
- **A Fase 0 está tecnicamente correta?** Em geral, sim, no nível introdutório. Não encontrei erro factual que torne o módulo inutilizável. Há simplificações e escolhas terminológicas que precisam de qualificação, sobretudo no modelo dado–informação–conhecimento, na distinção programa/especificação, na taxonomia erro–defeito–falha e na descrição de compilação/interpretação/runtime.
- **A Fase 0 está excessivamente longa?** Sim. As aulas têm entre aproximadamente 4,3 e 5,5 mil palavras, repetem a mesma arquitetura retórica e retomam extensamente exemplos, conexões corporativas, confusões comuns, sínteses e glossários. A extensão não é proporcional à dificuldade cognitiva das tarefas.
- **A consolidação é utilizável?** Sim, como revisão guiada. O estudo dirigido e os cenários são úteis. A prova objetiva é fácil e previsível; a rubrica não permite correção suficientemente consistente; o checklist depende de autodeclaração; o plano não estima horas nem implementa revisão espaçada real.
- **O roadmap atual é suficiente?** Não. Ele nomeia 32 fases, mas descreve cada uma em poucos parágrafos e omite áreas centrais ou não lhes atribui profundidade verificável. A especialização Mainframe/COBOL está mais bem representada que a formação de Ciência da Computação que deveria precedê-la.
- **O projeto pode atingir nível acadêmico elevado?** Pode, se o roadmap for substancialmente reconstruído antes de orientar as fases seguintes. Texto autônomo, exercícios, projetos e avaliações podem reproduzir boa parte do conteúdo e do rigor intelectual, mas não bastam títulos de fases nem capítulos longos. Serão necessários resultados observáveis, pré-requisitos, carga, bibliografia primária, laboratórios, programação desde cedo, provas cumulativas, projetos, feedback e critérios quantitativos.
- **Maiores obstáculos:** roadmap subespecificado; matemática e teoria ausentes; pouca prática planejada; atraso excessivo até programação; ausência de fontes; avaliação de baixa discriminação; volume e repetição; governança documental frágil.

**Contagem consolidada de achados priorizados:** 1 crítico, 8 altos, 12 médios e 7 baixos. A contagem refere-se aos achados agregados da seção 16, não a cada ocorrência textual.

## 2. Metodologia da revisão

Foram examinados os 77 arquivos versionados do repositório: 75 documentos Markdown e dois arquivos auxiliares vazios. A leitura abrangeu documentos globais, planejamento, quatro ciclos, seis templates, 16 arquivos de prompts, referências, planejamento da Fase 0, as 12 aulas e os 12 materiais de consolidação. O corpus Markdown contém aproximadamente 96,6 mil palavras; as aulas respondem por cerca de 58,5 mil e a consolidação por 8,1 mil.

As verificações estruturais incluíram branch, working tree, remote, último commit, arquivos rastreados, tamanhos, arquivos vazios, UTF-8 estrito, BOM, hashes duplicados, links Markdown locais, referências textuais a caminhos, consistência de numeração, títulos, índices e vocabulário de estado. A inspeção não encontrou arquivo Markdown inválido em UTF-8, duplicata byte a byte ou link Markdown local quebrado. Referências a nomes de saída no prompt 014 são especificações do prompt, não links navegáveis; portanto não foram classificadas como links quebrados.

Para a comparação externa foram consultadas fontes oficiais e primárias: o relatório [CS2023 da ACM/IEEE-CS/AAAI](https://csed.acm.org/wp-content/uploads/2025/11/CS2023-Report.htm), a [página oficial do CS2023](https://csed.acm.org/), os [requisitos do bacharelado em Ciência da Computação de Stanford](https://www.cs.stanford.edu/bs-degree-requirements) e o currículo oficial [Mathematics with Computer Science do MIT](https://catalog.mit.edu/degree-charts/mathematics-computer-science-course-18-c/). Essas referências foram usadas como padrões concretos de áreas, progressão, matemática, laboratórios, projetos e avaliação, não como argumento de prestígio.

Limitações: não houve aplicação das avaliações a alunos reais, medição de tempo de estudo, revisão por especialista de domínio IBM, execução de laboratórios nem validação psicométrica. O repositório não contém bibliografia acadêmica para verificar a origem de suas definições. A auditoria avalia o material existente e o planejamento declarado; não atribui conteúdo futuro que não esteja escrito.

## 3. Inventário do repositório

| Grupo | Arquivos | Função real | Estado |
|---|---:|---|---|
| Documentos globais | 8 | identidade, diretrizes, manifesto, glossário, prompts e roadmap | Parcialmente completos; coerentes, porém repetitivos e sem governança formal |
| Planejamento global | 3 | estrutura de fases, ordem e critérios de qualidade | Parcialmente completo; critérios qualitativos, sem carga, bibliografia ou métricas |
| Ciclos | 4 | resumir fases 0–31 | Completo como índice; superficial como projeto acadêmico |
| Templates | 6 | modelos de aula, avaliação, exercício, caso, estudo e glossário | Utilizáveis; induzem estrutura uniforme e repetição |
| Prompts | 16 | histórico das solicitações 000–014 e índice | Completo para o estágio; deve ser tratado como arquivo histórico, não norma concorrente |
| Referências | 1 | README de intenção | Incompleto: não contém referência bibliográfica alguma |
| Planejamento da Fase 0 | 9 documentos substantivos, além de índices/placeholders | ementa, plano, competências, domínio, estudo, roteiro, mapas e glossário | Substantivamente completo, mas redundante e parcialmente desatualizado |
| Aulas | 12 aulas + README | conteúdo principal | Completo; estudável, excessivamente longo e repetitivo |
| Consolidação | 12 | resumo, revisão, mapa, estudo, 80 exercícios, 22 perguntas, avaliações, rubrica, checklist e plano | Completa como conjunto inicial; qualidade avaliativa desigual |
| Pastas legadas da Fase 0 | 4 READMEs | exercícios, avaliações, estudos de caso e estudos dirigidos “futuros” | Inconsistentes com `consolidacao/`; inadequadamente paralelas |
| Auxiliares | `.megaignore`, `desktop.ini` | nenhum conteúdo | Vazios; `desktop.ini` é ruído de sistema operacional |

A estrutura real corresponde à descrição geral quanto a ciclos, Fase 0, 12 aulas e consolidação. Não corresponde quanto ao estado: `avaliacoes/README.md`, `exercicios/README.md`, `estudos-dirigidos/README.md` e `estudos-de-caso/README.md` ainda anunciam produção futura, embora materiais equivalentes tenham sido criados em `consolidacao/`. Também não existe acervo de referências, apesar de a ambição acadêmica exigir fontes.

## 4. Diagnóstico estrutural

### Git e arquivos

- Branch: `main`, acompanhando `origin/main` sem divergência indicada.
- Working tree no início da auditoria: limpo.
- Remote: `origin` em `https://github.com/PauloVinic/Forma-o-Mainframe-Cobol.git` para fetch e push.
- Último commit: `f48fc4e96bac8ccdd637d289dbd72db7e670acab`, de 5 de julho de 2026, “Adiciona consolidacao da Fase 0”.
- Todos os 77 arquivos encontrados estavam versionados; não havia arquivo não rastreado.
- `.megaignore` e `desktop.ini` têm zero byte. O primeiro não documenta nenhuma regra; o segundo é metadado acidental do Windows.
- Nenhum Markdown falhou na decodificação UTF-8 estrita; nenhum possui BOM UTF-8; não foram observados mojibakes aparentes.
- Não há duplicatas byte a byte. Há, entretanto, duplicação semântica extensa entre README, roadmap, documentos da fase, aulas, glossários e consolidação.

### Links, caminhos, índices e estado

Não foram encontrados links Markdown locais quebrados. Os índices principais apontam para arquivos existentes. A numeração 0–31 no roadmap e 1–12 nas aulas é consistente.

Problemas encontrados:

1. **Estado obsoleto em pastas paralelas — médio.** `avaliacoes/README.md:3–7`, `exercicios/README.md:3–7`, `estudos-dirigidos/README.md:3–7` e `estudos-de-caso/README.md:3–7` dizem que conteúdos “serão” criados. Avaliações, exercícios e estudo dirigido já existem em `consolidacao/`; estudo de caso separado não existe. Isso confunde a fonte canônica.
2. **Planejamento escrito no futuro após conclusão — baixo.** `plano-da-fase.md:3` ainda declara “12 aulas futuras”; `ementa.md:7,13` e `mapa-conceitual.md:3` mantêm linguagem anterior à implementação. É histórico útil, mas não está marcado como baseline congelada.
3. **README global desatualizado — médio.** `README.md:11,33,39` descreve o estágio inicial e afirma que aulas e exercícios não serão criados “no início”, sem uma seção clara de estado atual.
4. **Pasta de referências vazia de fontes — alto.** `referencias/README.md` só promete futuras referências. Nenhuma afirmação central das aulas é atribuída.
5. **Nome do repositório e capitalização — baixo.** O título `formacao-cs-mainframe-cobol` no README não coincide com o nome remoto codificado; “Mainframe/mainframe” varia entre título, nome comum e adjetivo sem regra plenamente aplicada.
6. **Arquivo de sistema versionado — baixo.** `desktop.ini` não cumpre função pedagógica ou de build.

## 5. Avaliação dos documentos globais

### Clareza e consistência

`README.md`, `DIRETRIZES_DO_PROJETO.md`, `DIRETRIZES_EDITORIAIS.md` e `MANIFESTO_PEDAGOGICO.md` convergem em princípios válidos: progressão, estudo autônomo, contextualização, explicação em camadas e rejeição de sintaxe sem fundamento. O público-alvo aparece no README, mas não há diagnóstico de entrada, teste de nivelamento nem trilhas para perfis tão diferentes quanto iniciante absoluto e desenvolvedor experiente.

O problema central é que “profundidade” é definida como desenvolvimento textual, não como exigência intelectual mensurável. `DIRETRIZES_EDITORIAIS.md` e `planejamento/criterios-de-qualidade.md` enfatizam texto corrido, exemplos e conexão futura, mas não exigem fontes, problemas não triviais, provas, experimentos, implementações, análise de complexidade, projetos ou revisão externa. Isso favorece material longo e bem apresentado sem assegurar rigor.

`ROADMAP.md` é claro como narrativa de progressão, mas insuficiente como currículo. Cada fase tem objetivo e ponte, porém não tem resultados de aprendizagem operacionais, tópicos obrigatórios detalhados, pré-requisitos verificáveis, carga, práticas, avaliações, bibliografia ou critério de aprovação.

`GUIA_DE_USO_DOS_PROMPTS.md` e `prompts/` são úteis para reprodutibilidade histórica. O risco é normativo: instruções repetidas em prompts, diretrizes, templates e planejamento podem divergir. Prompts concluídos deveriam ser arquivo histórico, e toda regra vigente deveria apontar para uma fonte normativa única.

`GLOSSARIO_INICIAL.md` e `glossario-da-fase.md` têm função sobreposta. O glossário da fase possui cerca de 800 linhas e repete para quase todo termo “relação com a Fase 0” e “conexão futura”, tornando-se mais enciclopédia local do que instrumento rápido de consulta.

### Recomendações documentais

- **Manter:** manifesto pedagógico, roadmap, diretrizes editoriais, critérios de qualidade, histórico de prompts e templates.
- **Fundir ou estabelecer hierarquia:** `DIRETRIZES_DO_PROJETO.md`, `DIRETRIZES_EDITORIAIS.md` e `planejamento/criterios-de-qualidade.md` devem ter responsabilidades exclusivas e referências cruzadas, não repetir as mesmas regras.
- **Dividir:** roadmap em visão global e especificações curriculares por área/fase, com resultados, carga, práticas e avaliações.
- **Simplificar:** glossário da fase e blocos repetidos de conexão futura; manter definição, exemplo, limites e fonte quando necessário.
- **Ampliar:** referências, política de fontes, público/pré-requisitos, critérios quantitativos de domínio, acessibilidade, ética, segurança e governança de mudanças.
- **Arquivar:** prompts concluídos e documentos de planejamento congelados devem ser explicitamente marcados como histórico para não competir com o estado corrente.
- **Referenciar:** cada fase futura deve apontar para competências globais e cada avaliação deve mapear itens a resultados de aprendizagem.

## 6. Avaliação do roadmap acadêmico

O CS2023 organiza a formação por conhecimento e competência em 17 áreas e enfatiza não apenas saber, mas demonstrar habilidades e disposições profissionais. Stanford exige matemática, ciência, fundamentos de engenharia, núcleo de CS, profundidade e projeto final; o currículo MIT 18-C inclui matemática discreta, álgebra linear ou otimização, equações diferenciais, programação, algoritmos, computabilidade/complexidade, sistemas e laboratório. O roadmap local, por contraste, contém títulos amplos sem profundidade, carga ou produtos verificáveis.

| Área | Cobertura atual | Lacuna | Prioridade | Recomendação |
|---|---|---|---|---|
| Lógica e matemática discreta | Planejada, mas superficial na Fase 3 | predicados, provas, indução, combinatória, recorrências, grafos/árvores com rigor | Alta | transformar em sequência formal com exercícios de demonstração |
| Probabilidade e estatística | Ausente | probabilidade, variáveis, inferência, estatística aplicada | Alta | criar eixo obrigatório antes de dados/observabilidade |
| Álgebra linear e cálculo | Ausentes | vetores, matrizes, transformações, cálculo e modelagem | Alta | incluir fundamentos e aplicações computacionais; calibrar profundidade ao perfil |
| Representação/arquitetura | Parcialmente coberta | álgebra booleana, ISA, assembly, caches, hierarquia, desempenho | Alta | detalhar laboratório e programação de baixo nível apropriada |
| Sistemas operacionais | Planejada, mas superficial | threads, concorrência, sincronização, virtualização, I/O e experimentos | Alta | incluir implementação/experimentos e análise de trade-offs |
| Estruturas de dados | Parcialmente coberta | arrays, listas, hashes, heaps, grafos, invariantes e implementação | Crítica | substituir “nível conceitual” por implementação, análise e provas |
| Algoritmos | Inadequada | assintótica, correção, recursão, D&C, guloso, DP, grafos, NP/complexidade | Crítica | criar núcleo clássico antes de “algoritmos corporativos” |
| Teoria da computação | Ausente | linguagens formais, autômatos, computabilidade, decidibilidade, Turing e complexidade | Alta | incluir sequência obrigatória própria |
| Linguagens de programação | Ausente como área | paradigmas, tipos, escopo, semântica, memória, compiladores e parsing | Alta | inserir fundamentos de PL e tradutores antes da especialização |
| Bancos de dados | Planejada, mas superficial | álgebra relacional, normalização, ACID, isolamento, índices, recuperação e planos | Alta | detalhar teoria, SQL, laboratório e projeto |
| Redes | Planejada, mas superficial | TCP/IP, DNS, HTTP, sockets, segurança e laboratórios | Alta | dividir redes de integração e exigir experimentos |
| Sistemas distribuídos | Parcial/implícita | consistência, disponibilidade, falhas, idempotência, retry, timeout e observabilidade | Alta | criar fase própria após redes/SO/bancos |
| Engenharia de software | Planejada, mas superficial | design, arquitetura, testes, CI/CD, revisão, refatoração, requisitos, incidentes | Alta | distribuir práticas em todo o curso, não concentrar numa fase |
| Segurança | Parcial e fragmentada | criptografia, autenticação, autorização, threat modeling, segurança operacional | Alta | eixo transversal e disciplina dedicada |
| Confiabilidade | Parcial no contexto corporativo | modelos de falha, resiliência, continuidade, DR e risco | Média-alta | formalizar métricas, exercícios e jogos de falha |
| Sociedade, ética e profissão | Quase ausente | ética, privacidade, acessibilidade, impacto social, responsabilidade | Alta | integrar transversalmente conforme CS2023 |
| Mainframe/COBOL | Bem representada em títulos | profundidade, laboratórios, fontes IBM, segurança/RACF, tooling e projeto ainda indefinidos | Alta | manter especialização, mas especificar competências práticas e fontes oficiais |
| Projetos e laboratórios | Um projeto final | prática progressiva, portfólio, capstones intermediários | Crítica | projeto/lab em cada bloco, com integração cumulativa |

Classificação sintética pedida:

- **Adequadamente coberta no plano:** contexto corporativo, batch, z/OS/JCL/VSAM/DB2/CICS/COBOL em amplitude nominal.
- **Planejada, mas superficial:** representação de dados, arquitetura, SO, estruturas, bancos, redes, engenharia de software e segurança básica.
- **Parcialmente coberta:** lógica discreta, algoritmos, confiabilidade, manutenção e modernização.
- **Ausente:** probabilidade/estatística, álgebra linear, cálculo, teoria da computação, fundamentos de linguagens/compiladores, sistemas distribuídos como disciplina, ética/acessibilidade e pesquisa.
- **Deslocada:** programação prática só aparece explicitamente muito tarde; estruturas de dados antes de uma linguagem prática torna implementação e análise artificiais.
- **Fragmentada/repetida:** conexões Mainframe/COBOL surgem em quase toda fase, enquanto fundamentos clássicos não recebem espaço equivalente.

## 7. Revisão da Fase 0 como conjunto

A ordem das aulas é coerente: contexto → sistema → componentes → dados → processamento → EPS → programa → fonte → execução → arquivos → ambientes → erros. As aulas 5 e 6, e em menor grau 7–9, poderiam ser unidades mais integradas porque repetem definições e exemplos.

A fase tem identidade: alfabetização conceitual corporativa. O problema é de escala. Aproximadamente 58,5 mil palavras equivalem a um livro curto para introduzir doze distinções básicas. O aluno percorre repetidamente cadastro, cobrança, folha, estoque, banco, governo, relatório e auditoria; lê em todas as aulas objetivo, problema, introdução, conexão corporativa, conexão Mainframe/COBOL, confusões, perguntas, síntese, glossário e domínio. A previsibilidade ajuda navegação, mas reduz ritmo e cria enchimento funcional.

O conjunto antecipa muitos termos — auditoria, rastreabilidade, integração, runtime, bytecode, VM, batch, ambiente, processo, dependência — sem prática ou modelos técnicos suficientes. Para alfabetização isso pode motivar, mas o glossário e as retomadas ampliam a carga extrínseca. Em contrapartida, faltam atividades curtas imediatamente após cada conceito, diagramas produzidos pelo aluno, classificação com feedback e pequenos experimentos de arquivo/ambiente que poderiam existir sem “ensinar programação”.

As conexões Mainframe/COBOL são úteis quando mostram arquivo, batch, ambiente e operação; tornam-se excessivas quando obrigatórias em todos os termos e seções. A fase prepara vocabulário para a Fase 1, mas não demonstra retenção. Hoje está mais próxima de um livro/apostila modular do que de um curso: possui explicação e avaliação, mas não feedback, aula prática, mediação, dados de dificuldade ou evidência de aprendizagem.

## 8. Revisão individual das 12 aulas

### Aula 1 — O que é tecnologia da informação

- **Ponto forte:** situa TI além de computador e conecta pessoas, processos, dados e tecnologia (`aula-01...md:45–83`).
- **Problemas/lacunas:** definição ampla mistura tecnologia, gestão da informação e sistemas de informação sem reconhecer fronteiras disciplinares; exemplos corporativos se acumulam; informação já é definida antes da aula própria.
- **Repetição:** “TI não é computador/programação/tela” reaparece em objetivo, problema, introdução, seção própria, confusões e síntese.
- **Severidade:** média editorial/pedagógica.
- **Recomendação:** condensar e explicitar que é uma definição operacional do curso, não consenso único.

### Aula 2 — O que é um sistema

- **Ponto forte:** componentes, fronteira, ambiente e interface são explicados com bons recortes (`aula-02...md:65–75`).
- **Problemas/lacunas:** “propósito” é tratado como requisito geral, embora sistemas naturais e sistemas emergentes não tenham propósito projetado; entrada–processamento–saída–feedback não descreve todos os sistemas; classificação natural/técnico/social/informacional pede fonte.
- **Repetição:** sistema não é tela/software é reiterado muitas vezes.
- **Severidade:** média factual/pedagógica.
- **Recomendação:** qualificar modelos como lentes úteis, não propriedades universais.

### Aula 3 — Hardware, software e pessoas

- **Ponto forte:** supera o clichê físico/lógico e introduz papéis humanos.
- **Problemas/lacunas:** dizer que software é “instrução, regra e comportamento” é metafórico; software inclui dados associados e documentação em algumas definições. Banco de dados é descrito como software (`:53`), confundindo DBMS com a base de dados.
- **Repetição:** relações pessoas/processos/dados retomam aulas 1 e 2 quase integralmente.
- **Severidade:** média factual.
- **Recomendação:** distinguir banco de dados de sistema gerenciador e usar definição terminológica referenciada.

### Aula 4 — Dados, informação e conhecimento

- **Ponto forte:** contexto, qualidade, validação e rastreabilidade têm exemplos concretos; reconhece que validação não garante verdade (`:111–117`).
- **Problemas/lacunas:** a progressão “dado → informação → conhecimento” (`:63–69`) é um modelo contestado, não uma lei; “dado é representação registrada de fato” exclui ou obscurece dados derivados, hipotéticos e sintéticos; conhecimento é antropocêntrico sem declarar escolha epistemológica.
- **Repetição:** exemplos de cadastro, folha, estoque, cobrança e governo reaparecem em todas as seções.
- **Severidade:** alta factual/conceitual, corrigível sem invalidar a aula.
- **Recomendação:** apresentar DIKW como modelo didático entre outros e separar dado, interpretação e evidência.

### Aula 5 — O que é processamento

- **Ponto forte:** diferencia coleta, armazenamento, consulta e transformação e relaciona regras a resultados.
- **Problemas/lacunas:** definição muito abrangente de processamento torna fronteiras instáveis; “individual, lote e contínuo” mistura dimensões diferentes e deixa streaming/interativo/transacional para alusões.
- **Repetição:** grande sobreposição com aulas 4 e 6.
- **Severidade:** média pedagógica.
- **Recomendação:** fundir parte com a Aula 6 ou usar um único estudo de caso progressivo.

### Aula 6 — Entrada, processamento e saída

- **Ponto forte:** entrada ruim, intermediários, saída técnica/útil e encadeamento são pedagogicamente eficazes.
- **Problemas/lacunas:** com cerca de 5,5 mil palavras, é a aula mais longa para um modelo simples; EPS pode induzir visão linear de sistemas interativos, concorrentes e orientados a eventos.
- **Repetição:** retoma extensamente processamento e qualidade de dados.
- **Severidade:** alta pedagógica/editorial pelo volume; baixa factual.
- **Recomendação:** reduzir e explicitar limites do modelo linear.

### Aula 7 — O que é um programa

- **Ponto forte:** distingue programa, sistema, aplicativo, ferramenta e tela; introduz programa armazenado/processo.
- **Problemas/lacunas:** “programa como especificação de comportamento” (`:37–45`) confunde programa com especificação; programa é uma implementação/descrição executável em uma linguagem, enquanto especificação pode ser não executável e independente da implementação. “Processo é instância ativa de programa” é aceitável como simplificação, mas precisa ser marcado como modelo inicial de SO.
- **Repetição:** os cenários de folha, cadastro, pagamento e relatório repetem EPS.
- **Severidade:** alta factual/terminológica.
- **Recomendação:** separar requisito, especificação, algoritmo, programa e processo.

### Aula 8 — O que é código-fonte

- **Ponto forte:** legibilidade, manutenção e distinção de configuração/script/executável são relevantes.
- **Problemas/lacunas:** “representação textual” é comum, mas nem toda linguagem-fonte precisa ser puramente textual; código-fonte não representa necessariamente “o programa” inteiro. Editor/IDE, comentários e legado ampliam demais o escopo.
- **Repetição:** programa/sistema/regra reaparece; mini glossário replica o glossário global.
- **Severidade:** média factual/editorial.
- **Recomendação:** usar “representação em linguagem de programação, geralmente textual” e reduzir termos laterais.

### Aula 9 — Compilação, interpretação e execução

- **Ponto forte:** rejeita falsa dicotomia compilado versus interpretado e reconhece modelos mistos (`:67–83`).
- **Problemas/lacunas:** definições de compilação (“forma preparada”) e interpretação (“condução”) são vagas; bytecode não é apenas uma etapa “entre fonte e execução final”; VM e runtime estão simplificados a ponto de não permitir comparação verificável. A questão objetiva 9 herda essa vagueza.
- **Repetição:** compilar não garante correção e executar não garante resultado aparecem em várias seções e novamente na Aula 12.
- **Severidade:** alta factual/pedagógica.
- **Recomendação:** definir tradução entre linguagens/representações, execução por máquina abstrata/concreta e exemplos contrastantes sem vincular linguagem a um único modelo.

### Aula 10 — Arquivos, pastas, formatos e extensões

- **Ponto forte:** distinção conteúdo/nome/formato/extensão/caminho é clara e útil; extensão não garante formato está correta.
- **Problemas/lacunas:** “arquivo como unidade de informação armazenada” é operacional, mas não universal; pasta/diretório e organização física/lógica variam por sistema operacional; texto/binário é apresentado como dicotomia intuitiva sem explicar que todo arquivo é bytes e “texto” depende de codificação.
- **Repetição:** extensão/formato é repetida em aula, exercícios, perguntas e prova.
- **Severidade:** média factual/pedagógica.
- **Recomendação:** introduzir bytes/codificação brevemente e explicitar dependência do SO.

### Aula 11 — Ambientes computacionais

- **Ponto forte:** mostra que ambiente não é só máquina e conecta configuração, permissão, dependência, versão e dados.
- **Problemas/lacunas:** local, servidor, corporativo, nuvem e mainframe não são categorias mutuamente exclusivas; desenvolvimento/teste/homologação/produção são convenções organizacionais, não taxonomia universal; “dados reais” em produção admite exceções controladas.
- **Repetição:** produção real/risco real e “funciona no meu ambiente” são reiterados.
- **Severidade:** média factual/editorial.
- **Recomendação:** apresentar eixos independentes (localização, finalidade, plataforma, governança).

### Aula 12 — O que é erro

- **Ponto forte:** análise por camadas, mensagens como pistas e rejeição de culpa automática são excelentes hábitos iniciais.
- **Problemas/lacunas:** a taxonomia `erro`/`defeito`/`falha` em `:41–47` não segue de modo consistente terminologias consolidadas de teste e confiabilidade; “erro” é usado para ação humana, estado, resultado e categoria genérica. Erro de ambiente/dado/regra/operacional mistura causa, local e natureza, logo as categorias podem se sobrepor.
- **Repetição:** compilar/executar não garante correção e exemplos corporativos retomam aulas 9–11.
- **Severidade:** alta factual/terminológica.
- **Recomendação:** escolher e citar uma taxonomia (por exemplo, falha observada, defeito interno, engano humano, incidente operacional) e declarar categorias não exclusivas.

## 9. Revisão da consolidação

- **Resumo geral:** integra a ordem das aulas, mas é principalmente uma paráfrase sequencial; quase não produz uma nova síntese ou caso unificador.
- **Guia de revisão:** é acionável, aponta corretamente aulas para lacunas e oferece critérios de autoexplicação. Falta registro de evidência e agenda de retomada.
- **Mapa integrado:** apresenta relações em prosa coerente, mas não é um mapa visual nem explicita relações de dependência, tensão, exceção ou retroalimentação.
- **Estudo dirigido:** cobre as 12 aulas de maneira equilibrada, exige produção própria e inclui cenários. A estrutura idêntica em todas as aulas é útil, porém previsível; não há solução comentada ou feedback graduado.
- **80 exercícios teóricos:** distribuição 30 definição, 20 comparação, 15 correção de frase e 15 cenários. Há variedade formal, mas forte redundância. Itens 1/51, 2/53, 14/38, 25/46/59, 29/65 e outros verificam quase a mesma distinção. Os cenários 66–80 são a parte mais diagnóstica. Itens 67, 70, 76 e 79 pedem “classifique” embora as categorias da Aula 12 se sobreponham; mais de uma resposta pode ser defensável se bem justificada.
- **22 perguntas dissertativas:** promovem integração maior que a prova objetiva, mas repetem exercícios 31–50 e a avaliação dissertativa. Não há amostra de resposta, grade de conteúdo ou limite de escopo.
- **Checklist:** os itens usam verbos observáveis (“explicar”, “diferenciar”, “analisar”), o que é melhor que declarações vagas. Ainda é autodeclaratório: não exige anexar exemplo, pontuação ou correção externa.
- **Plano:** três ritmos ajudam pessoas que trabalham, mas não há estimativa de horas; o ritmo intensivo concentra quatro aulas longas por dia e avaliação no quarto dia, provavelmente inviável para iniciante. “Ritmo aprofundado” relê tudo antes de testar, contrariando recuperação ativa precoce. Não há revisão espaçada depois de 1, 7, 21 dias.

## 10. Revisão das avaliações e exercícios

### Avaliação objetiva

As 40 questões têm gabarito internamente coerente e uma resposta claramente pretendida. Não encontrei troca de gabarito. O problema é discriminação: em quase todos os itens, a alternativa correta é completa e técnica, enquanto distratores são absurdos, absolutos ou metalinguísticos (“uma pergunta dissertativa”, “glossário incompleto”, “criar código COBOL”). É possível acertar por estilo e eliminação sem domínio.

Achados por questão/grupo:

- **Q1–8, Q10–18, Q20–26 e Q29–35:** claras, mas quase exclusivamente recordar/compreender; distratores obviamente falsos.
- **Q9:** “compilação garante que uma forma de preparação/tradução foi realizada” é excessivo: uma compilação pode falhar; o enunciado deveria tratar de compilação bem-sucedida e do que ela evidencia. **Alta.**
- **Q19, Q22 e Q27:** a resposta é plausível, mas categorias sobrepostas permitem outra análise; “indício” reduz o problema, porém justificativas deveriam aceitar hipóteses alternativas. **Média.**
- **Q21:** somar campo errado pode resultar de defeito lógico, mapeamento/configuração, metadado ou dado; “indício principal” é aceitável, não diagnóstico único. **Média.**
- **Q28:** avalia por que exemplos foram usados no material, não o conhecimento da disciplina. **Baixa.**
- **Q36, Q39 e Q40:** avaliam metaconhecimento do projeto, não alfabetização técnica. **Média.**
- **Q37:** distinção fonte/configuração é simplificada; configuração pode ser código declarativo e fonte pode incluir configuração. **Média.**
- **Q38:** lista problemas de qualidade como “erro de dado”, mas “sem contexto” pode ser problema de interpretação/modelagem. **Média.**

Não há pegadinha injusta; há o problema oposto: pistas excessivas. Recomenda-se substituir pelo menos metade por minicasos com alternativas plausíveis, pedir justificativa curta e mapear cada item a competência/dificuldade.

### Avaliação dissertativa e rubrica

As oito questões integram conceitos e Q2, Q4, Q7 e Q8 exigem aplicação. Entretanto, cada enunciado entrega o roteiro da “boa resposta”, reduzindo a necessidade de estruturar análise. A rubrica tem cinco níveis globais, mas não define pontos, pesos, critérios por questão nem exemplos limítrofes. “Adequado”, “forte” e “excelente” dependem de julgamento subjetivo. A decisão final usa “maioria das respostas”, sem nota mínima nem regra para erro conceitual grave.

Precisão deve ter peso eliminatório para conceitos nucleares; clareza, integração e exemplos podem ter escalas independentes. Dois avaliadores hoje poderiam atribuir níveis diferentes à mesma resposta.

## 11. Precisão técnica e factual

| Arquivo/linha | Ideia problemática | Motivo | Gravidade | Direção de correção |
|---|---|---|---|---|
| `aula-03...md:53` | banco de dados entendido como software | confunde base de dados com SGBD | Média | separar dados persistidos, banco e gerenciador |
| `aula-04...md:33–69` | DIKW como progressão | modelo contestado apresentado como estrutura natural | Alta | qualificar como modelo didático e citar fonte/crítica |
| `aula-07...md:37–45` | programa como especificação | confunde especificação e implementação executável | Alta | distinguir requisito, especificação, algoritmo e programa |
| `aula-07...md:117–123` | processo como instância ativa | simplificação de SO não declarada | Média | dizer “modelo introdutório comum” e adiar nuances |
| `aula-08...md:27` e glossários | fonte necessariamente textual | há representações visuais/estruturadas e código gerado | Média | usar “geralmente textual” |
| `aula-09...md:51–83,222–240` | compilação/interpretação/VM/runtime vagos | não estabelecem relações técnicas precisas | Alta | definir transformação, execução e ambiente com exemplos |
| `avaliacao-objetiva.md:55–59` | compilação “garante” preparação | ignora compilação malsucedida | Alta | explicitar “quando bem-sucedida” e limite da garantia |
| `aula-10...md:61–69` | texto versus binário | dicotomia sem codificação/bytes | Média | explicar interpretação de bytes por formato/encoding |
| `aula-11...md:73–113` | tipos de ambiente no mesmo eixo | categorias se sobrepõem | Média | separar finalidade, hospedagem, plataforma e governança |
| `aula-12...md:41–47` | erro/defeito/falha | taxonomia híbrida, sem fonte | Alta | adotar padrão explícito e categorias não exclusivas |
| `aula-12...md:73–101` | classes de erro exclusivas implícitas | causa, camada e efeito podem coexistir | Média | usar classificação multidimensional |
| `glossario-da-fase.md:1–801` | definições sem fontes | aparência de autoridade sem rastreabilidade | Alta | atribuir termos críticos a normas/livros oficiais |

Não foram encontradas afirmações desatualizadas sobre versões específicas de COBOL, IBM Z ou z/OS, porque a fase evita detalhes tecnológicos. Isso reduz erros temporais, mas também evidencia que a especialização ainda está apenas planejada.

## 12. Qualidade editorial

A voz é consistente, séria e sem tom promocional ostensivo. O português é compreensível e os títulos são estáveis. Os principais problemas são padrões, não deslizes isolados:

1. **Estrutura formularizada:** todas as aulas repetem objetivo, problema, introdução, conexão, confusões, reflexão, síntese, glossário e domínio. O template virou molde rígido.
2. **Redundância deliberada sem estratégia de recuperação:** conceitos são reexplicados em vez de recuperados por perguntas ou referência curta.
3. **Parágrafos de enumeração:** muitas frases acumulam seis a dez substantivos (“dados, arquivos, ambientes, permissões...”), aumentando volume sem aprofundar relações.
4. **Exemplos recorrentes:** banco, governo, folha, estoque, cobrança, relatório e cadastro aparecem em quase todas as aulas com variações pequenas.
5. **Conclusões previsíveis:** “não é apenas...”, “não basta...”, “futuramente...” e “em sistemas corporativos...” formam bordões editoriais.
6. **Capitalização:** “Mainframe” aparece como nome próprio genérico e “mainframe” como classe; a oscilação pode ser válida, mas não está documentada. Recomenda-se “mainframe” para a classe/plataforma em geral e nomes oficiais para produtos; “COBOL” sempre em caixa alta.
7. **Inglês:** runtime, batch, job, log e feedback são apresentados, mas a política de tradução/equivalência não é sistemática.
8. **Autoafirmações de rigor:** expressões como “compreensão sólida”, “de forma séria” e “maturidade” aparecem antes de evidência avaliativa. Devem ser substituídas por resultados observáveis.

## 13. Rigor acadêmico

Há resultados de aprendizagem, progressão, exercícios, avaliações, revisão e critérios de domínio. Falta transformar isso em sistema acadêmico verificável.

Na taxonomia cognitiva, a Fase 0 concentra-se em **recordar** e **compreender**; cenários alcançam **aplicar** e **analisar** em nível inicial. Quase não há **avaliar** alternativas com evidência e não há **criar** um artefato além de resumo pessoal. A leitura domina a carga. Não existem referências obrigatórias, experimentos, coleta de evidência, feedback especializado, banco de erros, projetos, revisão por pares ou avaliação supervisionada.

Fases futuras precisarão de:

- resultados por unidade com condições e critérios mensuráveis;
- pré-requisitos testados, não apenas declarados;
- problemas graduados e cumulativos;
- programação, laboratórios e projetos desde o ciclo básico;
- provas fechadas e abertas, práticas e orais quando pertinente;
- feedback, recuperação e reavaliação com versões diferentes;
- bibliografia primária/secundária e exercícios de leitura técnica;
- demonstrações matemáticas, análise de algoritmos e experimentos de sistemas;
- integração transversal de segurança, ética, comunicação e trabalho profissional;
- dados reais de tempo, dificuldade, erro e retenção para revisar o material.

## 14. Comparação com formação universitária forte

### Onde o projeto já está forte

Está forte em intenção de progressão, atenção a sistemas corporativos, operação, rastreabilidade, manutenção e contextualização de Mainframe/COBOL. Esses temas frequentemente recebem menos atenção em cursos generalistas. A Fase 0 oferece mais cuidado terminológico que muitos tutoriais rápidos.

### Onde está abaixo e o que está ausente

Comparado ao CS2023 e aos currículos oficiais consultados, está muito abaixo em especificidade curricular, matemática, algoritmos, teoria, sistemas, prática e avaliação. Stanford explicita unidades de matemática, ciência, engenharia, núcleo, profundidade e projeto; MIT explicita disciplinas de matemática discreta, álgebra/equações diferenciais, programação, algoritmos, computabilidade/complexidade, sistemas e laboratório. O projeto local lista fases sem carga equivalente e não contém teoria da computação, cálculo/álgebra linear/probabilidade, núcleo completo de algoritmos ou laboratórios progressivos.

### O que estudo independente pode reproduzir

Conteúdo teórico, leituras, listas, programação, laboratórios virtuais, projetos, revisão de código assíncrona, simulados, portfólio e avaliações orais remotas podem ser reproduzidos com boa qualidade. Mainframe pode ser praticado por emuladores, ambientes educacionais e acesso autorizado, desde que o plano especifique recursos e limites.

### O que pode ser simulado

Prazos, rubricas, pré-requisitos, provas cumulativas, projetos em equipe, defesa de projeto, revisão por pares, incidentes simulados, change management, laboratórios de redes/SO/bancos e capstone com cliente fictício podem aproximar experiências universitárias/profissionais.

### O que texto não substitui integralmente

Professor que diagnostica concepções erradas, colegas com soluções diversas, pesquisa orientada, comunidade acadêmica, laboratórios físicos especializados, acesso institucional, prova supervisionada, estágio, responsabilidade compartilhada e feedback humano longitudinal. O projeto deve declarar essa diferença e recomendar complementos, não afirmar equivalência plena.

## 15. Riscos

| Risco | Probabilidade | Impacto | Evidência | Mitigação |
|---|---|---|---|---|
| Volume crescer sem rigor | Alta | Alto | 58,5 mil palavras para alfabetização; roadmap de 32 fases | limites de carga, resultados e revisão por evidência |
| Material longo e pouco exigente | Alta | Alto | prova objetiva óbvia; repetição textual | substituir parte da leitura por problemas/labs |
| Baixa retenção | Alta | Alto | releitura extensa, pouca recuperação espaçada | quizzes cumulativos e agenda 1/7/21/60 dias |
| Atraso até prática | Alta | Alto | programação apenas após muitos fundamentos/fases | programação e experimentos graduais no Ciclo 1 |
| Roadmap não atingir CS forte | Alta | Crítico | áreas centrais ausentes | redesenho curricular antes da Fase 1 |
| Dependência de texto de IA | Alta | Alto | estilo formularizado e ausência de fontes | revisão humana, fontes, testes com alunos e autoria registrada |
| Conceitos sem fonte | Alta | Alto | `referencias/` sem bibliografia | política de citação e bibliografia por aula |
| Avaliações previsíveis | Alta | Alto | distratores absurdos e roteiros entregues | blueprint, itens plausíveis e validação piloto |
| Documentos divergirem | Alta | Médio | READMEs “futuros” após consolidação | fonte canônica, status e checagem automatizada |
| Burocracia documental | Alta | Médio | 9+ documentos da fase, glossário de 800 linhas, prompts | reduzir e hierarquizar documentos |
| Fragmentação excessiva | Média | Médio | 32 fases; fundamentos espalhados | agrupar em disciplinas/blocos com créditos |
| Desmotivação | Alta | Alto | quatro a seis mil palavras por aula sem prática | sessões menores, projetos e feedback rápido |
| Lacuna matemática/teórica | Alta | Crítico | roadmap omite áreas inteiras | núcleo formal obrigatório |
| Especialização tardia | Média | Médio | COBOL só na Fase 20 | manter profundidade posterior, mas usar demonstrações contextuais antes |
| Especialização precoce no discurso | Alta | Médio | Mainframe/COBOL citados em quase toda seção | reduzir menções ritualizadas |
| Falta de projetos integradores | Alta | Alto | apenas projeto final nomeado | capstones por ciclo |
| Manutenção difícil | Alta | Alto | definições replicadas em aulas/glossários/resumos | conteúdo canônico e testes de links/estado |

## 16. Achados priorizados

### Críticos (1)

1. **C1 — Roadmap incompatível com a ambição acadêmica.** `ROADMAP.md`, `ciclos/*.md`, `planejamento/estrutura-de-fases.md`: faltam núcleos inteiros, profundidade, carga, prática e avaliação. Compromete a capacidade de atingir o objetivo, não o estudo imediato da Fase 0.

### Altos (8)

1. **A1 — Referências inexistentes.** `referencias/README.md`, todas as aulas e glossários.
2. **A2 — Volume e repetição excessivos da Fase 0.** `aulas/aula-01...` a `aula-12...`.
3. **A3 — Prática e projetos atrasados/insuficientes.** `ROADMAP.md`, fases 0–12 e projeto apenas na Fase 31.
4. **A4 — Avaliação objetiva de baixa discriminação.** `consolidacao/avaliacao-objetiva.md`.
5. **A5 — Rubrica sem pesos e descritores analíticos.** `rubrica-de-correcao.md`, `avaliacao-dissertativa.md`.
6. **A6 — Simplificações terminológicas centrais.** aulas 4, 7, 9 e 12, conforme seção 11.
7. **A7 — Ausência de carga, pré-requisitos testáveis e domínio quantitativo.** roadmap, ementa e critérios de domínio.
8. **A8 — Ausência de feedback humano/revisão especializada e validação com alunos.** documentos globais e metodologia implícita.

### Médios (12)

1. **M1 — READMEs de estado contraditórios.** `avaliacoes/`, `exercicios/`, `estudos-dirigidos/`, `estudos-de-caso/`.
2. **M2 — README global desatualizado.** `README.md:11–39`.
3. **M3 — Regras duplicadas e risco de divergência.** diretrizes, manifesto, critérios, templates e prompts.
4. **M4 — Glossários excessivos e sobrepostos.** `GLOSSARIO_INICIAL.md`, `glossario-da-fase.md`, mini glossários.
5. **M5 — Mapa integrado é lista em prosa, não mapa de relações.** `mapa-integrado-de-conceitos.md`.
6. **M6 — Exercícios redundantes.** `exercicios-teoricos.md`, `perguntas-dissertativas.md`.
7. **M7 — Checklist depende de autodeclaração.** `checklist-final-de-dominio.md`.
8. **M8 — Plano sem horas/revisão espaçada e ritmo intensivo inviável.** `plano-de-estudo-sugerido.md`.
9. **M9 — Categorias conceituais sobrepostas sem qualificação.** aulas 2, 5, 11 e 12.
10. **M10 — Excesso de conexão ritualizada com Mainframe/COBOL.** aulas, glossário e templates.
11. **M11 — Pouca variação cognitiva e ausência de criação.** consolidação inteira.
12. **M12 — Público heterogêneo sem nivelamento ou trilhas.** `README.md:19–23` e plano de estudo.

### Baixos (7)

1. **B1 — `desktop.ini` vazio e versionado.**
2. **B2 — `.megaignore` vazio e sem função documentada.**
3. **B3 — linguagem futura em planejamento concluído.** plano, ementa e mapa.
4. **B4 — capitalização Mainframe/mainframe não normatizada.** vários documentos.
5. **B5 — títulos sem acentos em documentos/templates antigos.** editorial, não encoding.
6. **B6 — questão 28 e itens metacurriculares 36/39/40.** `avaliacao-objetiva.md`.
7. **B7 — poucos parágrafos exatamente duplicados, mas forte repetição semântica.** aulas 7–9 e glossários.

## 17. O que corrigir antes de estudar a Fase 0

Não há problema que impeça totalmente o estudo imediato. Há, contudo, três correções que reduziriam prejuízo significativo:

1. qualificar as taxonomias das aulas 4, 7, 9 e 12, para que o aluno não memorize simplificações como definições universais;
2. fornecer uma rota reduzida/essencial, porque a extensão pode impedir conclusão e retenção;
3. não usar a prova objetiva atual como evidência suficiente de domínio; exigir respostas de cenário corrigidas por pessoa competente.

As inconsistências de pasta, capitalização e estado não impedem o aluno.

## 18. O que pode ser corrigido durante o estudo

- registrar tempo real por aula e pontos de abandono;
- marcar trechos repetitivos e exemplos que não acrescentam compreensão;
- testar quais termos exigem glossário e quais podem ser removidos;
- coletar respostas erradas para melhorar distratores e rubrica;
- ajustar plano de estudo, ritmo e revisão espaçada com dados do aluno;
- decidir se aulas 5/6 e 7/8/9 devem ser condensadas;
- uniformizar capitalização, títulos e traduções;
- limpar placeholders e documentos históricos depois de definir governança.

## 19. O que corrigir antes da Fase 1

1. Redesenhar o roadmap acadêmico e inserir as áreas ausentes.
2. Definir quando programação prática começa; não deixar estruturas/algoritmos apenas conceituais.
3. Especificar competências, pré-requisitos, carga, laboratórios, projetos e avaliações por fase.
4. Criar política de fontes e bibliografia; revisar definições críticas.
5. Pilotar a Fase 0 com aluno real e revisar por evidência.
6. Reduzir o corpus da Fase 0 ou criar trilha essencial versus aprofundamento.
7. Reconstruir avaliação objetiva, rubrica e decisão de domínio.
8. Definir fonte canônica e status dos documentos.
9. Criar plano transversal de matemática, segurança, ética, comunicação e engenharia.
10. Estabelecer capstone/laboratório por ciclo, não apenas ao final.

## 20. Proposta de evolução do roadmap

Sem reescrevê-lo, recomenda-se:

- reorganizar 32 fases em blocos equivalentes a disciplinas, com créditos/horas e dependências;
- introduzir programação e ambiente prático no primeiro ciclo, paralelamente aos fundamentos;
- expandir matemática em discreta formal, probabilidade/estatística e álgebra linear; justificar cálculo conforme perfil;
- criar núcleo de algoritmos/estruturas com implementação, provas e complexidade;
- criar teoria da computação e fundamentos de linguagens/compiladores;
- aprofundar arquitetura/SO com assembly, concorrência, memória, I/O e virtualização;
- separar redes de sistemas distribuídos e integração corporativa;
- tornar segurança, ética, confiabilidade, comunicação e dados eixos transversais;
- exigir laboratório e projeto em cada bloco, com um projeto integrador por ciclo;
- preservar o bloco Mainframe/COBOL, acrescentando fontes IBM, acesso prático, segurança, operação, teste, observabilidade e modernização baseada em casos;
- declarar o que é núcleo obrigatório, aprofundamento e eletiva.

## 21. Plano de ação recomendado

### Etapa A — correções imediatas

| Ação | Prioridade | Esforço | Dependências | Resultado esperado |
|---|---|---|---|---|
| qualificar definições críticas | Alta | Médio | fontes escolhidas | evitar aprendizagem conceitual rígida/incorreta |
| criar rota essencial da Fase 0 | Alta | Médio | análise de redundância | reduzir abandono sem perder competências |
| tornar rubrica analítica | Alta | Médio | blueprint de competências | correção reproduzível |
| revisar prova objetiva | Alta | Médio | piloto de itens | maior discriminação |

### Etapa B — estudo real da Fase 0

| Ação | Prioridade | Esforço | Dependências | Resultado esperado |
|---|---|---|---|---|
| aplicar diagnóstico inicial | Alta | Baixo | questões de entrada | baseline do aluno |
| registrar horas, dúvidas e erros | Alta | Baixo | formulário simples | evidência de carga/dificuldade |
| usar recuperação ativa semanal | Alta | Médio | banco de questões | retenção mensurável |
| obter correção humana de respostas | Alta | Médio | avaliador competente | detectar falsas compreensões |

### Etapa C — revisão após feedback do aluno

| Ação | Prioridade | Esforço | Dependências | Resultado esperado |
|---|---|---|---|---|
| cortar/fundir repetições | Alta | Alto | dados da Etapa B | material mais eficiente |
| calibrar exercícios e ritmos | Alta | Médio | resultados reais | dificuldade e carga realistas |
| revisar exemplos e glossários | Média | Médio | dúvidas coletadas | foco em conceitos que causam erro |

### Etapa D — revisão estrutural do roadmap

| Ação | Prioridade | Esforço | Dependências | Resultado esperado |
|---|---|---|---|---|
| mapear CS2023 e currículos oficiais | Crítica | Alto | escolha de perfil | cobertura demonstrável |
| definir disciplinas, horas e pré-requisitos | Crítica | Alto | mapa de competências | progressão executável |
| inserir matemática, teoria, PL, distribuídos e segurança | Crítica | Alto | desenho global | base genuína de CS |
| planejar labs e capstones por ciclo | Crítica | Alto | recursos disponíveis | domínio prático cumulativo |

### Etapa E — preparação da Fase 1

| Ação | Prioridade | Esforço | Dependências | Resultado esperado |
|---|---|---|---|---|
| definir resultados observáveis e avaliação | Alta | Médio | Etapa D | fase verificável |
| decidir linguagem/ferramentas introdutórias | Alta | Médio | estratégia prática | reduzir atraso até fazer computação |
| selecionar bibliografia e fontes | Alta | Médio | escopo fechado | precisão e leitura acadêmica |
| criar piloto curto antes do módulo completo | Alta | Médio | anteriores | validar método antes de crescer |

## 22. Veredito final

**Classificação: estudável, mas precisa de revisão antes da Fase 1.**

A Fase 0 pode ser estudada agora com cautela: é organizada, majoritariamente correta, possui sequência, exercícios e consolidação. Não requer paralisação completa nem foi encontrado erro crítico interno que invalide as 12 aulas. Entretanto, o volume, a repetição, as simplificações terminológicas e a baixa força diagnóstica das avaliações impedem classificá-la como excepcionalmente sólida.

Para o projeto completo, a situação é mais séria. O roadmap atual não sustenta a promessa de formação universitária forte: áreas fundamentais estão ausentes ou reduzidas a títulos, e não há carga, laboratórios, projetos progressivos, bibliografia ou avaliação compatível. Avançar diretamente para a Fase 1 sem corrigir essa arquitetura aumentaria o custo de mudança e perpetuaria um padrão de texto extenso com rigor não demonstrado.

O projeto tem uma boa fundação editorial e uma especialização final coerente, mas ainda não tem um currículo acadêmico completo. O próximo avanço responsável é estudar/pilotar a Fase 0, corrigir suas definições e avaliações, e redesenhar o roadmap antes de produzir a Fase 1.
