<h1 id="5b/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $AA^T=I$ and $\det A=1$, $A$ is an [orthogonal matrix](../../../../../../../orthogonal-matrix.md) in the [special orthogonal group](../../../../../../../special-orthogonal-group.md). It also satisfies $A^TA=I$ and thus preserves the [dot product](../../../../../../../dot-product.md). Normalize the fixed [eigenvector](../../../../../../../eigenvector.md) to $e_3=v/\|v\|$. For $u\cdot e_3=0$,

$$
(Au)\cdot e_3=(Au)\cdot(Ae_3)=u\cdot e_3=0,
$$

so the [orthogonal complement](../../../../../../../orthogonal-complement.md) of the fixed axis is invariant. Choose an oriented [orthonormal basis](../../../../../../../orthonormal-basis.md) $e_1,e_2,e_3$. In this basis the [matrix](../../../../../../../matrix.md) has form $\operatorname{diag}(B,1)$, where $B$ is a real $2\times2$ orthogonal matrix of determinant one.

Write the first column of $B$ as $(\cos\theta,\sin\theta)^T$. Its unit second column must be perpendicular to the first; positivity of the determinant selects $(-\sin\theta,\cos\theta)^T$. Thus $B=R(\theta)$, and $A$ fixes the axis through $v$ while rotating its perpendicular plane by $\theta$. Since [trace](../../../../../../../matrix-trace.md) is invariant under change of basis,

$$
\operatorname{tr}A=1+2\cos\theta,\qquad \boxed{\cos\theta=\frac{\operatorname{tr}A-1}{2}.}
$$

This proves that $A$ is the required axial [rotation](../../../../../../../rotation-mathematics.md). The trace determines the unsigned angle; the action in the oriented perpendicular plane determines its sign. The identity case has angle zero and any axis.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5B](../../../5b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
