<h1 id="k/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the [curl](../../../../../curl.md) of the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid-split.md). The [gradient](../../../../../gradient.md) on the right has zero [curl](../../../../../curl.md). Use the stated vector identity with $\mathbf F=\boldsymbol\omega$, $\mathbf G=\mathbf u$:

$$
\partial_t\boldsymbol\omega
+(\mathbf u\cdot\nabla)\boldsymbol\omega
-(\boldsymbol\omega\cdot\nabla)\mathbf u
+\boldsymbol\omega(\nabla\cdot\mathbf u)
-\mathbf u(\nabla\cdot\boldsymbol\omega)=0.
$$

[incompressible flow](../../../../../incompressible-flow.md) gives $\nabla\cdot\mathbf u=0$, while a [curl](../../../../../curl.md) always has zero [divergence](../../../../../divergence.md), so $\nabla\cdot\boldsymbol\omega=0$. The remaining terms give

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}
=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

For a two-dimensional [velocity](../../../../../velocity.md) independent of $z$, $\boldsymbol\omega=(0,0,v_x-u_y)$ and $(\boldsymbol\omega\cdot\nabla)\mathbf u=\omega_z\partial_z\mathbf u=0$. Thus **the scalar [vorticity](../../../../../vorticity-split.md) is conserved following each fluid particle**. It can still vary from particle to particle; this is advection, not a claim of spatially uniform [vorticity](../../../../../vorticity-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [K](../../../k.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
