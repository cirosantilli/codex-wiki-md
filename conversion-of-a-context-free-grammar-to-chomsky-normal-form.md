# Conversion of a context-free grammar to Chomsky normal form

↑ **Parent:** [Chomsky normal form](chomsky-normal-form.md)

To convert a [context-free grammar](context-free-grammar.md) to [Chomsky normal form](chomsky-normal-form.md), first add a fresh start symbol. Remove [epsilon productions](epsilon-production.md), retaining the exceptional start production only when the empty word is to remain in the language; then remove [unit productions](unit-production.md) and symbols that cannot participate in a terminal derivation. Replace each terminal occurring in a right-hand side of length at least two by a new nonterminal that produces that terminal. Finally split every right-hand side of length greater than two into binary productions using fresh nonterminals.

## ↑ Ancestors (8)

1. [Chomsky normal form](chomsky-normal-form.md)
2. [Context-free grammar](context-free-grammar.md)
3. [Context-free language](context-free-language.md)
4. [Formal language theory](formal-language-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/4g/b/solution.md)
