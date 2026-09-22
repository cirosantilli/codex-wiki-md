<h1 id="2/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With exact data $f=Ku^\dagger$, the iteration error obeys

$$
u^{(k)}-u^\dagger=-(I+\tau K^*K)^{-k}u^\dagger.
$$

The [source condition for quadratic regularization](../../../../../../../source-condition-for-quadratic-regularization.md) $u^\dagger=K^*v$ excludes any [null space](../../../../../../../kernel-of-a-linear-map.md) component. Using its [singular system of a compact operator](../../../../../../../singular-system-of-a-compact-operator.md) coefficients,

$$
\|u^{(k)}-u^\dagger\|^2
=\sum_j\frac{\sigma_j^2}{(1+\tau\sigma_j^2)^{2k}}
|\langle v,w_j\rangle|^2.
$$

By [Bernoulli's inequality](../../../../../../../bernoulli-s-inequality.md), $(1+\tau\sigma^2)^k\geq1+k\tau\sigma^2$. Also $1+k\tau\sigma^2\geq2\sqrt{k\tau}\,\sigma$. Therefore

$$
\frac{\sigma}{(1+\tau\sigma^2)^k}\leq\frac1{2\sqrt{k\tau}}.
$$

Summing the squared coefficients and using [Bessel inequality](../../../../../../../bessel-s-inequality.md) yields

$$
\boxed{\|u^{(k)}-u^\dagger\|
\leq\frac{\|v\|}{2\sqrt{k\tau}}=O(k^{-1/2}).}
$$

This is an a priori error rate from the [source condition for quadratic regularization](../../../../../../../source-condition-for-quadratic-regularization.md), with constant independent of $k$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
