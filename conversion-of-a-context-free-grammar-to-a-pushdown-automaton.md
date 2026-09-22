# Conversion of a context-free grammar to a pushdown automaton

↑ **Parent:** [Context-free grammar](context-free-grammar.md)

Store the start [nonterminal symbol](nonterminal-symbol.md) on a [stack](stack-data-structure.md). An [epsilon transition](epsilon-transition.md) nondeterministically replaces its top [nonterminal symbol](nonterminal-symbol.md) by a [production rule](production-rule.md) right-hand side. A top [terminal symbol](terminal-symbol.md) can be removed only while consuming the same input symbol. With a protected [stack bottom marker](stack-bottom-marker.md), enter a final control state when that marker is exposed. Requiring all input to have been read implements [acceptance by final state](acceptance-by-final-state.md). The [stack](stack-data-structure.md) records the unprocessed suffix of a [leftmost derivation](leftmost-derivation.md), proving equality of the recognized and generated [formal languages](formal-language.md).

## ↑ Ancestors (7)

1. [Context-free grammar](context-free-grammar.md)
2. [Context-free language](context-free-language.md)
3. [Formal language theory](formal-language-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/models-of-computation/2/b/iii/solution.md)
