<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $q$ be the true density and $p$ the announced density. The advantage of truthful reporting for the [logarithmic scoring rule](../../../../../../logarithmic-scoring-rule.md) is

$$
\mathbb E_q[\log q(Y)]-\mathbb E_q[\log p(Y)]
=\int q(y)\log\frac{q(y)}{p(y)}\,dy
=D_{\mathrm{KL}}(q\Vert p).
$$

The [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) is nonnegative, with equality exactly when the densities agree almost everywhere. For instance, [Jensen inequality](../../../../../../jensen-s-inequality.md) gives $\mathbb E_q[\log(p/q)]\le\log\mathbb E_q[p/q]\le0$; equality requires a constant likelihood ratio on the true support and no remaining mass outside it. Consequently

$$
\boxed{\mathbb E_q[\log q(Y)]\ge\mathbb E_q[\log p(Y)],
\quad\text{with equality iff }p=q\text{ a.e.}}
$$

This proves strict propriety when the expected log scores are well defined, for example with a finite true expected log density. A forecast assigning zero density to a set of positive true probability has score $-\infty$ there and cannot outperform the truth. The hint's strict $>0$ must be corrected to $\ge0$ to allow its equality case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
