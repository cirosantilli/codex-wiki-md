<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a fixed environment, use two [independent](../../../../../../independent-random-variables.md) copies of the walk to express $Z_t^2=\langle\kappa_t^{(1)}\kappa_t^{(2)}\rangle$. The product is finite and nonnegative, so we can interchange the two expectations. At each time $j$, if the walks occupy different sites, the two environment signs are [independent](../../../../../../independent-random-variables.md) and their factors have product expectation $1$. If they coincide, both factors use the same sign and

$$
\mathbb E(1+\varepsilon h)^2=1+\varepsilon^2.
$$

Different time layers are [independent](../../../../../../independent-random-variables.md) even when a site is visited again. Therefore, with the simultaneous collision count $I_t=\sum_{j=1}^t\mathbf1_{\{\xi_j^{(1)}=\xi_j^{(2)}\}}$,

$$
\boxed{\mathbb EZ_t^2=\left\langle(1+\varepsilon^2)^{I_t}\right\rangle.}
$$

This is the [collision-count second moment for independent path weights](../../../../../../collision-count-second-moment-for-independent-path-weights.md). It involves equal-time intersections, not arbitrary intersections of the two spatial ranges.

The difference walk $D_j=\xi_j^{(1)}-\xi_j^{(2)}$ has [independent](../../../../../../independent-random-variables.md) bounded increments symmetric about zero and a full-dimensional step distribution. It may hold at zero for one step; such a hold counts as a positive-time return. The allowed transience fact gives

$$
\rho=\mathbb P_0(D_j=0\text{ for some }j\ge1)<1.
$$

Moreover $\rho>0$ since the two first steps can be equal. Restarting the [independent increments](../../../../../../independent-increments.md) after every return to zero shows that the total positive-time return count $I_\infty$ has the zero-based [geometric distribution](../../../../../../geometric-distribution.md)

$$
\mathbb P(I_\infty=k)=(1-\rho)\rho^k,\quad k=0,1,2,\ldots.
$$

Indeed the probability of at least $k$ returns is $\rho^k$, and subtracting successive tails gives this law. Consequently, whenever $\rho(1+\varepsilon^2)<1$,

$$
\sup_t\mathbb EZ_t^2\le\left\langle(1+\varepsilon^2)^{I_\infty}\right\rangle
=\sum_{k=0}^\infty(1-\rho)[\rho(1+\varepsilon^2)]^k
=\frac{1-\rho}{1-\rho(1+\varepsilon^2)}<\infty.
$$

A sufficient small-noise condition is $0<\varepsilon<\min(1,\sqrt{(1-\rho)/\rho})$.

The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) now gives $Z_t\to\zeta$ in $L^2$ as well as almost surely. One can see the [mean](../../../../../../expected-value.md) preservation directly: for $t\ge s$, the [martingale](../../../../../../martingale-split.md) identity gives $\mathbb E(Z_t-Z_s)^2=\mathbb EZ_t^2-\mathbb EZ_s^2$. The [second moments](../../../../../../second-moment.md) are increasing and bounded, so the sequence is Cauchy in $L^2$ and its limit is the already identified almost-sure limit. Thus

$$
\boxed{\mathbb E\zeta=\lim_t\mathbb EZ_t=1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
