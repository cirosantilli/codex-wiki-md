# Binary divisibility automaton

↑ **Parent:** [Minimal deterministic finite automaton](minimal-deterministic-finite-automaton.md)

For a positive integer $m$, binary strings can be tested for divisibility by $m$ with residue states $0,\ldots,m-1$ and transition

$$
r\xrightarrow{b}2r+b\pmod m,
\qquad b\in\{0,1\}.
$$

The initial and accepting residue is zero. For $m=7$, all seven states are reachable and pairwise distinguishable, so this automaton is minimal.

## ↑ Ancestors (9)

1. [Minimal deterministic finite automaton](minimal-deterministic-finite-automaton.md)
2. [DFA minimization](dfa-minimization.md)
3. [Deterministic finite automaton](deterministic-finite-automaton.md)
4. [Finite-state machine](finite-state-machine.md)
5. [Formal language theory](formal-language-theory.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/12h/solution.md)
