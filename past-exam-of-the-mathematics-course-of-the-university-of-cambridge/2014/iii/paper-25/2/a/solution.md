<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Absolute convergence](../../../../../../absolute-convergence.md) and the [Fundamental theorem of arithmetic](../../../../../../fundamental-theorem-of-arithmetic.md) give the [Euler product](../../../../../../euler-product.md)

$$
\boxed{\zeta(s)=\prod_{p\ \mathrm{prime}}(1-p^{-s})^{-1},\qquad\Re s>1.}
$$

For a finite set of primes, expand the geometric factors: their product sums $n^{-s}$ over integers whose prime factors lie in that set. Let the finite sets increase through all primes. [Absolute convergence](../../../../../../absolute-convergence.md) permits passage to the limit and recovers the full [Dirichlet series](../../../../../../dirichlet-series.md). Moreover $\sum_{p,m\ge1}|p^{-ms}|/m<\infty$, so the logarithm converges and the product has no zeros there.

The same [absolutely convergent](../../../../../../absolute-convergence.md) logarithm, and $3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\ge0$, give

$$
\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1\quad(\sigma>1).
$$

This is the product version of the [three-four-one zero-free-region argument](../../../../../../three-four-one-zero-free-region-argument.md). It also proves there are no zeros on $\Re s=1$: if $\zeta(1+it_0)=0$ for $t_0\ne0$, its factor has order at least four as $\sigma\downarrow1$, while the real [pole](../../../../../../pole.md) contributes only order minus three and the $2t_0$ factor remains bounded. The displayed left side would tend to zero, a contradiction. At $t_0=0$ there is a [pole](../../../../../../pole.md), not a zero.

For large $|t|$, put $L=\log(|t|+2)$. The [Hardy-Littlewood approximation to the Riemann zeta function](../../../../../../hardy-littlewood-approximation-to-the-riemann-zeta-function.md) at $x\asymp|t|$ gives $|\zeta(\sigma+it)|\ll L$ for $1-2/L\le\sigma\le3$; its finite sum is bounded by $\sum_{n\le x}n^{-1+2/L}\ll L$ and the integral term is bounded. The [Cauchy estimate for derivatives](../../../../../../cauchy-estimate.md) on circles of radius comparable to $1/L$ consequently gives $|\zeta'(\sigma+it)|\ll L^2$ for $1-L^{-9}\le\sigma\le2$.

Take $\sigma_0=1+aL^{-9}$ with a small fixed $a>0$. The product inequality, $\zeta(\sigma_0)\ll L^9/a$, and $|\zeta(\sigma_0+2it)|\ll L$ imply

$$
|\zeta(\sigma_0+it)|\ge c_0a^{3/4}L^{-7}.
$$

If $1-cL^{-9}\le\sigma\le\sigma_0$, integration of the [derivative](../../../../../../derivative.md) along the horizontal segment changes this value by at most $C(a+c)L^{-7}$. Choose $a$ sufficiently small that $Ca<c_0a^{3/4}/4$, then $c\le a$ sufficiently small. The lower bound remains a positive multiple of $L^{-7}$. For $\sigma_0\le\sigma\le2$, the same product inequality, $\zeta(\sigma)\le\zeta(\sigma_0)$, and the near-one upper bound give that lower bound directly. For $\sigma\ge2$, the reciprocal [Euler product](../../../../../../euler-product.md) gives $|1/\zeta(s)|\le\zeta(2)$.

Finally the no-zero result on $\Re s=1$, [compactness](../../../../../../compact-space.md) at bounded heights and the regular reciprocal at the [pole](../../../../../../pole.md) allow a further fixed reduction of $c$ to include bounded $t$. We have proved the [weak logarithmic zero-free region for the Riemann zeta function](../../../../../../weak-logarithmic-zero-free-region-for-the-riemann-zeta-function.md)

$$
\boxed{\left|\frac1{\zeta(\sigma+it)}\right|\ll\log^7(|t|+2),\qquad\sigma\ge1-\frac c{\log^9(|t|+2)}.}
$$

The reciprocal at $s=1$ is its holomorphic extension, equal to zero.

## ↑ Ancestors (11)

1. [A](../a.md)
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
