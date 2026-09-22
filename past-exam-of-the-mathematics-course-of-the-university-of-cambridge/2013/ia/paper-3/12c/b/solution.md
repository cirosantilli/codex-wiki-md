<h1 id="12c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the usual bounded-domain hypotheses, with piecewise smooth boundary and a sufficiently smooth [vector field](../../../../../../vector-field.md), the [divergence theorem](../../../../../../divergence-theorem.md) states

$$
\boxed{\int_\Omega\nabla\cdot\mathbf F\,dV=\int_{\partial\Omega}\mathbf F\cdot\mathbf n\,dS,}
$$

where $\mathbf n$ is outward. Apply it to $g\mathbf F$ and use the [product rule](../../../../../../product-rule.md) $\nabla\cdot(g\mathbf F)=\mathbf F\cdot\nabla g+g\nabla\cdot\mathbf F$ to obtain

$$
\boxed{\int_\Omega(\mathbf F\cdot\nabla g+g\nabla\cdot\mathbf F)\,dV
=\int_{\partial\Omega}g\mathbf F\cdot\mathbf n\,dS.}
$$

For uniqueness, let $w=u_1-u_2$ for two [classical solutions](../../../../../../classical-solution.md) with the same [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md). Then $\Delta w=0$ and $w=0$ on the boundary. Taking $\mathbf F=\nabla w$, $g=w$ gives [Green's first identity](../../../../../../green-s-first-identity.md) in the form

$$
\int_\Omega|\nabla w|^2\,dV
=\int_{\partial\Omega}w\partial_nw\,dS-\int_\Omega w\Delta w\,dV=0.
$$

The continuous nonnegative integrand must vanish, so $w$ is constant on each connected component. The zero boundary data make every such constant zero. Thus **the solution of the [Dirichlet problem](../../../../../../dirichlet-problem.md) for the [Laplace equation](../../../../../../laplace-equation.md) is unique, if it exists**. This establishes [Uniqueness of the Dirichlet problem](../../../../../../uniqueness-of-the-dirichlet-problem.md); existence is assumed. Boundedness, or suitable conditions at infinity, is needed: on an unbounded half-space the [harmonic function](../../../../../../harmonic-function.md) $w=z$ has zero boundary values but is not identically zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
