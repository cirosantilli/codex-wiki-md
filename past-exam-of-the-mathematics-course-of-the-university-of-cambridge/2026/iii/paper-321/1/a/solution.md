<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [surface density of a disk](../../../../../../surface-density-of-a-disk.md) and outward radial mass flux by

$$
\Sigma=\int_{-\infty}^{\infty}\rho\,dz,
\qquad
\mathcal F=2\pi r\int_{-\infty}^{\infty}\rho u_r\,dz.
$$

Vertical integration of mass conservation eliminates the surface term because $\rho u_z\to0$, and axisymmetry eliminates the azimuthal derivative. Hence

$$
\boxed{\partial_t\Sigma+\frac1{2\pi r}\partial_r\mathcal F=0}.
$$

For $u_\phi\simeq r\Omega(r)$, the [specific angular momentum](../../../../../../specific-angular-momentum.md) is $h=ru_\phi=r^2\Omega$. Multiply the azimuthal momentum equation by $r$, integrate vertically and azimuthally, and define the [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md)

$$
\boxed{\mathcal G=-2\pi r^2\int_{-\infty}^{\infty}\Pi_{r\phi}\,dz}.
$$

Subtracting $h$ times the mass equation from the integrated angular-momentum equation gives

$$
\boxed{\mathcal F\frac{dh}{dr}+\frac{d\mathcal G}{dr}=0}.
$$

For an axisymmetric circular flow, $\Pi_{r\phi}=\mu r\,d\Omega/dr$. If

$$
\bar\nu\Sigma=\int_{-\infty}^{\infty}\mu\,dz,
$$

then

$$
\boxed{\mathcal G=-2\pi\bar\nu\Sigma r^3\frac{d\Omega}{dr}}.
$$

Combining the two conservation laws gives

$$
\boxed{\partial_t(2\pi r\Sigma h)
+\partial_r(\mathcal Fh+\mathcal G)=0}.
$$

The first term is the local rate of change of angular momentum per radial interval, $\mathcal Fh$ is outward advective angular-momentum flux, and $\mathcal G$ is outward stress-carried angular-momentum flux.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
