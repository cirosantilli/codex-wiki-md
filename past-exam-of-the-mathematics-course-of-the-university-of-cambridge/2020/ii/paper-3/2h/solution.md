<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

The [polynomial Runge theorem](../../../../../polynomial-runge-theorem.md) says that if $K\subset\mathbb C$ is [compact](../../../../../compact-space.md), $\mathbb C\setminus K$ is [connected](../../../../../connected-space.md), and $f$ is [holomorphic](../../../../../holomorphic-function.md) on a neighbourhood of $K$, then for every $\varepsilon>0$ there is a [polynomial](../../../../../polynomial-split.md) $p$ such that $\sup_{z\in K}|p(z)-f(z)|<\varepsilon$.

For an explicit approximation on the left semicircle $K=\{z:|z|=1,\operatorname{Re}z\leq0\}$, define

$$
p_n(z)=-\frac14\sum_{j=0}^n\sum_{k=0}^{n^2}\binom{j+k}{k}\left(\frac z4\right)^k.
$$

The two [power-series expansions](../../../../../power-series.md)

$$
\frac1z=\sum_{j=0}^{\infty}\frac{(-4)^j}{(z-4)^{j+1}},
\qquad
\frac1{(z-4)^{j+1}}=\frac1{(-4)^{j+1}}\sum_{k=0}^{\infty}\binom{j+k}{k}\left(\frac z4\right)^k
$$

produce this formula. The first is a [geometric series](../../../../../geometric-series.md) whose ratio has modulus at most $4/\sqrt{17}<1$ on $K$. The second converges uniformly on the whole [unit circle](../../../../../complex-unit-circle.md); the elementary bound $\binom{j+k}{k}\leq2^{j+k}$ shows that truncating it at $k=n^2$ gives a total error tending to zero even after summing over $0\leq j\leq n$. Consequently $p_n\to1/z$ [uniformly](../../../../../uniform-convergence.md) on $K$. This is an [explicit polynomial approximation of the reciprocal on the left semicircle](../../../../../explicit-polynomial-approximation-of-the-reciprocal-on-the-left-semicircle.md).

**No such sequence exists on the punctured unit circle $S=\{z:|z|=1,z\ne1\}$.** If polynomials $p_n$ converged uniformly there, they would be [Uniformly Cauchy](../../../../../uniformly-cauchy-sequence.md). Continuity gives

$$
\sup_{|z|=1}|p_n(z)-p_m(z)|=\sup_{z\in S}|p_n(z)-p_m(z)|,
$$

so they would converge uniformly on the entire unit circle. The [uniform limit theorem](../../../../../uniform-limit-theorem.md) would force the value at the missing point to be $1$, and hence the limit would be $1/z$ on the full circle. But the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) gives $\oint p_n(z)\,dz=0$ for every $n$, while [uniform convergence and contour integration](../../../../../uniform-convergence-and-contour-integration.md) would imply

$$
0=\lim_{n\to\infty}\oint p_n(z)\,dz=\oint\frac{dz}{z}=2\pi i,
$$

a contradiction. This is the [polynomial approximation obstruction on a punctured circle](../../../../../polynomial-approximation-obstruction-on-a-punctured-circle.md).

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
