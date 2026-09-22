<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The canonical [Dirichlet Green function](../../../../../../dirichlet-green-function.md) on the [unit disc](../../../../../../unit-disc.md) with its pole at zero is $-\log|w|$. Conformal invariance of the planar Green kernel therefore gives

$$
G_D(z,\phi(w))=-\log|w|.
$$

Comparing with $G_D(z,y)=-\log|z-y|-G_z(y)$ yields

$$
G_z(\phi(w))=-\log|\phi(w)-\phi(0)|+\log|w|=-\psi(w).
$$

This also explains the boundary data: when $|w|=1$, the correction is $-\log|\phi(w)-z|$. The composition with $\phi^{-1}$ is harmonic by [conformal invariance of harmonicity](../../../../../../conformal-invariance-of-harmonicity.md). Its apparent singularity at $z$ is removable because the quotient defining $\psi$ extends to $\phi'(0)$.

Evaluating there proves the [regular part of the planar Dirichlet Green function](../../../../../../regular-part-of-the-planar-dirichlet-green-function.md) formula

$$
\boxed{G_z(y)=-\psi(\phi^{-1}(y)),\qquad G_z(z)=-\log|\phi'(0)|=-\log\operatorname{crad}_D(z).}
$$

On an unbounded domain, boundary values alone need not specify a unique [harmonic function](../../../../../../harmonic-function.md). Here $G_z$ is the correction belonging to the canonical Dirichlet Green kernel, which fixes that ambiguity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
