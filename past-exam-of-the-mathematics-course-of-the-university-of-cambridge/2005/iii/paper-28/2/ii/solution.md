<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A precise endpoint version of the [Perron formula](../../../../../../perron-s-formula.md) is as follows. If $F(s)=\sum_{n\geq1}a_nn^{-s}$ converges absolutely on $\Re s=c>0$, then, for $x>0$,

$$
\boxed{\sum_{n<x}a_n+\frac12\mathbf1_{x\in\mathbb N}a_x
=\lim_{T\to\infty}\frac1{2\pi i}
\int_{c-iT}^{c+iT}F(s)\frac{x^s}{s}\,ds.}
$$

When $x$ is not an [integer](../../../../../../integer.md), the left side is simply the sum over $n\leq x$.

Prove first the scalar kernel formula, with symmetric vertical limits:

$$
K(y)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}\frac{y^s}{s}\,ds
=\begin{cases}1,&y>1,\\1/2,&y=1,\\0,&0<y<1.\end{cases}
$$

For $y>1$, close the contour to the left and apply the [residue theorem](../../../../../../residue-theorem.md) at $s=0$; the exponential $e^{s\log y}$ makes the closing integral vanish. For $y<1$, close to the right, where there is no enclosed [pole](../../../../../../pole.md) and the exponential decreases. The usual semicircle estimate, or integration by parts on the closing arcs, justifies these limits. At $y=1$ the truncated integral is $\pi^{-1}\arctan(T/c)$, tending to $1/2$.

One also needs a uniform bound to pass through the [Dirichlet series](../../../../../../dirichlet-series.md). Pairing the two halves of the vertical integral gives, with $u=\log y$,

$$
K_T(y)=\frac{y^c}{\pi}\int_0^T
\frac{c\cos(tu)+t\sin(tu)}{c^2+t^2}\,dt.
$$

The cosine term is absolutely bounded. The sine term is uniformly bounded by integration by parts against the bounded sine integral $\int_0^v\sin(tu)\,dt/t$, since $t^2/(c^2+t^2)$ is increasing from zero to one. Thus $|K_T(y)|\leq C_cy^c$, independently of $T,y$.

For finite $T$, [absolute convergence](../../../../../../absolute-convergence.md) permits termwise integration, giving $\sum_na_nK_T(x/n)$. The uniform bound dominates this by $C_cx^c\sum_n|a_n|n^{-c}<\infty$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) and the scalar kernel formula now prove the boxed [Perron formula](../../../../../../perron-s-formula.md), including its half-weight endpoint convention.

For the link with [primes](../../../../../../prime-number.md), the [logarithmic derivative](../../../../../../logarithmic-derivative.md) of the [Euler product](../../../../../../euler-product.md) gives

$$
-\frac{\zeta'(s)}{\zeta(s)}=\sum_{n\geq1}\frac{\Lambda(n)}{n^s}\qquad(\Re s>1).
$$

Applying [Perron formula](../../../../../../perron-s-formula.md) therefore expresses the second [Chebyshev function](../../../../../../chebyshev-function.md) $\psi_0(x)$, with half weight at a prime-power endpoint, as the vertical integral of $-\zeta'/\zeta(s)\,x^s/s$. Shift this contour left, choosing heights away from zeros and using the partial-fraction expansion to control the integrand. The [pole](../../../../../../pole.md) at one contributes $x$, a nontrivial zero $\rho$ of multiplicity $m$ contributes $-m x^\rho/\rho$, the trivial zeros contribute $\sum_{k\geq1}x^{-2k}/(2k)$, and the [pole](../../../../../../pole.md) from $1/s$ contributes $-\zeta'(0)/\zeta(0)=-\log(2\pi)$. Thus the resulting [Riemann–von Mangoldt explicit formula](../../../../../../riemann-von-mangoldt-explicit-formula.md) is

$$
\psi_0(x)=x-\sum_\rho\frac{x^\rho}{\rho}
-\log(2\pi)-\frac12\log(1-x^{-2})\qquad(x>1),
$$

with zeros summed symmetrically in height. A truncated contour gives the corresponding truncated formula and remainder. **The [pole](../../../../../../pole.md) at one gives the main term for [primes](../../../../../../prime-number.md); zeros farther left give smaller oscillating corrections.** Zero-free regions therefore translate into error bounds for $\psi(x)$ and, by [partial summation](../../../../../../abel-s-summation-formula.md), for the [prime-counting function](../../../../../../prime-counting-function.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
