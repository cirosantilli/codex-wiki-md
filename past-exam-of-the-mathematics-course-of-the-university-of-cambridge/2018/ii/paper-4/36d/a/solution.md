<h1 id="36d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [electric polarization](../../../../../../polarization-density.md) $P$ is electric dipole moment per unit volume. A polarized body acts as the bound volume and [surface charge density](../../../../../../surface-charge-density.md)

$$
\rho_{\rm b}=-\nabla\mathbin{\cdot}P,
\qquad \sigma_{\rm b}=P\mathbin{\cdot}n.
$$

Indeed, summing the [scalar potential](../../../../../../scalar-potential.md) of its dipoles and integrating by parts gives

$$
\phi(x)=\frac1{4\pi\epsilon_0}
\int_V P(x')\mathbin{\cdot}\nabla'\frac1{|x-x'|}\,d^3x'
$$



$$
=\frac1{4\pi\epsilon_0}
\left[
\int_V\frac{-\nabla'\mathbin{\cdot}P(x')}{|x-x'|}\,d^3x'
+\int_S\frac{P(x')\mathbin{\cdot}n}{|x-x'|}\,dS'
\right].
$$

This is exactly the potential of $\rho_{\rm b}$ and $\sigma_{\rm b}$.

For the central free charge, [Gauss's law](../../../../../../gauss-s-law.md) for the [electric displacement field](../../../../../../electric-displacement-field.md) gives

$$
D(r)=\frac{q}{4\pi r^2}\hat r,
\qquad E=\frac D\epsilon,
\qquad P=D-\epsilon_0E
=\left(1-\frac{\epsilon_0}{\epsilon}\right)
\frac{q}{4\pi r^2}\hat r.
$$

Thus on the sphere,

$$
\boxed{\sigma_{\rm b}
=\left(1-\frac{\epsilon_0}{\epsilon}\right)
\frac{q}{4\pi R^2}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [36D](../../36d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
