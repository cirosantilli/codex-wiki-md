<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the given [matrix](../../../../../../matrix.md) $A$, the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
\det(A-\lambda I)=(2-\lambda)(1-\lambda)-6=\lambda^2-3\lambda-4=(\lambda-4)(\lambda+1).
$$

For $\lambda=4$, the [eigenvector](../../../../../../eigenvector.md) equation gives $v_2=v_1$; for $\lambda=-1$, it gives $3v_1+2v_2=0$. Thus the [eigenvalues](../../../../../../eigenvalue.md) and their corresponding [eigenspaces](../../../../../../eigenspace.md) are

$$
\boxed{\lambda=4:\ \operatorname{span}\{(1,1)^T\},\qquad \lambda=-1:\ \operatorname{span}\{(2,-3)^T\}.}
$$

For any [eigenvector](../../../../../../eigenvector.md) $v$ with [eigenvalue](../../../../../../eigenvalue.md) $\lambda$, the vector-valued [function](../../../../../../function-split.md) $e^{\lambda x}v$ satisfies $Y'=AY$, since its [derivative](../../../../../../derivative.md) is $\lambda e^{\lambda x}v=e^{\lambda x}Av$. The two displayed [eigenvectors](../../../../../../eigenvector.md) are [linearly independent](../../../../../../linear-independence.md), so the [general solution](../../../../../../general-solution.md) of the [linear system of ordinary differential equations](../../../../../../linear-system-of-differential-equations.md) is

$$
\boxed{\begin{pmatrix}y_1(x)\\y_2(x)\end{pmatrix}=C_1e^{4x}\begin{pmatrix}1\\1\end{pmatrix}+C_2e^{-x}\begin{pmatrix}2\\-3\end{pmatrix},\qquad C_1,C_2\in\mathbb R.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
