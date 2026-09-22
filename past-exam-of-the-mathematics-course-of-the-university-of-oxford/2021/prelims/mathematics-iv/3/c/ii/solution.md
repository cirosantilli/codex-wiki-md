<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Let $B=A^TA$. It is a [symmetric matrix](../../../../../../../symmetric-matrix.md), and $\mathbf v^TB\mathbf v=\|A\mathbf v\|^2\geq0$. By the [spectral theorem for real symmetric matrices](../../../../../../../spectral-theorem-for-real-symmetric-matrices.md), choose an [orthonormal basis](../../../../../../../orthonormal-basis.md) $\mathbf v_1,\mathbf v_2,\mathbf v_3$ of [eigenvectors](../../../../../../../eigenvector.md) of $B$, with nonnegative [eigenvalues](../../../../../../../eigenvalue.md) $\lambda_1,\lambda_2,\lambda_3$.

For each $i\ne j$, take the unit [parallelogram](../../../../../../../parallelogram.md) parametrized by $s\mathbf v_i+t\mathbf v_j$, $0\leq s,t\leq1$. Its [surface area](../../../../../../../surface-area.md) is $1$. Moreover,

$$
A\mathbf v_i\cdot A\mathbf v_j=\mathbf v_i^TB\mathbf v_j=0,\qquad
\|A\mathbf v_i\|^2=\lambda_i.
$$

The image [parallelogram](../../../../../../../parallelogram.md) consequently has [area](../../../../../../../surface-area.md) $\sqrt{\lambda_i\lambda_j}$. By the assumption this equals $1$ for all three pairs, giving

$$
\lambda_1\lambda_2=\lambda_1\lambda_3=\lambda_2\lambda_3=1.
$$

No [eigenvalue](../../../../../../../eigenvalue.md) can be zero. Dividing the [equations](../../../../../../../equation.md) and using positivity yields $\lambda_1=\lambda_2=\lambda_3=1$. Hence

$$
\boxed{A^TA=I,\quad\text{so }A\text{ is orthogonal}.}
$$

Thus testing all surfaces is stronger than necessary: the three unit [parallelograms](../../../../../../../parallelogram.md) in these principal directions already determine the result. This is the three-dimensional [characterization of linear surface-area isometries](../../../../../../../characterization-of-linear-surface-area-isometries.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [c](../../c.md)
3. [3](../../../3.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
