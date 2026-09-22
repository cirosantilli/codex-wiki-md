<h1 id="11a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the usual [Dirichlet problem](../../../../../../dirichlet-problem.md) on a bounded regular volume, suppose $\phi_1,\phi_2$ both satisfy the stated data. Their difference $u=\phi_1-\phi_2$ is a [harmonic function](../../../../../../harmonic-function.md), with $\nabla^2u=0$ in $V$ and $u=0$ on $\partial V$. In [Green's first identity](../../../../../../green-s-first-identity.md), choose both functions equal to $u$:

$$
\int_V|\nabla u|^2\,dV=\int_{\partial V}u\frac{\partial u}{\partial n}\,dS=0.
$$

The nonnegative continuous integrand forces $\nabla u=0$. Thus $u$ is constant on each connected component, and its zero boundary values force each constant to vanish. This proves **uniqueness** for the [Dirichlet problem](../../../../../../dirichlet-problem.md).

If the boundary value is a constant $c$, the constant function $c$ is itself a [harmonic function](../../../../../../harmonic-function.md) with those data. Uniqueness therefore yields

$$
\boxed{\phi\equiv c\text{ throughout }V.}
$$

Boundedness, or an appropriate condition at infinity replacing it, is essential. On the upper half-space both $u=0$ and $u=z$ are [harmonic functions](../../../../../../harmonic-function.md) with zero data on its boundary plane. They show why unrestricted uniqueness must not be asserted for an unbounded volume.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
