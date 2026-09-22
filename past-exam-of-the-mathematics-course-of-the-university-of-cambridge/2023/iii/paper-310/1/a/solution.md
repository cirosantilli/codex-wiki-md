<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a component with the [barotropic equation of state](../../../../../../barotropic-equation-of-state.md) $P=w\rho$, the [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) is

$$
\dot\rho+3H(1+w)\rho=0.
$$

Using $H=\dot a/a$ makes this a [separable differential equation](../../../../../../separable-differential-equation.md):

$$
\frac{d\rho}{\rho}=-3(1+w)\frac{da}{a}.
$$

Taking $a_0=1$ gives the [constant-equation-of-state density scaling](../../../../../../constant-equation-of-state-density-scaling.md)

$$
\boxed{\rho(a)=\rho_0a^{-3(1+w)}
=\rho_0(1+z)^{3(1+w)}}.
$$

The spatially flat [Friedmann equation](../../../../../../friedmann-equations.md) and the [cosmological density parameters](../../../../../../cosmological-density-parameter.md) therefore give

$$
\boxed{H(z)=H_0E(z)},
\qquad
E(z)=\left[\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}\right]^{1/2}.
$$

Along a radial light ray, $d\chi=dt/a$. Since the [redshift-time relation](../../../../../../redshift-time-relation.md) is $dt=-dz/[(1+z)H]$ and $a=(1+z)^{-1}$,

$$
d\chi=-\frac{dz}{H(z)}.
$$

Hence the [comoving radial distance](../../../../../../comoving-radial-distance.md) is

$$
\boxed{\chi(z)=\frac1{H_0}\int_0^z
\frac{dz'}{\left[\sum_i\Omega_{i,0}(1+z')^{3(1+w_i)}\right]^{1/2}}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
