# State elimination for finite automata

↑ **Parent:** [Generalized finite automaton](generalized-finite-automaton.md)

To remove an internal state $k$, replace each surviving label by $R_{ij}\cup R_{ik}(R_{kk})^*R_{kj}$. The added term accounts for entering $k$, traversing its loop any number of times, and leaving it. Fresh initial and final states allow all old states to be eliminated, producing a [regular expression](regular-expression.md) for the same language.

**Table of contents**

- [Finite-state path expression](finite-state-path-expression.md)

## ↑ Ancestors (7)

1. [Generalized finite automaton](generalized-finite-automaton.md)
2. [Finite-state machine](finite-state-machine.md)
3. [Formal language theory](formal-language-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/4h/a/solution.md)
