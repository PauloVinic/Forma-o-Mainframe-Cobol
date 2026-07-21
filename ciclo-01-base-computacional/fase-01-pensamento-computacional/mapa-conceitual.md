# Mapa Conceitual Textual — Fase 1

## Visão relacional

```text
situação observada
├─ produz sintomas ── evidências ──> hipóteses de causa
├─ envolve interessados ──> necessidades e critérios de sucesso
└─ é delimitada como PROBLEMA
   ├─ estado inicial ───────────────┐
   ├─ estado desejado ─────────────┤
   ├─ entradas, regras e recursos ─┤──> especificação verificável
   └─ restrições e escopo ─────────┘

PROBLEMA
├─ decomposição <── dependências e recomposição ──> partes
├─ abstração <── propósito, fronteira e detalhe ──> modelos
└─ padrões <── exemplos, diferenças e exceções ──> generalização
                         │
                         v
              escolha de REPRESENTAÇÕES
       ┌────────────┬───────────┬──────────────┐
       v            v           v              v
    tabelas     diagramas   fluxogramas    pseudocódigo
       └────────────┴──── rastreabilidade ─────┘
                         │
                         v
                     ALGORITMO
       entrada ──> passos efetivos ──> saída
                         │
          ┌──────────────┼──────────────┐
          v              v              v
      sequência       decisões       repetições
          └──────────────┼──────────────┘
                         v
              estados e transições
                         │
             tabelas de rastreamento
                         │
                         v
             módulos, contratos e composição
                         │
                         v
       comportamento esperado <──> observado
                         │
            testes ──> evidências ──> depuração
               ^                         │
               └──── correção e regressão
                         │
                         v
            solução suficientemente correta
                         │
        ┌────────────────┴────────────────┐
        v                                 v
  custo e eficiência              adequação e limites
        └──────── comparação e escolha ───┘
                         │
                         v
               implementação futura
```

## Relações que não são lineares

### Formulação e feedback

O problema não fica imutável depois da primeira descrição. Ao decompor, o aluno pode descobrir uma dependência omitida; ao testar, pode perceber que o critério de sucesso era ambíguo; ao comparar estratégias, pode encontrar restrição de custo não registrada. Essas descobertas retornam à formulação. Revisar não significa fracassar: significa manter rastreabilidade entre evidência e decisão.

### Decomposição, abstração e padrões

Decomposição separa aspectos para análise, mas precisa de abstração para escolher o detalhe útil. Abstração torna casos comparáveis, facilitando padrões. Padrões podem sugerir uma decomposição reutilizável, enquanto exceções revelam abstração excessiva. As três dimensões se corrigem mutuamente.

### Representação e algoritmo

Representação não é a solução em si. Um algoritmo pode ser representado em pseudocódigo, fluxograma ou linguagem natural estruturada; a mesma representação pode conter algoritmo correto, incorreto ou incompleto. Converter representações é um teste de clareza: divergências revelam ambiguidades ou perdas.

### Estado, controle e rastreamento

Sequência determina a ordem das transições. Decisão escolhe uma transição conforme condição. Repetição aplica transições enquanto houver continuidade e progresso. O rastreamento registra estados sucessivos e permite comparar o que deveria ocorrer com o que ocorreu.

### Correção, eficiência e adequação

Teste e depuração sustentam uma conclusão limitada sobre correção. Eficiência trata recursos consumidos; adequação considera contexto, clareza, risco e restrições. Uma solução pode ser correta e cara, eficiente e incorreta, ou correta e eficiente mas inadequada ao ambiente. Nenhuma dessas propriedades deve substituir as outras.

## Ciclos de revisão

1. **Ciclo de formulação:** descrição → ambiguidades → perguntas → nova descrição.
2. **Ciclo de modelagem:** abstração → exemplo/contraexemplo → ajuste de fronteira.
3. **Ciclo algorítmico:** passos → rastreamento → defeito → revisão dos passos.
4. **Ciclo de teste:** esperado → execução manual → observado → hipótese → correção → regressão.
5. **Ciclo de escolha:** solução correta → medição/contagem → comparação → decisão justificada.

## Conexões com o percurso

A Fase 0 fornece os conceitos de sistema, requisito, especificação, dado, entrada, processamento, saída, programa, erro, falha e evidência. A Fase 1 organiza esses conceitos em soluções. A Fase 2 aprofundará controle lógico sem linguagem; matemática discreta formalizará proposições, conjuntos, relações e funções; estruturas de dados darão formas de organizar os dados sobre os quais algoritmos operam; algoritmos corporativos aprofundarão estratégias recorrentes. COBOL só aparecerá depois que solução, algoritmo, representação e implementação puderem ser distinguidos.
