<h1 id="12h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [probability distributions](../../../../../../probability-distribution.md) $p,q$ with positive entries, [Gibbs inequality](../../../../../../gibbs-inequality.md) is

$$
D(p\Vert q)=\sum_jp_j\log\frac{p_j}{q_j}\geq0,
$$

with equality exactly when $p=q$. Indeed, $\log x\leq x-1$, with equality only at $x=1$, gives

$$
- D(p\Vert q)=\sum_jp_j\log(q_j/p_j)\leq\sum_j(q_j-p_j)=0.
$$

This also proves the equality condition. With zero entries the same [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) statement holds using $0\log(0/q)=0$ and $p\log(p/0)=+\infty$ for $p>0$, or by restricting to the support and taking limits.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12H](../../12h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
