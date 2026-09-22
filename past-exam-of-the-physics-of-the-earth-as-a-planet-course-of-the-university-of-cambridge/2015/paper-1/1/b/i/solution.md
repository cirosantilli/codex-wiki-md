<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume a stable, lossless elastic body with the usual symmetry of the [elasticity tensor](../../../../../../elasticity-tensor.md) and [boundary conditions](../../../../../../boundary-condition.md) that eliminate the surface terms in [integration by parts](../../../../../../integration-by-parts.md), such as a traction-free outer surface. Its elastic stiffness operator is then self-adjoint. When [density](../../../../../../density.md) varies spatially, the precise eigenproblem is generalized:

$$
\hat H\mathbf u_\alpha=\rho\omega_\alpha^2\mathbf u_\alpha,
\qquad
\langle\mathbf u_\alpha,\mathbf u_\beta\rangle_\rho
=\int_\Omega\rho\,\mathbf u_\alpha^*\cdot\mathbf u_\beta\,dV
=\delta_{\alpha\beta}.
$$

Here $\alpha$ abbreviates the pair of mode labels. Equivalently, $\rho^{-1}\hat H$ is a [self-adjoint operator](../../../../../../self-adjoint-operator.md) in the mass [inner product](../../../../../../inner-product-split.md). Stability makes $\omega_\alpha^2$ real and nonnegative. Modes at different [eigenvalues](../../../../../../eigenvalue.md) are orthogonal, and an [orthonormal basis](../../../../../../orthonormal-basis.md) can be selected within each degenerate eigenspace. Completeness permits expansion of a suitable [displacement field](../../../../../../displacement-field-mechanics.md) in these [mass-weighted elastic normal modes](../../../../../../mass-weighted-elastic-normal-modes.md).

Insert the expansion and project onto $\mathbf u_\alpha^*$. Mass normalization diagonalizes both the [acceleration](../../../../../../acceleration.md) term and the restoring term. For a symmetric [stress glut tensor](../../../../../../stress-glut-tensor.md) supported away from the boundary,

$$
\int_\Omega\mathbf u_\alpha^*\cdot(-\nabla\cdot\boldsymbol\Gamma)\,dV
=\int_\Omega\boldsymbol\Gamma:\nabla\mathbf u_\alpha^*\,dV
=\int_\Omega\boldsymbol\Gamma:\mathbf e_\alpha^*\,dV.
$$

The symmetry of the [stress glut tensor](../../../../../../stress-glut-tensor.md) removes the antisymmetric part of the displacement gradient, leaving the [strain](../../../../../../strain.md). The result is **one independent forced oscillator per mode**, with the stated excitation integral. If the modes instead have mass norm $N_\alpha$, that integral is divided by $N_\alpha$. A source touching the boundary requires the corresponding surface forcing to be retained rather than silently dropping it.

Rigid translations and rotations can be zero-frequency modes of a free body. Their [strain](../../../../../../strain.md) vanishes, so an internal symmetric [seismic moment tensor](../../../../../../seismic-moment-tensor.md) does not excite them through this coupling. Attenuation, radiative boundaries or other non-self-adjoint effects require modifications of the simple conservative expansion.

## ↑ Ancestors (15)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the physics of the Earth as a Planet course of the University of Cambridge](../../../../../split.md)
7. [Physics of the Earth as a Planet course of the University of Cambridge](../../../../../../physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
