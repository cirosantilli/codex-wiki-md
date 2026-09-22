<h1 id="16b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The orbital [angular momentum operators](../../../../../../angular-momentum-operator.md) are

$$
\boxed{\hat L_i=\sum_{j,k}\varepsilon_{ijk}\hat x_j\hat p_k=-i\hbar\sum_{j,k}\varepsilon_{ijk}x_j\partial_k,\qquad \hat L^2=\sum_{i=1}^3\hat L_i^2.}
$$

In particular $\hat L_3=-i\hbar(x_1\partial_2-x_2\partial_1)$. For smooth compactly supported functions $\phi,\psi$, integration by parts produces no boundary term, and $\partial_2x_1=\partial_1x_2=0$. Hence

$$
\langle\phi,\hat L_3\psi\rangle=\langle\hat L_3\phi,\psi\rangle.
$$

This proves Hermiticity on the common test-function domain, and the same calculation applies on suitable decaying domains. As an unbounded operator, it is not defined on every $L^2$ function: the usual [self-adjoint operator](../../../../../../self-adjoint-operator.md) realization is the generator of unitary rotations about the third axis. Thus the integration statement includes its necessary domain/boundary assumptions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
