<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Suppose $\phi_1,\phi_2$ are two sufficiently regular solutions with the same [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), and put $w=\phi_1-\phi_2$. Then $\Delta w=0$ in $V$ and $w=0$ on its boundary. Apply the [divergence theorem](../../../../../divergence-theorem.md) to $w\nabla w$:

$$
\int_V\bigl(|\nabla w|^2+w\Delta w\bigr)\,dV=\int_S w\,\partial_nw\,dS=0.
$$

Thus $\nabla w=0$ throughout $V$, so $w$ is constant on each connected component. Its zero boundary values force every such constant to be zero. This proves **uniqueness of the Dirichlet solution**, without assuming its existence.

For a prescribed [Neumann boundary condition](../../../../../neumann-boundary-condition.md), the difference instead has $\partial_nw=0$. The same energy argument still gives $\nabla w=0$, but does not fix the constant. Consequently **the solution is unique up to an additive constant on each connected component**. A value at one point, or the integral mean, fixes the constant on a connected region. There is also a necessary compatibility condition: if $g=\partial_n\phi$ on $S$, the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\boxed{\int_S g\,dS=\int_V\Delta\phi\,dV=0}.
$$

It is required on each component if the region is disconnected. Data failing this condition admit no harmonic solution. This is the homogeneous-source instance of the [Neumann Poisson problem](../../../../../neumann-poisson-problem.md).

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
