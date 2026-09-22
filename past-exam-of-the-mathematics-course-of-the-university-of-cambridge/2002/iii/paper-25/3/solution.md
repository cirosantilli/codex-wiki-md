<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $s=\sigma+it$ and let $\rho=\beta+i\gamma$ run over [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md), including [multiplicity](../../../../../multiplicity-mathematics.md). The bounds involving $\log|t|$ below are for $|t|\ge3$. At bounded heights their uniform versions use $\log(|t|+3)$; $\log|t|$ itself cannot be the right bound near [zero](../../../../../zero-of-a-function.md) or $|t|=1$.

Start with the [Hadamard factorization](../../../../../hadamard-factorization-theorem.md) of the [Riemann xi function](../../../../../riemann-xi-function.md), an [entire function](../../../../../entire-function.md) of order one. Its [logarithmic derivative](../../../../../logarithmic-derivative.md) has the convergent expansion

$$
\frac{\xi'}{\xi}(s)=B+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right).
$$

Differentiating $\xi(s)=\tfrac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)$ gives

$$
\frac{\zeta'}{\zeta}(s)
=B+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right)
-\frac1s-\frac1{s-1}+\frac12\log\pi-\frac12\frac{\Gamma'}{\Gamma}(s/2).
$$

The real sum of $1/\rho$ converges absolutely: $0\le\beta\le1$ makes its terms $O(\gamma^{-2})$ at large height, and the order-one [Hadamard factorization](../../../../../hadamard-factorization-theorem.md) ensures the required summability. Thus these terms and $\Re B$ form a fixed constant. The [Stirling formula](../../../../../stirling-formula.md) for the [digamma function](../../../../../digamma-function.md) gives, uniformly for $1<\sigma\le2$ and $|t|\ge3$,

$$
F(\sigma+it):=-\Re\frac{\zeta'}{\zeta}(\sigma+it)
=\frac12\log|t|-\sum_\rho\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma)^2}+O(1).
$$

This is the useful real form of the [global partial-fraction expansion of the zeta logarithmic derivative](../../../../../global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md). Every term subtracted is nonnegative because the [Euler product](../../../../../euler-product.md) excludes [zeros](../../../../../zero-of-a-function.md) with $\beta>1$. At the simple [pole](../../../../../pole.md) $s=1$, one also has $F(\sigma)=1/(\sigma-1)+O(1)$ as $\sigma\downarrow1$.

The [three-four-one zero-free-region argument](../../../../../three-four-one-zero-free-region-argument.md) now detects a [zero](../../../../../zero-of-a-function.md) too close to one. The [Von Mangoldt function](../../../../../von-mangoldt-function.md) is nonnegative and the absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md) gives

$$
0\le3F(\sigma)+4F(\sigma+it)+F(\sigma+2it),
$$

because the corresponding coefficient at $n$ is $\Lambda(n)n^{-\sigma}[3+4\cos(t\log n)+\cos(2t\log n)]$. If $\beta+it$ is a [zero](../../../../../zero-of-a-function.md), retain its term in the expansion at height $t$ and discard the other nonpositive terms. The expansion at height $2t$ gives an upper bound even without retaining a particular [zero](../../../../../zero-of-a-function.md). We obtain, for an absolute constant $C_0>0$,

$$
\frac4{\sigma-\beta}\le\frac3{\sigma-1}+C_0\log|t|.
$$

Choose $0<a<1$ so small that $5/(9a)>C_0$, put $b=a/8$, and take $\sigma=1+a/\log|t|$. If $1-\beta\le b/\log|t|$, the last inequality would require

$$
\frac{32}{9a}\le\frac3a+C_0,
\qquad\text{or}\qquad\frac5{9a}\le C_0,
$$

a contradiction. Therefore

$$
\boxed{\zeta(\sigma+it)\ne0\quad\text{for}\quad
\sigma>1-\frac b{\log|t|},\quad |t|\ge3,}
$$

for some fixed $b>0$. This proves the required [zero-free region of the Riemann zeta function](../../../../../zero-free-region-of-the-riemann-zeta-function.md). Nonvanishing on $\Re s=1$ at bounded nonzero heights, proved in Question 2, and the isolation of [zeros](../../../../../zero-of-a-function.md) allow a decrease of $b$ giving the uniform formulation with $\log(|t|+3)$ as well. Near $s=1$, apply this observation to the nonzero [holomorphic function](../../../../../holomorphic-function.md) $(s-1)\zeta(s)$.

Next evaluate the real expansion at $\sigma=2$. The absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md) bounds $|\zeta'/\zeta(2+it)|\le\sum_n\Lambda(n)n^{-2}$ uniformly in $t$, so

$$
\sum_\rho\frac{2-\beta}{(2-\beta)^2+(t-\gamma)^2}
=\frac12\log|t|+O(1).
$$

Since $1\le2-\beta\le2$, each term on the left is at least $1/[4+(t-\gamma)^2]$. The [smoothed zeta zero-count bound](../../../../../smoothed-zeta-zero-count-bound.md) follows:

$$
\boxed{\sum_\rho\frac1{4+(t-\gamma)^2}\ll\log|t|.}
$$

Each [zero](../../../../../zero-of-a-function.md) satisfying $|t-\gamma|<1$ contributes more than $1/5$, so this also gives the [local zero count for the Riemann zeta function](../../../../../local-zero-count-for-the-riemann-zeta-function.md):

$$
\boxed{\#\{\rho:|t-\Im\rho|<1\}\ll\log|t|.}
$$

The same kernel sum is bounded at compact heights, since its tail converges uniformly there; the bounds with $\log(|t|+3)$ are consequently valid for all real $t$.

For completeness, the contour estimate used in Question 2 follows from these very formulas. Subtract the complex [logarithmic derivative](../../../../../logarithmic-derivative.md) expansion at $2+it$ from that at $\sigma+it$, with $1-b/(2\log(T+3))\le\sigma\le2$ and $|t|\le T$. Terms with $|t-\gamma|>1$ have differences $O((t-\gamma)^{-2})$, whose sum is $O(\log(|t|+3))$ by the kernel bound. There are $O(\log(|t|+3))$ remaining terms. After reducing $b$, the [zero-free region of the Riemann zeta function](../../../../../zero-free-region-of-the-riemann-zeta-function.md) separates every such [zero](../../../../../zero-of-a-function.md) horizontally from the half-width boundary by $\gg1/\log(T+3)$: their heights satisfy $|\gamma|\le T+1$. Thus on the left edge, and on the horizontal edges at $t=\pm T$, each reciprocal is $O(\log(T+3))$. The [Gamma function](../../../../../gamma-function.md) and [pole](../../../../../pole.md) terms satisfy the same required bound; at small heights on the left edge the [pole](../../../../../pole.md) distance is $\gg1/\log(T+3)$. This proves $|\zeta'/\zeta|\ll\log^2(T+3)$ on those edges and justifies the contour shift without choosing heights that dodge unknown [zeros](../../../../../zero-of-a-function.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
