<h1 id="16c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the curl of the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md). The pressure term disappears, curl commutes with the Laplacian, and the incompressible vector identity

$$
\nabla\times((\mathbf u\cdot\nabla)\mathbf u)
=(\mathbf u\cdot\nabla)\boldsymbol\omega
-(\boldsymbol\omega\cdot\nabla)\mathbf u
$$

gives

$$
\frac{\partial\boldsymbol\omega}{\partial t}
 +(\mathbf u\cdot\nabla)\boldsymbol\omega
=(\boldsymbol\omega\cdot\nabla)\mathbf u
 +\nu\nabla^2\boldsymbol\omega.
$$

Therefore the [material derivative](../../../../../../material-derivative.md) form is

$$
\boxed{
\frac{D\boldsymbol\omega}{Dt}
=(\boldsymbol\omega\cdot\nabla)\mathbf u
+\nu\nabla^2\boldsymbol\omega}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16C](../../16c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
