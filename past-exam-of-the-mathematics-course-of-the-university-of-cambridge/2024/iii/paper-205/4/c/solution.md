<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $B=\varnothing$, then for every $j$ at least one of $H_j^\beta$ and $H_j^\eta$ is true. Since

$$
\{q_j\leq t\}=\{q_j^\beta\leq t\}\cap\{q_j^\eta\leq t\},
$$

validity of the [p-value](../../../../../../p-value.md) for whichever component null is true implies $\mathbb P(q_j\leq t)\leq t$. Therefore the [union bound](../../../../../../boole-s-inequality.md) gives

$$
\mathbb P\!\left(\min_{1\leq j\leq p}q_j\leq\frac\alpha p\right)
\leq\sum_{j=1}^p\mathbb P\!\left(q_j\leq\frac\alpha p\right)
\leq\alpha.
$$

This is the [Bonferroni correction](../../../../../../bonferroni-correction.md) for the composite intersection alternatives.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
