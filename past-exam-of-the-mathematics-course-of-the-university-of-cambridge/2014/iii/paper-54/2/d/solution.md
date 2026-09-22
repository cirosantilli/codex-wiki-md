<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Integrate [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) through a narrow slab around the disk. The horizontal derivative contributions vanish as its thickness tends to zero, leaving the normal-derivative jump

$$
\partial_z\Phi(0^+)-\partial_z\Phi(0^-)=4\pi G\Sigma.
$$

The [even function](../../../../../../even-function.md) symmetry of $\Phi$ makes the derivatives opposite, so

$$
\boxed{\partial_z\Phi(0^+)=2\pi G\Sigma.}
$$

In the current-free simply connected upper half-space, [Ampère's circuital law](../../../../../../ampere-s-circuital-law.md) gives $\nabla\times\mathbf B=0$ and permits a [magnetic scalar potential](../../../../../../magnetic-scalar-potential.md). Rescale it so that $\sqrt{4\pi G/\mu_0}\,\mathbf B=-\nabla\Phi_M$. The [divergence](../../../../../../divergence.md)-free condition makes $\Phi_M$ satisfy [Laplace's equation](../../../../../../laplace-equation.md), with

$$
\partial_z\Phi_M(0^+)=-\sqrt{\frac{4\pi G}{\mu_0}}B_{z0}.
$$

Compare with the gravitational jump condition. Subject to the same isolated-field boundary condition at infinity, $\Phi_M$ is the harmonic potential of the effective [surface density](../../../../../../surface-density-of-a-disk.md)

$$
\boxed{\Sigma_M=-\frac{B_{z0}}{\sqrt{\pi G\mu_0}}.}
$$

This [gravity-equivalent magnetic surface density](../../../../../../gravity-equivalent-magnetic-surface-density.md) can have either sign; it is a mathematical representation of the exterior [magnetic field](../../../../../../magnetic-field.md), not physical negative mass. An imposed nondecaying field would require additional boundary data and would not be fixed by the disk [surface density](../../../../../../surface-density-of-a-disk.md) alone.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
