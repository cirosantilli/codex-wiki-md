<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md) gives

$$
\sum_{n\leq x}\log n
=\sum_{d\leq x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\leq x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

By the [Stirling formula](../../../../../../stirling-formula.md), the left side is $\log(\lfloor x\rfloor!)=x\log x-x+O(\log x)$, while the assumed [Chebyshev estimate](../../../../../../chebyshev-estimate.md) gives $\psi(x)=O(x)$. Hence

$$
\sum_{n\leq x}\frac{\Lambda(n)}n=\log x+O(1).
$$

The contribution of proper [prime powers](../../../../../../prime-power.md) is bounded uniformly:

$$
\sum_{\substack{p^k\leq x\\k\geq2}}\frac{\log p}{p^k}
\leq\sum_p\frac{\log p}{p(p-1)}<\infty.
$$

Removing it leaves

$$
\boxed{\sum_{p\leq x}\frac{\log p}{p}=\log x+O(1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
