# Guia de Uso dos Prompts

Este projeto será construído por prompts sucessivos. Para preservar coerência, cada prompt deve trabalhar em uma etapa pequena, verificável e alinhada ao roadmap.

Um prompt futuro não deve pedir a criação da formação inteira, de muitos módulos ao mesmo tempo ou de conteúdos avançados antes da base correspondente. O repositório deve crescer por continuidade: revisar o que já existe, identificar a próxima fase, definir escopo e só então criar ou revisar conteúdo.

## Regras para proximos prompts

Cada prompt futuro deve:

- trabalhar em uma etapa pequena;
- respeitar as diretrizes editoriais;
- não criar conteúdo superficial;
- não avançar para código antes da hora;
- desenvolver uma fase por vez;
- revisar os arquivos existentes antes de criar novos;
- manter consistência com o roadmap;
- atualizar documentos de planejamento quando necessário;
- preservar a progressão pedagógica.

## Como estruturar um bom pedido

Um bom pedido deve indicar a fase, o tipo de arquivo esperado e os limites da tarefa. Também deve lembrar que o conteúdo precisa ser desenvolvido em texto corrido, sem virar lista superficial.

Exemplo de pedido adequado:

> Desenvolva a Fase 0 — Alfabetização técnica. Antes de criar os arquivos, revise README.md, ROADMAP.md, DIRETRIZES_DO_PROJETO.md, DIRETRIZES_EDITORIAIS.md e planejamento/estrutura-de-fases.md. Crie apenas os documentos necessários para esta fase. Não crie código, exercícios práticos ou conteúdo de COBOL. Escreva em português do Brasil, com explicações desenvolvidas, conexão com as fases futuras e critérios de domínio.

## Como evitar avancos fora de hora

Se uma fase ainda está tratando de fundamentos, o prompt não deve pedir comandos, instalação de ferramentas ou exemplos de linguagem. Quando um tema futuro precisar ser mencionado, ele deve aparecer como conexão conceitual, não como conteúdo principal.

Por exemplo, na Fase 0 pode ser aceitável explicar que sistemas corporativos exigem vocabulário técnico, mas não é adequado ensinar JCL, COBOL ou DB2 nessa fase.

## Como pedir revisao quando o conteudo ficar raso

Use este modelo quando um arquivo parecer curto, superficial ou fragmentado:

> Revise o conteúdo de [caminho-do-arquivo] com base em DIRETRIZES_EDITORIAIS.md e planejamento/criterios-de-qualidade.md. O texto está superficial e precisa ser aprofundado. Não transforme a revisão em uma lista de tópicos. Explique os conceitos em camadas, melhore as transições, acrescente contexto de sistemas reais quando fizer sentido e preserve a progressão pedagógica da fase. Não avance para assuntos que pertencem a fases futuras.

## Como pedir continuidade

Ao continuar o projeto, o prompt deve dizer explicitamente qual é a próxima fase e o que não deve ser feito ainda. Isso reduz o risco de misturar planejamento, aula, exercício e código no mesmo passo.

A continuidade recomendada após esta fundação é desenvolver a Fase 0 — Alfabetização técnica, começando pela definição do escopo da fase e por seus critérios de domínio.
