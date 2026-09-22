<h1 id="12i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extend $\delta:Q\times\Sigma\to Q$ to

$$
\widehat\delta:Q\times\Sigma^*\to Q
$$

by

$$
\widehat\delta(q,\varepsilon)=q,
\qquad
\widehat\delta(q,wa)=\delta(\widehat\delta(q,w),a).
$$

The [extended transition function of a deterministic finite automaton](../../../../../../extended-transition-function-of-a-deterministic-finite-automaton.md) processes a whole word from left to right. The language accepted by $D$ is

$$
\boxed{L(D)=\{w\in\Sigma^*:\widehat\delta(q_0,w)\in F\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12I](../../12i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
