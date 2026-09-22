<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\psi(x)=\sum_{n\le x}\Lambda(n)$, where $\Lambda$ is the [Von Mangoldt function](../../../../../../von-mangoldt-function.md). The [Riemann–von Mangoldt explicit formula](../../../../../../riemann-von-mangoldt-explicit-formula.md), in its symmetric limiting form for $x>1$, is

$$
\psi_0(x)=x-\lim_{T\to\infty}\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}-\log(2\pi)-\frac12\log(1-x^{-2}).
$$

Here nontrivial zeros are counted with multiplicity, the limit is taken symmetrically through admissible heights, and $\psi_0$ assigns half weight at a jump. Its difference from $\psi$ is at most $(\log x)/2$. The [Euler product](../../../../../../euler-product.md) and part (a) exclude zeros with real part at least one. The [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md) leaves only the [trivial zeros of the Riemann zeta function](../../../../../../trivial-zero-of-the-riemann-zeta-function.md) at negative even integers outside $0<\Re\rho<1$; their already displayed logarithmic correction is $O(x^{-2})$ for large $x$. These terms and the constant are negligible in the requested asymptotic error, rather than literally absent from the exact formula.

A useful [truncated explicit formula for the second Chebyshev function](../../../../../../truncated-explicit-formula-for-the-second-chebyshev-function.md) is, uniformly for $2\le T\le x$,

$$
\psi(x)=x-\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}+O\left(\frac{x\log^2(xT)}T+\log x\right).
$$

One may first take a height in $[T,T+1]$ separated from zeros and then adjust to $T$ using the local count. The [local zero count for the Riemann zeta function](../../../../../../local-zero-count-for-the-riemann-zeta-function.md) is

$$
\boxed{\#\{\rho:0<\Re\rho<1,\ t\le\Im\rho\le t+1\}\ll\log(|t|+3).}
$$

It includes multiplicity and is uniform in real $t$. It follows by subtracting the [Riemann–von Mangoldt formula](../../../../../../riemann-von-mangoldt-formula.md) at endpoints, handling bounded heights separately and using conjugation for negative heights. Both closed endpoints change the count only by another local bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
