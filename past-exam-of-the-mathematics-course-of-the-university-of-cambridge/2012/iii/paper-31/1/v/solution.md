<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For $1\leq k\leq m$, the [correlation function of a point process](../../../../../../correlation-function-of-a-point-process.md) associated with the [eigenvalues](../../../../../../eigenvalue.md) is

$$
R_k(x_1,\ldots,x_k)=\frac{m!}{(m-k)!}\int_{\mathbb R^{m-k}}f_m(x_1,\ldots,x_m)\,dx_{k+1}\cdots dx_m.
$$

The [factorial](../../../../../../factorial.md) factor counts ordered selections of $k$ distinct [eigenvalues](../../../../../../eigenvalue.md), so this is a [factorial](../../../../../../factorial.md) moment density, rather than the ordinary probability density of $k$ particular labels. Equivalently, for a nonnegative measurable test [function](../../../../../../function-split.md) $F$,

$$
\mathbb E\sum_{i_1,\ldots,i_k\text{ distinct}}F(\lambda_{i_1},\ldots,\lambda_{i_k})=\int_{\mathbb R^k}F(x_1,\ldots,x_k)R_k(x_1,\ldots,x_k)\,d\mathbf x.
$$

Repeated [projection kernel determinant integration](../../../../../../projection-kernel-determinant-integration.md), with $r=m$, gives a factor $(m-k)!$ on integrating an $m$-by-$m$ kernel [determinant](../../../../../../determinant.md) down to size $k$. Together with the normalizing $1/m!$ in $f_m$, the factors cancel:

$$
\boxed{R_k(x_1,\ldots,x_k)=\det[K_m(x_i,x_j)]_{i,j=1}^k.}
$$

In particular $R_1(x)=K_m(x,x)$ and $\int R_k\,d\mathbf x=m!/(m-k)!$. Set $R_0=1$ and $R_k=0$ for $k>m$. The [eigenvalue](../../../../../../eigenvalue.md) configuration is thus a [determinantal point process](../../../../../../determinantal-point-process.md) with a rank-$m$ [finite-rank projection kernel](../../../../../../finite-rank-projection-kernel.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
