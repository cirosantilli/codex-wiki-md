<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [deformation](../../../../deformation-mechanics.md) maps a material point in the reference body to its current position, $y:\Omega\to\mathbb R^3$, with [deformation gradient](../../../../deformation-gradient.md) $F=Dy$. A [homogeneous deformation](../../../../homogeneous-deformation.md) has constant [gradient](../../../../gradient.md) and is affine, $y(X)=FX+b$.

If $\det F>0$, the matrix $F^TF$ is symmetric positive definite. The matrix-square-root theorem says that any such matrix has a unique symmetric positive definite square root, obtained by taking positive square roots in its orthogonal [spectral decomposition](../../../../spectral-decomposition.md). Set

$$
\boxed{U=(F^TF)^{1/2},\qquad R=FU^{-1}.}
$$

Then $R^TR=U^{-1}F^TFU^{-1}=I$ and $\det R=\det F/\det U>0$, so $R\in\mathrm{SO}(3)$ and $F=RU$. If also $F=\widetilde R\widetilde U$, then $F^TF=\widetilde U^2$; [uniqueness](../../../../uniqueness.md) of the positive square root gives $\widetilde U=U$ and then $\widetilde R=R$. This proves **existence and [uniqueness](../../../../uniqueness.md) of [polar decomposition](../../../../polar-decomposition.md)**.

The principal stretches are the positive [eigenvalues](../../../../eigenvalue.md) of $U$, equivalently the [singular values](../../../../singular-value.md) of $F$ or square roots of the [eigenvalues](../../../../eigenvalue.md) of $F^TF$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
