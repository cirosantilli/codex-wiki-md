<h1 id="17d/solution">Solution</h1>

↑ **Parent:** [17D](../17d.md)

For a steady inviscid incompressible fluid of constant density in uniform gravity $\mathbf g=-g\mathbf e_z$, the [Euler equation for fluid motion](../../../../../euler-equations-for-an-inviscid-fluid.md) and continuity equation are

$$
\rho(\mathbf u\cdot\nabla)\mathbf u=-\nabla p+\rho\mathbf g,\qquad \nabla\cdot\mathbf u=0.
$$

Taking the scalar product with $\mathbf u$ gives

$$
(\mathbf u\cdot\nabla)\left(\frac12|\mathbf u|^2+\frac p\rho+gz\right)=0.
$$

Thus **Bernoulli's quantity is constant along each streamline**. For an irrotational connected flow it is constant throughout the flow; constancy across different [streamlines](../../../../../streamline.md) is not assumed in general.

Since incompressibility makes $\nabla\cdot(\rho\mathbf u\otimes\mathbf u)=\rho(\mathbf u\cdot\nabla)\mathbf u$, integrating over a fixed control volume and applying the [divergence theorem](../../../../../divergence-theorem.md) yields the integral momentum balance

$$
\boxed{\int_S\rho\mathbf u(\mathbf u\cdot\mathbf n)\,dS
=-\int_Sp\mathbf n\,dS+\int_V\rho\mathbf g\,dV.}
$$

Here $\mathbf n$ is outward and the left side is the net outgoing [momentum flux](../../../../../momentum-flux.md). Uniform atmospheric [pressure](../../../../../pressure.md) has zero resultant on a closed control surface, so it may be subtracted from all pressures in the jet calculations.

## ↑ Ancestors (10)

1. [17D](../17d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
