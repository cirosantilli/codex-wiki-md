<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $\operatorname{Re}s>1$, the [Euler product](../../../../euler-product.md) theorem is

$$
\boxed{F(s)=\prod_{p}\left(\sum_{e=0}^\infty f(p^e)p^{-es}\right).}
$$

The local series converge absolutely, and the product is [absolutely convergent](../../../../absolute-convergence.md) in the sense that the sum over [primes](../../../../prime-number-split.md) of the absolute deviations of the local factors from one is finite. Indeed this sum is bounded by $\sum_{n\ge2}|f(n)|n^{-\operatorname{Re}s}$. To prove the identity, expand the product over [primes](../../../../prime-number-split.md) at most $y$. [Absolute convergence](../../../../absolute-convergence.md) permits all those local expansions, and multiplicativity identifies the [coefficients](../../../../coefficient.md) with $f(n)$ for [integers](../../../../integer-split.md) whose [prime](../../../../prime-number-split.md) factors are at most $y$. Every omitted [integer](../../../../integer-split.md) exceeds $y$, so the difference from the full [Dirichlet series](../../../../dirichlet-series.md) is bounded by its absolute tail beyond $y$, which tends to zero. The same tail bound on a closed right half-plane inside $\operatorname{Re}s>1$ proves local [uniform convergence](../../../../uniform-convergence.md). With signed [coefficients](../../../../coefficient.md) a local factor can be zero; the identity does not require claiming every such general [Euler product](../../../../euler-product.md) is nonzero.

For $d(n^2)$, multiplicativity gives local [coefficients](../../../../coefficient.md) $d(p^{2e})=2e+1$. With $z=p^{-s}$,

$$
\sum_{e\ge0}(2e+1)z^e=\frac{1+z}{(1-z)^2}=\frac{1-z^2}{(1-z)^3}.
$$

The divisor bound from (1), applied with a sufficiently small exponent, proves [absolute convergence](../../../../absolute-convergence.md) when $\operatorname{Re}s>1$; divergence at one follows from $d(n^2)\ge1$. Multiplying the local identities therefore gives

$$
\boxed{\sum_{n\ge1}\frac{d(n^2)}{n^s}=\frac{\zeta(s)^3}{\zeta(2s)}.}
$$

For $n\le x$, the inequality $n^\delta\le x^\delta$ gives $d(n^2)/n\le x^\delta d(n^2)/n^{1+\delta}$. Sum those nonnegative terms and enlarge to the whole infinite series to get the required comparison.

For real $1<s<2$, integral comparison gives $\zeta(s)\le1+(s-1)^{-1}\le2/(s-1)$, while $\zeta(2s)\ge1$. Hence $\zeta(s)^3/\zeta(2s)=O((s-1)^{-3})$ uniformly in that interval. Choosing $\delta=1/\log x$ for $x\ge3$ makes $0<\delta<1$ and $x^\delta=e$. Thus

$$
\boxed{\sum_{n\le x}\frac{d(n^2)}n=O((\log x)^3).}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
