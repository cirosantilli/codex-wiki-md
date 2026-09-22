<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For degree zero, [compactness](../../../../../../compact-space.md) and the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) make [holomorphic functions](../../../../../../holomorphic-function.md) constant on each [connected component](../../../../../../connected-component.md). For degree two, a [holomorphic differential form](../../../../../../holomorphic-differential-form.md) is $\bar\partial$-closed and its $\partial$ derivative has type $(3,0)$, which vanishes on a complex surface. Degrees above two have no nonzero holomorphic forms. It remains to treat a [holomorphic differential form](../../../../../../holomorphic-differential-form.md) $\alpha$ of degree one.

Set $\beta=d\alpha=\partial\alpha$. Its coefficients are holomorphic, so $\beta$ is a [holomorphic differential form](../../../../../../holomorphic-differential-form.md) of degree two, hence closed by the degree-two observation. Its conjugate is closed too. The [Stokes theorem](../../../../../../stokes-theorem.md) gives

$$
\int_M\beta\wedge\bar\beta
=\int_Md(\alpha\wedge\bar\beta)=0.
$$

The integrand is nonnegative in the complex orientation. In local coordinates, if $\beta=b(z)\,dz_1\wedge dz_2$ with $z_j=x_j+iy_j$, then

$$
\beta\wedge\bar\beta
=4|b(z)|^2\,dx_1\wedge dy_1\wedge dx_2\wedge dy_2.
$$

It is strictly positive wherever $\beta$ is nonzero. Its zero integral therefore forces $\beta=0$ everywhere. Thus [holomorphic forms on a compact complex surface are closed](../../../../../../holomorphic-forms-on-a-compact-complex-surface-are-closed.md), even when the surface is not Kähler:

$$
\boxed{d\alpha=0\quad\text{for every global holomorphic }p\text{-form}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
