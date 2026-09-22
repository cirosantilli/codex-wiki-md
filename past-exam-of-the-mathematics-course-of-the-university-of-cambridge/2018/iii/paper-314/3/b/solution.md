<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [poloidal magnetic flux function](../../../../../../poloidal-magnetic-flux-function.md) convention $\mathbf B_p=R^{-1}\nabla\Psi\times\mathbf e_\phi$, so $2\pi\Psi$ is magnetic flux up to a reference constant. Its [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md) components are

$$
\boxed{B_R=-\frac1R\frac{\partial\Psi}{\partial z},\qquad B_z=\frac1R\frac{\partial\Psi}{\partial R}.}
$$

The prescribed surface flux therefore gives

$$
B_z(R,0)=\frac{\delta\Psi_0}{R_0^\delta}R^{\delta-2},\qquad B_R(R,0)=B_z(R,0)\tan\alpha.
$$

The constant offset $\Psi_1$ does not affect either field component. If instead $\Psi$ denotes the full physical flux rather than flux divided by $2\pi$, both component formulas acquire a common $1/(2\pi)$ factor; the subsequent logarithmic derivative relation is unchanged.

The [Gauss's law for magnetism](../../../../../../gauss-s-law-for-magnetism.md) constraint is $R^{-1}\partial_R(RB_R)+\partial_zB_z=0$. Since $\alpha$ is constant with radius on the surface, it gives the [power-law poloidal field near a disk surface](../../../../../../power-law-poloidal-field-near-a-disk-surface.md) relation

$$
\boxed{\left.\frac{\partial B_z}{\partial z}\right|_{0}=-\frac{\delta(\delta-1)\Psi_0\tan\alpha}{R_0^\delta}R^{\delta-3}=-\frac{\delta-1}{R}B_z(R,0)\tan\alpha.}
$$

For a smooth one-sided field above the surface, $B_z(R,z)=B_z(R,0)[1-(\delta-1)\tan\alpha\,z/R]+O(z^2)$. Thus the field initially decreases with height if $\delta>1$, increases if $0<\delta<1$, and has zero first height derivative if $\delta=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
