# Suffix-nonnegative binary language

↑ **Parent:** [Context-free language](context-free-language.md)

A [context-free language](context-free-language.md) recognized by scanning a [string](string.md) over the [alphabet](alphabet.md) $\{0,1\}$ from right to left, counting 0 as $+1$ and 1 as $-1$, and requiring every partial count to remain nonnegative. A [context-free grammar](context-free-grammar.md) with a unique [parse tree](parse-tree.md) for each generated [string](string.md) is $S\to\epsilon\mid S0\mid S1B0$, $B\to\epsilon\mid B1B0$. To see uniqueness, reverse the [strings](string.md): every nonempty nonnegative path either never returns to zero after its first step, or has a unique first return. These two cases determine the production and its component substrings.

## ↑ Ancestors (6)

1. [Context-free language](context-free-language.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation/10/b/i/solution.md)
