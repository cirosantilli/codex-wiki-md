<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Regard $A$ as a [matrix](../../../../../matrix.md) over the [rational numbers](../../../../../rational-number.md). Part (a)(ii), with $n=2$, gives its [characteristic polynomial](../../../../../characteristic-polynomial.md) $X^2+1$. Therefore, writing $i$ for the [imaginary unit](../../../../../imaginary-unit.md),

$$
\det(iI-A)=i^2+1=0.
$$

The [matrix](../../../../../matrix.md) $M=iI-A$ is not zero: otherwise $A=iI$ would have noninteger diagonal entries. It consequently has [rank of a matrix](../../../../../matrix-rank.md) one over the [fraction field](../../../../../field-of-fractions.md) $\mathbb Q(i)$ of the [Gaussian integers](../../../../../gaussian-integer.md).

By part (b)(i), $\mathbb Z[i]$ is a [euclidean domain](../../../../../euclidean-domain.md), hence a [principal ideal domain](../../../../../principal-ideal-domain.md), so apply [Smith normal form](../../../../../smith-normal-form.md). There exist $P,Q\in\operatorname{GL}_2(\mathbb Z[i])$ such that

$$
P(iI-A)Q=\begin{pmatrix}d&0\\0&0\end{pmatrix},\qquad d\ne0.
$$

Indeed, invertible multiplication preserves [rank of a matrix](../../../../../matrix-rank.md), so exactly one diagonal entry is nonzero. For $e_2=(0,1)^{\mathsf T}$, multiplication on the right gives $P(iI-A)Qe_2=0$. Since $P$ is an [invertible matrix](../../../../../invertible-matrix.md),

$$
\boxed{(iI-A)Qe_2=0}.
$$

The [Smith normal form supplies a kernel basis](../../../../../smith-normal-form-supplies-a-kernel-basis.md) lemma ensures that the null vector $Qe_2$ is a column of an [invertible matrix](../../../../../invertible-matrix.md) over $\mathbb Z[i]$; an arbitrary nonzero solution over $\mathbb Q(i)$ would not itself establish that requirement.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
