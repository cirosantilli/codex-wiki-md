<h1 id="6b/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A matrix and its [matrix transpose](../../../../../../../transpose.md) have the same [characteristic polynomial](../../../../../../../characteristic-polynomial.md), because

$$
\det(\lambda I-A^T)=\det[(\lambda I-A)^T]=\det(\lambda I-A).
$$

Thus they have the same [eigenvalues](../../../../../../../eigenvalue.md), including algebraic multiplicities.

The proposed sum identity is false. For

$$
A=\begin{pmatrix}0&1\\0&0\end{pmatrix},
$$

both eigenvalues $\lambda_i$ are zero, whereas

$$
A^TA=\begin{pmatrix}0&0\\0&1\end{pmatrix}
$$

has eigenvalues $0,1$. Hence

$$
\boxed{\sum_i\mu_i=1\ne0=\sum_i\lambda_i^2}.
$$

Equivalently, the two sides are generally $\operatorname{tr}(A^TA)$ and $\operatorname{tr}(A^2)$, which need not agree.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6B](../../../6b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
