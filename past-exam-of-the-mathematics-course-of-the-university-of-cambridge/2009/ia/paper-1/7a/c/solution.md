<h1 id="7a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand $x=\sum_j c_jv_j$ in the [orthonormal basis](../../../../../../orthonormal-basis.md) from part (a). Then

$$
\frac{x^\dagger Ax}{x^\dagger x}=\frac{\sum_j\lambda_j|c_j|^2}{\sum_j|c_j|^2}.
$$

For $x\ne0$, the weights $|c_j|^2/\sum_k|c_k|^2$ are nonnegative and sum to one. The [Rayleigh quotient](../../../../../../rayleigh-quotient.md) therefore lies between the smallest and largest [eigenvalues](../../../../../../eigenvalue.md). Conversely, normalized extreme [eigenvectors](../../../../../../eigenvector.md) $v_{\min},v_{\max}$ give, for $0\le t\le1$,

$$
x=\sqrt{1-t}\,v_{\min}+\sqrt t\,v_{\max},\qquad \frac{x^\dagger Ax}{x^\dagger x}=(1-t)\lambda_{\min}+t\lambda_{\max}.
$$

Thus **the exact [Hermitian Rayleigh quotient range](../../../../../../hermitian-rayleigh-quotient-range.md) is**

$$
\boxed{[\lambda_{\min},\lambda_{\max}].}
$$

When $n=1$, the range is the singleton containing the sole [eigenvalue](../../../../../../eigenvalue.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7A](../../7a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
