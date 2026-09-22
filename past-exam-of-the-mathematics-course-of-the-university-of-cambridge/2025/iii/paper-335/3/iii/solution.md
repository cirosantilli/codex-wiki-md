<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write

$$
B=I-\frac1\alpha A^*A.
$$

The stated iteration is $x_{n+1}=Bx_n+\alpha^{-1}A^*y$, so repeated substitution and the [geometric series](../../../../../../geometric-series.md) identity give

$$
x_n=B^nx_0+\frac1\alpha\sum_{j=0}^{n-1}B^jA^*y.
$$

For the singular component $v_i$, put $r_i=1-\sigma_i^2/\alpha$. Since the initial Tikhonov solution has coefficient $\sigma_i(y,u_i)/(\sigma_i^2+\alpha)$, one obtains

$$
x_n=\sum_{i=1}^\infty
\left[
r_i^n\frac{\sigma_i}{\sigma_i^2+\alpha}
+\frac{1-r_i^n}{\sigma_i}
\right](y,u_i)v_i.
$$

Therefore the requested spectral filter is

$$
\boxed{
g_{\alpha,n}(\sigma)
=\frac1\sigma\left[
1-\frac{\alpha}{\sigma^2+\alpha}
\left(1-\frac{\sigma^2}{\alpha}\right)^n
\right].}
$$

**Thus equation (3) reads $x_n=\sum_i g_{\alpha,n}(\sigma_i)(y,u_i)v_i$. Convergence of this stationary iteration requires $|1-\sigma_i^2/\alpha|<1$ on the nonzero spectrum, for example $\alpha>\|A\|^2/2$.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
