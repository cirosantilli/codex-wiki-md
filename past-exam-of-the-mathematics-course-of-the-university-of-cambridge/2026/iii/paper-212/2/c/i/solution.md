<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expanding the square and using the independence of the percolation edges gives

$$
\mathbb EX_r^2
=\sum_{\gamma,\gamma'}\mu(\gamma)\mu(\gamma')
\frac{\mathbb P(\gamma,\gamma'\text{ open})}
{\mathbb P(\gamma\text{ open})\mathbb P(\gamma'\text{ open})}.
$$

The ratio equals $p^{-N_r(\gamma,\gamma')}$, where $N_r$ is the number of common edges in the two truncated paths. It is at most $p^{-N}$ for $N=|\xi\cap\xi'|$, under the convention in the hypothesis; in particular $N\geq1$ because both paths contain $o$. For every integer $N\geq1$,

$$
p^{-N}\leq\sum_{n=1}^Np^{-n}.
$$

The [tail-sum formula](../../../../../../../tail-sum-formula.md) and the assumed exponential intersection tail therefore yield

$$
\boxed{\mathbb EX_r^2
\leq\sum_{n=1}^\infty p^{-n}(\mu\times\mu)(N\geq n)
\leq C\sum_{n=1}^\infty\left(\frac\zeta p\right)^n
=\frac{C\zeta}{p-\zeta}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 212](../../../../paper-212-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
