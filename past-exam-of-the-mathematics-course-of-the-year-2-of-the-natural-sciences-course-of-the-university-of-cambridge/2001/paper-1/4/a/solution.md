<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $Av=\lambda v$ for a nonzero [eigenvector](../../../../../eigenvector.md), then $A^2v=\lambda^2v$. Since $A^2=A$, $\lambda(\lambda-1)=0$: every [eigenvalue](../../../../../eigenvalue.md) is zero or one. Let $m$ be the number of ones, counted with [algebraic multiplicity](../../../../../algebraic-multiplicity.md). The [trace](../../../../../matrix-trace.md) is $m$ and the [determinant](../../../../../determinant.md) is the product of these [eigenvalues](../../../../../eigenvalue.md). Therefore

$$
\boxed{m=n:\quad\det A=1,\ \operatorname{tr}A=n;\qquad0\leq m<n:\quad\det A=0,\ \operatorname{tr}A=m.}
$$

Every output $y=Ax$ is fixed by a second application:

$$
\boxed{Ay=A^2x=Ax=y.}
$$

The [image of a linear map](../../../../../image-of-a-linear-map.md) is thus the [eigenspace](../../../../../eigenspace.md) for the [eigenvalue](../../../../../eigenvalue.md) one. To establish its dimension without assuming [diagonalizability](../../../../../diagonalizable-matrix.md), decompose every input as

$$
x=Ax+(I-A)x.
$$

The first term lies in the [image of a linear map](../../../../../image-of-a-linear-map.md) $A$ and the second in its [kernel](../../../../../kernel-of-a-linear-map-split.md). Their intersection is zero, because a vector in the image is fixed by $A$ whereas a vector in the kernel is killed by $A$. Thus the space is their [direct sum](../../../../../direct-sum.md), and an adapted [basis](../../../../../basis.md) puts $A$ into the form $\operatorname{diag}(I_r,0)$, where $r=\operatorname{rank}A$. Comparing [traces](../../../../../matrix-trace.md) gives $r=m$:

$$
\boxed{\dim\operatorname{im}A=n\text{ in case (i)},\qquad\dim\operatorname{im}A=m\text{ in case (ii)}.}
$$

This is an [idempotent linear map](../../../../../projection-linear-algebra.md), and [trace of an idempotent equals its rank](../../../../../trace-of-an-idempotent-equals-its-rank.md). If $m=0$, no nonzero output exists. The dimension in the question refers to the image subspace, including its zero vector.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
