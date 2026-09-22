<h1 id="11h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $n=\prod_{p^\alpha\parallel n}p^\alpha$, multiplicativity and the prime-power formula for the [divisor function](../../../../../../divisor-function.md) give

$$
\frac{\tau(n)}{n^\epsilon}
=\prod_{p^\alpha\parallel n}\frac{\alpha+1}{p^{\alpha\epsilon}}.
$$

Choose $P_0=2^{1/\epsilon}$. For $p\geq P_0$ and $\alpha\geq1$, the elementary bound $\alpha+1\leq2^\alpha$ gives

$$
\frac{\alpha+1}{p^{\alpha\epsilon}}\leq1.
$$

For each of the finitely many primes $p<P_0$, the sequence $(\alpha+1)p^{-\alpha\epsilon}$ tends to zero and therefore has a finite maximum $M_p$ over $\alpha\geq0$. Consequently

$$
\frac{\tau(n)}{n^\epsilon}
\leq C(\epsilon):=\prod_{p<P_0}M_p<\infty,
$$

uniformly in $n$, which proves $\tau(n)\leq C(\epsilon)n^\epsilon$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
