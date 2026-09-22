<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[absolute convergence](../../../../absolute-convergence.md) depends only on $\sigma=\operatorname{Re}s$, since $|a_nn^{-s}|=|a_n|n^{-\sigma}$. Let $A$ be the set of real $\sigma$ for which $\sum|a_n|n^{-\sigma}$ converges. Comparison with a convergent member shows that $A$ is upward closed. The hypotheses give a member of $A$ and a real number outside $A$, so its [infimum](../../../../infimum.md) $\sigma_0$ is finite. If $\sigma>\sigma_0$, some $\tau\in A$ lies below $\sigma$, giving convergence by comparison; if $\sigma<\sigma_0$, convergence would contradict the definition of the [infimum](../../../../infimum.md). Thus **$\sigma_0=\inf A$ is the [abscissa of absolute convergence of a Dirichlet series](../../../../abscissa-of-absolute-convergence-of-a-dirichlet-series.md)**. This argument leaves convergence on the boundary open.

Partition $1,\ldots,n$ according to $d=n/\gcd(k,n)$. Writing $k=(n/d)j$ identifies the part indexed by $d\mid n$ with the [integers](../../../../integer-split.md) $1\leq j\leq d$ [coprime](../../../../coprime-integers.md) to $d$. There are $\phi(d)$ of them. Counting the entire partition proves the [totient divisor-sum identity](../../../../totient-divisor-sum-identity.md)

$$
\boxed{\sum_{d\mid n}\phi(d)=n.}
$$

We use the multiplication theorem for absolutely convergent [Dirichlet series](../../../../dirichlet-series.md): their product is the [Dirichlet series](../../../../dirichlet-series.md) of the [Dirichlet convolution](../../../../dirichlet-convolution.md) of their coefficients. [absolute convergence](../../../../absolute-convergence.md) justifies rearrangement of the double sum. Here $0<\phi(n)\leq n$, so its series converges absolutely for $\sigma>2$, and

$$
\zeta(s)\sum_{n\geq1}\frac{\phi(n)}{n^s}
=\sum_{n\geq1}\frac{\sum_{d\mid n}\phi(d)}{n^s}
=\sum_{n\geq1}n^{1-s}=\zeta(s-1).
$$

The [Euler product](../../../../euler-product.md) implies $\zeta(s)\neq0$ for $\sigma>1$. Division gives

$$
\boxed{\sum_{n\geq1}\frac{\phi(n)}{n^s}
=\frac{\zeta(s-1)}{\zeta(s)}\quad(\operatorname{Re}s>2).}
$$

We finally use the [simple pole](../../../../simple-pole.md) of the [Riemann zeta function](../../../../riemann-zeta-function.md) at one, of residue one, and $0<\zeta(2)<\infty$. The quotient therefore tends to $+\infty$ as real $s\downarrow2$. If $\sum\phi(n)n^{-2}$ converged, its nonnegative terms would dominate the series at every real $s>2$, giving a uniform finite bound and a contradiction. Thus the series diverges at two; comparison then excludes [absolute convergence](../../../../absolute-convergence.md) at every $\sigma<2$. Combined with the convergence already proved, **the abscissa is exactly two**. This is the [totient Dirichlet series and its absolute convergence boundary](../../../../totient-dirichlet-series-and-its-absolute-convergence-boundary.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
