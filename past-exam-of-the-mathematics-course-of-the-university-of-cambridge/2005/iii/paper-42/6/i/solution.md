<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [Edgeworth expansion](../../../../../../edgeworth-series.md) refines the [central limit theorem](../../../../../../central-limit-theorem.md) by incorporating higher [cumulants](../../../../../../cumulant.md). For iid centred observations with [variance](../../../../../../variance-split.md) $\sigma^2$, standardized sum $Z_n=\sum_iX_i/(\sigma\sqrt n)$, standardized third cumulant $\gamma_1=\kappa_3/\sigma^3$ and fourth cumulant $\gamma_2=\kappa_4/\sigma^4$, its central-region density expansion is

$$
f_{Z_n}(z)=\phi(z)\left[1+\frac{\gamma_1}{6\sqrt n}H_3(z)+\frac1n\left\{\frac{\gamma_2}{24}H_4(z)+\frac{\gamma_1^2}{72}H_6(z)\right\}\right]+o(n^{-1}),
$$

under sufficient moment and smoothness/nonlattice conditions. Here $H_3=z^3-3z$, $H_4=z^4-6z^2+3$, $H_6=z^6-15z^4+45z^2-15$ are probabilists' [Hermite polynomials](../../../../../../hermite-polynomial.md). Expanding the characteristic exponent gives the cubic and quartic terms, while squaring the cubic term in the exponential gives the $H_6$ correction. Integrating the first correction, using $(\phi H_{k-1})'=-\phi H_k$, gives

$$
\boxed{\mathbb P(Z_n\leq z)=\Phi(z)+\frac{\gamma_1}{6\sqrt n}(1-z^2)\phi(z)+O(n^{-1}).}
$$

Thus skewness determines the first departure from the [normal approximation](../../../../../../normal-approximation.md); inversion gives a [Cornish-Fisher expansion](../../../../../../cornish-fisher-expansion.md) for [quantiles](../../../../../../quantile-function.md). These are asymptotic expansions, not guaranteed nonnegative densities in extreme tails. Lattice data require continuity/lattice corrections, and moment assumptions alone do not justify a uniform smooth-density expansion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
