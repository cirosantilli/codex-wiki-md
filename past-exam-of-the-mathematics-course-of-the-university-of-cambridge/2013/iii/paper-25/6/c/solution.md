<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Continuity and adaptedness make the first boundary hit a [stopping time](../../../../../../stopping-time.md). A continuous path starting in the open domain cannot leave it before meeting its boundary. Thus $X_{t\wedge T}\in\mathcal D\cup\partial\mathcal D$, with the usual interpretation when $T=\infty$. If $|u|\le K$ on this set, then

$$
|M_{t\wedge T}|=e^{-\lambda(t\wedge T)}|u(X_{t\wedge T})|\le K.
$$

The stopped process is a bounded [local martingale](../../../../../../local-martingale.md); the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes it a martingale and, in fact, a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md). The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives **almost sure and $L^1$ convergence** as $t\to\infty$.

Its limit can also be identified pathwise. On $\{T<\infty\}$ the stopped process is eventually constant at $e^{-\lambda T}u(X_T)$. On $\{T=\infty\}$ its absolute value is at most $Ke^{-\lambda t}$ and hence tends to zero. Thus the limit is $e^{-\lambda T}u(X_T)\mathbf1_{\{T<\infty\}}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
