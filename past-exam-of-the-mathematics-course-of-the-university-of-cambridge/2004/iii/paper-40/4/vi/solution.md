<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

[Antithetic variates](../../../../../../antithetic-variates.md) preserve each draw's marginal law but couple two estimates negatively. For an average of identically distributed $H,H'$,

$$
\operatorname{Var}\left(\frac{H+H'}2\right)
=\frac12\left(\operatorname{Var}(H)+\operatorname{Cov}(H,H')\right).
$$

Negative [covariance](../../../../../../covariance.md) improves on two [independent](../../../../../../independent-random-variables.md) evaluations at the same computational budget.

Here generate [independent](../../../../../../independent-random-variables.md) $U_1,\ldots,U_r\sim U(0,1)$ and pair $x_j=kU_j$ with $x_j'=k(1-U_j)$. Both are uniform on $[0,k]$. The [antithetic Cauchy-tail integration on a finite interval](../../../../../../antithetic-cauchy-tail-integration-on-a-finite-interval.md) estimator is

$$
\boxed{\widehat\mu_A=\frac12-\frac{k}{2r}\sum_{j=1}^r
\left[f(kU_j)+f(k(1-U_j))\right].}
$$

It is unbiased. Put $h(u)=f(ku)$. This decreases, whereas $h(1-u)$ increases. For an [independent](../../../../../../independent-random-variables.md) copy $U'$ of $U$, the [covariance](../../../../../../covariance.md) identity gives

$$
\operatorname{Cov}(h(U),h(1-U))
=\frac12\mathbb E[(h(U)-h(U'))(h(1-U)-h(1-U'))]\leq0.
$$

Each product is nonpositive, and for $k>0$ it is strictly negative off the diagonal. Therefore

$$
\operatorname{Var}(\widehat\mu_A)
=\frac{k^2}{2r}\left[\operatorname{Var}(h(U))+
\operatorname{Cov}(h(U),h(1-U))\right]
<\frac{k^2}{2r}\operatorname{Var}(h(U)),
$$

which is the [variance](../../../../../../variance-split.md) using $2r$ [independent](../../../../../../independent-random-variables.md) evaluations in part (v). Thus the comparison accounts for the doubled number of [probability density function](../../../../../../probability-density-function.md) evaluations in each pair.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
