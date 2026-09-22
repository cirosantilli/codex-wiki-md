<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A [Hermitian matrix](../../../../../hermitian-operator.md) satisfies $A=A^\dagger$, where $\dagger$ means conjugate transpose. If $Av=\lambda v$ with $v\neq0$, then $v^\dagger Av=\lambda\|v\|^2$ is real, since it equals its complex conjugate $v^\dagger A^\dagger v$. Thus every [eigenvalue](../../../../../eigenvalue.md) is real. To prove the finite-dimensional [spectral theorem](../../../../../spectral-theorem.md), choose a unit [eigenvector](../../../../../eigenvector.md) $v$; one exists because the complex [characteristic polynomial](../../../../../characteristic-polynomial.md) has a root. Its [orthogonal complement](../../../../../orthogonal-complement.md) is invariant, since for $w\perp v$,

$$
v^\dagger Aw=(Av)^\dagger w=\lambda v^\dagger w=0.
$$

The restriction to that complement is again Hermitian. Induction on dimension supplies an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../eigenvector.md), so $A=U\operatorname{diag}(\lambda_1,\ldots,\lambda_n)U^\dagger$ for a [unitary matrix](../../../../../unitary-matrix.md) $U$.

In this basis, $x^\dagger Ax=\sum_i\lambda_i|(U^\dagger x)_i|^2$. Therefore $\boxed{A>0\iff\lambda_i>0\text{ for every }i}$. In that case the [square root of a matrix](../../../../../square-root-of-a-matrix.md)

$$
C=U\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n})U^\dagger
$$

is Hermitian, positive definite and satisfies $C^2=A$. For uniqueness, any positive-definite Hermitian $D$ satisfying $D^2=A$ commutes with $A$ and hence preserves each [eigenspace](../../../../../eigenspace.md) of $A$. Its restriction to the $\lambda$-eigenspace is Hermitian, and its positive [eigenvalues](../../../../../eigenvalue.md) all solve $\mu^2=\lambda$. Thus that restriction is $\sqrt\lambda I$, forcing $D=C$. This is the [principal square root of a positive semidefinite matrix](../../../../../principal-square-root-of-a-positive-semidefinite-matrix.md), here strictly positive definite.

Now let $D=\sqrt B$ and $X=C-D$. Expanding without assuming that $C$ and $D$ commute gives

$$
CX+XC=2C^2-CD-DC=(A-B)+X^2.
$$

The [Hermitian matrix](../../../../../hermitian-operator.md) $X$ has $X^2\geq0$ because $v^\dagger X^2v=\|Xv\|^2$, whereas $A-B>0$. Hence $CX+XC>0$. If $Xv=\mu v$, $v\neq0$, then

$$
0<v^\dagger(CX+XC)v=2\mu\,v^\dagger Cv.
$$

Since $C>0$, every real [eigenvalue](../../../../../eigenvalue.md) $\mu$ of $X$ is positive. The positive-eigenvalue criterion now gives the strict finite-dimensional [operator monotonicity of the square root](../../../../../operator-monotonicity-of-the-square-root.md):

$$
\boxed{CX+XC>0,\qquad \sqrt A-\sqrt B=X>0.}
$$

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
