<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
c=\frac N{|m|},
\qquad
D=\frac{\omega^2}{c^2}-k^2.
$$

Solving zonal momentum and incompressibility for $\hat u$ and $\hat\phi$ in terms of $\hat v$ gives

$$
\boxed{
\hat u
=\frac{i}{D}
\left(\frac{\beta y\omega}{c^2}\hat v
-k\hat v_y\right)},
$$



$$
\boxed{
\hat\phi
=\frac{i}{D}
\left(k\beta y\hat v-\omega\hat v_y\right)}.
$$

Substitution into meridional geostrophic balance cancels the terms involving $D$ and yields

$$
\boxed{
\hat v_{yy}-\frac{\beta^2y^2m^2}{N^2}\hat v
=\frac{k\beta}{\omega}\hat v}.
$$

Set

$$
\xi=\sqrt{\frac{\beta|m|}{N}}\,y.
$$

The equation becomes

$$
\hat v_{\xi\xi}-\xi^2\hat v
=\frac{kN}{\omega|m|}\hat v.
$$

Using the [Hermite polynomial](../../../../../../hermite-polynomial.md) eigenvalues gives

$$
\boxed{
\omega_n=-\frac{Nk}{(2n+1)|m|}},
\qquad n=1,2,\ldots,
$$

and

$$
\boxed{
\hat v_n(y)=V_n
H_n(\xi)e^{-\xi^2/2}}.
$$

The associated pressure amplitude is

$$
\boxed{
\hat\phi_n
=\frac{i(k\beta y\hat v_n-\omega_n\hat v_{n,y})}
{\omega_n^2m^2/N^2-k^2}}.
$$

For $n=0$, the denominator used to solve for $\hat u$ and $\hat\phi$ vanishes because $\omega_0^2m^2/N^2=k^2$. The inversion therefore assumed precisely the condition that excludes that degenerate case; it must be analyzed separately and is not a member of this [equatorial Rossby wave](../../../../../../equatorial-rossby-wave.md) family.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
