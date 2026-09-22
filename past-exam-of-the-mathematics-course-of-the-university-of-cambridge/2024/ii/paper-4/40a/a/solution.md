<h1 id="40a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [power method](../../../../../../power-method.md) starts from $q_0\ne0$ and iterates

$$
q_{j+1}=\frac{Aq_j}{\|Aq_j\|}.
$$

If the [eigenvalue](../../../../../../eigenvalue.md) of largest [modulus](../../../../../../modulus.md) is separated by a [spectral gap](../../../../../../spectral-gap.md) and the initial [vector](../../../../../../vector.md) is [nonorthogonal](../../../../../../nonorthogonal-vectors.md) to a corresponding [eigenvector](../../../../../../eigenvector.md), the iterates converge in direction to that [eigenvector](../../../../../../eigenvector.md).

[Inverse iteration](../../../../../../inverse-iteration.md) with shift $s$ instead solves

$$
(A-sI)y_{j+1}=q_j,
\qquad
q_{j+1}=\frac{y_{j+1}}{\|y_{j+1}\|}.
$$

It applies the [power method](../../../../../../power-method.md) to $(A-sI)^{-1}$ and therefore finds an [eigenvector](../../../../../../eigenvector.md) whose [eigenvalue](../../../../../../eigenvalue.md) is closest to $s$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40A](../../40a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
