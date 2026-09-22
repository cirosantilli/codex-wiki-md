<h1 id="12b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with real-valued smooth functions on the bounded region enclosed by $S$, with the [oriented surface element](../../../../../../oriented-surface-element.md) pointing outward. Set $\psi=\phi-\phi_1$. It is a [harmonic function](../../../../../../harmonic-function.md) in $V$ and has zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) on $S$. Applying [Green's first identity](../../../../../../green-s-first-identity.md) to $\psi$ with itself gives

$$
\int_V|\nabla\psi|^2\,dV
=\int_S\psi\,\partial_n\psi\,dS-\int_V\psi\Delta\psi\,dV=0.
$$

Both terms on the right vanish by the boundary condition and harmonicity. The integrand is nonnegative and continuous, so $\nabla\psi=0$ throughout $V$. Consequently $\psi$ is constant on each [connected component](../../../../../../connected-component.md); every bounded component meets the prescribed boundary, where that constant is zero. Therefore

$$
\boxed{\phi_1=\phi\text{ throughout }V.}
$$

This is the energy proof of [Uniqueness of the Dirichlet problem](../../../../../../uniqueness-of-the-dirichlet-problem.md). Connectedness of $V$ is not essential if the boundary values are prescribed on every component. Boundedness, or suitable decay and integrability at infinity, is needed for the boundary/energy argument; the finite enclosed-volume interpretation is used here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
