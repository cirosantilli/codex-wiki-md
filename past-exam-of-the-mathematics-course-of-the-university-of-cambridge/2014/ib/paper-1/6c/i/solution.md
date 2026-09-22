<h1 id="6c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Insert an exact smooth solution into the [linear multistep method](../../../../../../linear-multistep-method.md) and define its unscaled [local truncation error](../../../../../../local-truncation-error.md) by

$$
\mathcal R_h[y]=\sum_{\ell=0}^s\rho_\ell y(t+\ell h)-h\sum_{\ell=0}^s\sigma_\ell y'(t+\ell h).
$$

Its [Taylor expansion](../../../../../../taylor-expansion.md) has coefficients

$$
\mathcal R_h[y]=c_0y(t)+\sum_{j\geq1}c_jh^jy^{(j)}(t),\qquad
c_0=\sum_\ell\rho_\ell,\quad c_j=\frac1{j!}\sum_\ell\ell^j\rho_\ell-\frac1{(j-1)!}\sum_\ell\ell^{j-1}\sigma_\ell.
$$

The method has order at least $p$ exactly when $c_0=\cdots=c_p=0$, since then $\mathcal R_h[y]=O(h^{p+1})$ for every sufficiently smooth $y$. Necessity can be checked by inserting polynomials of successive degrees. This also corresponds to the usual truncation error $\mathcal R_h/h=O(h^p)$.

On the other hand, expansion of the [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) gives

$$
\rho(e^z)-z\sigma(e^z)=c_0+c_1z+c_2z^2+\cdots.
$$

Thus the [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) is

$$
\boxed{\rho(e^z)-z\sigma(e^z)=O(z^{p+1})\ \Longleftrightarrow\ \text{order at least }p.}
$$

If “order $p$” is meant to be the exact rather than guaranteed order, one additionally requires $c_{p+1}\ne0$. The first two vanishing conditions are the usual [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) relations $\rho(1)=0$, $\rho'(1)=\sigma(1)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
