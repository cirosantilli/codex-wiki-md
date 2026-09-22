<h1 id="8e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [real spectral theorem](../../../../../../real-spectral-theorem.md), the real [symmetric matrix](../../../../../../symmetric-matrix.md) $A$ has an orthonormal basis of [eigenvectors](../../../../../../eigenvector.md). In that basis the associated [quadratic form](../../../../../../quadratic-form.md) is

$$
q(x)=\lambda_1x_1^2+\cdots+\lambda_nx_n^2.
$$

Rescaling the coordinates belonging to nonzero [eigenvalues](../../../../../../eigenvalue.md) changes every positive coefficient to $+1$ and every negative coefficient to $-1$. Hence the diagonal normal form has one positive square for each positive eigenvalue and one negative square for each negative eigenvalue. By [Sylvester's law of inertia](../../../../../../sylvester-s-law-of-inertia.md), these counts do not depend on the diagonalizing basis, so

$$
\boxed{\operatorname{signature}H
=\#\{\lambda_i>0\}-\#\{\lambda_i<0\}}.
$$

The numerical eigenvalues are not invariant under a general [change of basis](../../../../../../change-of-basis.md), because the matrix changes by congruence rather than similarity. For example, on a one-dimensional space let $q(e)=1$. Its matrix in the basis $(e)$ is $(1)$, whereas in the basis $(2e)$ it is $(4)$. The eigenvalue changes from $1$ to $4$, although its sign, and therefore the signature, is unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
