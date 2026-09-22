<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [holomorphic de Rham complex](../../../../../../holomorphic-de-rham-complex.md) is exact locally, which is the criterion for an [exact sequence of sheaves](../../../../../../exact-sequence-of-sheaves.md). Work in a small star-shaped [holomorphic coordinate](../../../../../../holomorphic-coordinate.md) neighbourhood in $\mathbb C^2$, centred at zero. A [holomorphic function](../../../../../../holomorphic-function.md) has $\partial f=0$ exactly when it is constant on this neighbourhood, giving exactness at $\mathcal O_M$ and the injection of the [constant sheaf](../../../../../../constant-sheaf.md).

For exactness at $\Omega_M^1$, let $\alpha=a_1(z)\,dz_1+a_2(z)\,dz_2$ be holomorphic and $\partial$-closed. Then $\partial a_1/\partial z_2=\partial a_2/\partial z_1$. Define the [holomorphic function](../../../../../../holomorphic-function.md)

$$
F(z)=\int_0^1\bigl(z_1a_1(tz)+z_2a_2(tz)\bigr)\,dt.
$$

Differentiation under the integral and the closedness identity give

$$
\frac{\partial F}{\partial z_j}
=\int_0^1\left(a_j(tz)+t\sum_i z_i\frac{\partial a_j}{\partial z_i}(tz)\right)dt
=[t\,a_j(tz)]_{t=0}^{t=1}=a_j(z).
$$

Thus $\partial F=\alpha$.

For exactness at $\Omega_M^2$, any [holomorphic differential form](../../../../../../holomorphic-differential-form.md) of degree two is $\beta=b(z)\,dz_1\wedge dz_2$ and is automatically $\partial$-closed by dimension. Define

$$
\gamma(z)=\int_0^1 t\,b(tz)(z_1\,dz_2-z_2\,dz_1)\,dt.
$$

Its derivative is

$$
\partial\gamma
=\int_0^1\left(2t\,b(tz)+t^2\sum_i z_i\frac{\partial b}{\partial z_i}(tz)\right)dt\,dz_1\wedge dz_2
=[t^2b(tz)]_0^1\,dz_1\wedge dz_2=\beta.
$$

These local primitives prove the [holomorphic Poincaré lemma](../../../../../../holomorphic-poincare-lemma.md) in the degrees needed here. Exactness on every stalk gives

$$
\boxed{0\longrightarrow\underline{\mathbb C}\longrightarrow\mathcal O_M
\xrightarrow{\partial}\Omega_M^1\xrightarrow{\partial}\Omega_M^2\longrightarrow0.}
$$

This is sheaf exactness; the local primitives need not glue to global ones.

## ↑ Ancestors (11)

1. [B](../b.md)
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
