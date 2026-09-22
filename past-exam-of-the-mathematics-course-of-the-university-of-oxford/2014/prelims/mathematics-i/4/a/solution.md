<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A real number $\lambda$ is an [eigenvalue](../../../../../../eigenvalue.md) of $A$ if there is a nonzero [vector](../../../../../../vector.md) $v$ with $Av=\lambda v$; such a $v$ is an [eigenvector](../../../../../../eigenvector.md) for $\lambda$. The nonzero condition is essential.

For distinct [eigenvalues](../../../../../../eigenvalue.md) $\lambda_1,\ldots,\lambda_r$, choose corresponding nonzero [eigenvectors](../../../../../../eigenvector.md) $v_1,\ldots,v_r$. Prove their [linear independence](../../../../../../linear-independence.md) by induction on $r$. The claim for one vector is immediate. Given a relation $\sum_{i=1}^r a_iv_i=0$, apply $A-\lambda_rI$ to get

$$
\sum_{i=1}^{r-1}a_i(\lambda_i-\lambda_r)v_i=0.
$$

By the induction hypothesis, every coefficient here is zero. Distinctness gives $a_i=0$ for $i<r$, and the original relation then gives $a_r=0$ since $v_r\ne0$. Thus the [eigenvectors](../../../../../../eigenvector.md) are [linearly independent](../../../../../../linear-independence.md).

With $n$ distinct real [eigenvalues](../../../../../../eigenvalue.md), the $n$ real [eigenvectors](../../../../../../eigenvector.md) form a [basis](../../../../../../basis.md) of $\mathbb R^n$. Put them into the columns of $P$. Then $P$ is invertible and

$$
AP=P\operatorname{diag}(\lambda_1,\ldots,\lambda_n),
\qquad
\boxed{P^{-1}AP=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This proves [diagonalizability](../../../../../../diagonalizable-matrix.md) directly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
