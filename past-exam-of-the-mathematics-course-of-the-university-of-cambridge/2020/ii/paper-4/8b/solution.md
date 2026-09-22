<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Write the position of a mass element relative to the [center of mass](../../../../../center-of-mass.md) as $\mathbf r$, so its inertial-frame velocity is $\dot{\mathbf X}+\boldsymbol\omega\times\mathbf r$. The center-of-mass identity $\int\mathbf r\,dm=0$ removes all cross terms. Define the [inertia tensor](../../../../../inertia-tensor.md) about the center of mass by

$$
I_{ij}=\int\bigl(r^2\delta_{ij}-r_ir_j\bigr)\,dm.
$$

The total [angular momentum](../../../../../angular-momentum.md) about the origin and [kinetic energy](../../../../../kinetic-energy.md) are then

$$
\mathbf L=M\mathbf X\times\dot{\mathbf X}+I\boldsymbol\omega,
\qquad
T=\frac12M|\dot{\mathbf X}|^2+\frac12\boldsymbol\omega\mathbin{\cdot}I\boldsymbol\omega.
$$

Let $\rho(r)=C r^{-1}\sin(\pi r/R)$. [Spherical symmetry](../../../../../spherical-symmetry.md) makes $I=I_0\mathbf1$. The mass normalization is

$$
M=4\pi C\int_0^R r\sin\frac{\pi r}{R}\,dr=4CR^2,
$$

so $C=M/(4R^2)$. A moment about any diameter is

$$
I_0=\frac{8\pi}{3}\int_0^R\rho(r)r^4\,dr
=\frac{8\pi C}{3}\frac{R^4}{\pi^4}\int_0^\pi x^3\sin x\,dx
=\frac{2MR^2(\pi^2-6)}{3\pi^2}.
$$

Therefore

$$
\boxed{I=\frac{2MR^2(\pi^2-6)}{3\pi^2}\,\mathbf1}.
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
