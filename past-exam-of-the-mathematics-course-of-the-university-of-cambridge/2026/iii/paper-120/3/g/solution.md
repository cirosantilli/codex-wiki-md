<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Given a finite input word $w$, construct the typed term $\mathbf wq_0$ effectively and beta-normalize it. The [Strong normalization theorem for simply typed lambda calculus](../../../../../../strong-normalization-theorem-for-simply-typed-lambda-calculus.md) guarantees termination, and confluence gives exactly one of the finitely many normal forms $q_i$. Compare that normal form syntactically with the listed accepting states in $F$. This algorithm accepts exactly when $\delta^*(q_0,w)\in F$, so $L$ is recursive. Equivalently, this is the standard theorem that every language recognized by a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) is a [regular language](../../../../../../regular-language.md) and hence decidable.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
