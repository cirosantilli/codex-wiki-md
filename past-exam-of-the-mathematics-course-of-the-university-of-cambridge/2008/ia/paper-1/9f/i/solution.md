<h1 id="9f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [comparison test for series](../../../../../../comparison-test-for-series.md) says that an eventual upper bound by a convergent positive [series](../../../../../../series-mathematics.md) proves convergence, while an eventual lower bound by a divergent positive [series](../../../../../../series-mathematics.md) proves divergence. The [p-series](../../../../../../p-series.md) $\sum n^{-s}$ converges exactly when $s>1$.

If $p>1$, then $(\log n)^q\geq1$ for all sufficiently large $n$, so

$$
0<\frac1{n^p(\log n)^q}\leq\frac1{n^p},
$$

and the [series](../../../../../../series-mathematics.md) converges. If $0<p<1$, choose $\eta=(1-p)/2>0$. The allowed logarithmic bound, applied with exponent $\eta/q$, gives $(\log n)^q<n^\eta$ eventually. Thus

$$
\frac1{n^p(\log n)^q}>\frac1{n^{p+\eta}},\qquad p+\eta=(p+1)/2<1,
$$

and the [series](../../../../../../series-mathematics.md) diverges.

For $p=1$, use the [integral test for convergence](../../../../../../integral-test-for-convergence.md): for an eventually positive decreasing function $g$, $\sum g(n)$ and $\int g(x)\,dx$ either both converge or both diverge. Here $g(x)=1/[x(\log x)^q]$ is decreasing for $x>1$, and the substitution $u=\log x$ gives

$$
\int_2^\infty\frac{dx}{x(\log x)^q}
=\int_{\log2}^\infty u^{-q}\,du.
$$

This integral converges exactly when $q>1$. Hence the [polynomial-logarithmic series convergence](../../../../../../polynomial-logarithmic-series-convergence.md) classification is

$$
\boxed{\text{Convergence iff }p>1\text{ or }(p=1\text{ and }q>1).}
$$

All other allowed positive $p,q$ give divergence.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
