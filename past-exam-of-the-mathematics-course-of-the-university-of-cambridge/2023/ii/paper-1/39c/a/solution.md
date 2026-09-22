<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The steady incompressible [Stokes flow](../../../../../../stokes-flow-split.md) equations are

$$
-\nabla p+\mu\nabla^2\mathbf u=0,
\qquad
\nabla\mathbin{\cdot}\mathbf u=0.
$$

Taking the [curl](../../../../../../curl.md) eliminates the pressure gradient and commutes with the Laplacian, so for the [vorticity](../../../../../../vorticity.md) $\boldsymbol\omega=\nabla\times\mathbf u$,

$$
\boxed{\nabla^2\boldsymbol\omega=0}.
$$

This is the vorticity part of [Harmonic pressure and vorticity in Stokes flow](../../../../../../harmonic-pressure-and-vorticity-in-stokes-flow.md).

For a two-dimensional incompressible flow, choose the [stream function](../../../../../../stream-function.md) convention

$$
u_x=\psi_y,
\qquad
u_y=-\psi_x.
$$

Then

$$
\omega_z=\partial_xu_y-\partial_yu_x=-\nabla^2\psi.
$$

Applying the harmonic-vorticity equation gives

$$
\boxed{\nabla^4\psi=0},
$$

the [Biharmonic stream function for planar Stokes flow](../../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
