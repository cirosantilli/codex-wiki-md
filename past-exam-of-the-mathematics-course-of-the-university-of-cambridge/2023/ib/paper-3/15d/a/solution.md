<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [magnetic field](../../../../../../magnetic-field.md) is $B=\nabla\times A$. The magnetostatic [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) is $\nabla\times B=\mu_0J$, so the [curl of the curl identity](../../../../../../curl-of-the-curl-identity.md) gives

$$
\nabla(\nabla\cdot A)-\nabla^2A=\mu_0J.
$$

A [gauge transformation](../../../../../../gauge-transformation.md) $A\mapsto A+\nabla\chi$ does not change $B$. We may therefore choose the [Coulomb gauge](../../../../../../coulomb-gauge.md) $\nabla\cdot A=0$ by solving the [Poisson equation](../../../../../../poisson-equation.md) $\nabla^2\chi=-\nabla\cdot A$. It follows component by component in a [Cartesian coordinate system](../../../../../../cartesian-coordinate-system.md) that

$$
\boxed{\nabla^2A=-\mu_0J}.
$$

The free-space [Green function](../../../../../../green-s-function.md) of the [Laplacian](../../../../../../laplacian.md) then gives

$$
\boxed{A(r)=\frac{\mu_0}{4\pi}\int_{\mathbb R^3}
\frac{J(r')}{|r-r'|}\,d^3r'}.
$$

For a localized steady [current density](../../../../../../current-density.md), [conservation of electric charge](../../../../../../charge-conservation.md) gives $\nabla'\cdot J=0$; [integration by parts](../../../../../../integration-by-parts.md) confirms directly that this integral has zero [divergence](../../../../../../divergence.md) and hence obeys the Coulomb gauge.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
