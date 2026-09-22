<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Monotonicity of the ordered probabilities gives $ip_i\leq\sum_{j\leq i}p_j\leq1$, so $\log i\leq-\log p_i$. Consequently

$$
\mathbb E[L^*(X)]
=\sum_ip_i\lfloor\log i\rfloor
\leq\sum_ip_i\log i
\leq H(X).
$$

Given $L^*(X)=l$, the source symbol can take at most $2^l$ values. The [maximum entropy distribution on a finite set](../../../../../../maximum-entropy-distribution-on-a-finite-set.md) is uniform, hence

$$
H(X\mid L^*(X)=l)\leq\log2^l=l.
$$

Averaging this [conditional entropy](../../../../../../conditional-entropy.md) inequality proves

$$
\boxed{H(X\mid L^*(X))\leq\mathbb E[L^*(X)].}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
