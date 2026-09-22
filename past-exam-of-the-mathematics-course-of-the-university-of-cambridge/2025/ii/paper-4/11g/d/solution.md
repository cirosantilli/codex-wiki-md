<h1 id="11g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every prime in $(\sqrt X,X]$ is at least $\sqrt X$. Consequently the [primorial](../../../../../../primorial.md) satisfies

$$
P(X)\geq(\sqrt X)^{\pi(X)-\pi(\sqrt X)}.
$$

Combining this with part (c) and taking logarithms gives

$$
\bigl(\pi(X)-\pi(\sqrt X)\bigr)\frac{\log X}{2}
\leq X\log4,
$$

so

$$
\pi(X)\leq\pi(\sqrt X)+\frac{2X\log4}{\log X}
\leq\sqrt X+\frac{2X\log4}{\log X}.
$$

For $X\geq2$, the inequality $\log X\leq\sqrt X$ implies

$$
\sqrt X\leq\frac{X}{\log X}.
$$

Thus the [prime-counting upper bound from a primorial estimate](../../../../../../prime-counting-upper-bound-from-a-primorial-estimate.md) yields

$$
\pi(X)\leq(1+2\log4)\frac{X}{\log X}.
$$

We may take $c=1+2\log4$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
