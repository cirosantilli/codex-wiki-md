<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let regeneration cycles have lengths $C_i$, contain $A_i$ arrivals, and accrue queue-length reward

$$
R_i=\int_{\text{cycle }i}Q(t)dt.
$$

Fubini's geometric identity writes this area as the sum, over customers in the cycle, of their time in the system, up to boundary terms whose contribution vanishes over many cycles. The renewal-reward theorem therefore gives

$$
L=\frac{\mathbb ER_1}{\mathbb EC_1},
\qquad
\lambda=\frac{\mathbb EA_1}{\mathbb EC_1},
\qquad
W=\frac{\mathbb ER_1}{\mathbb EA_1}.
$$

Hence [Little law](../../../../../../little-s-law.md) is

$$
\boxed{L=\lambda W.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
